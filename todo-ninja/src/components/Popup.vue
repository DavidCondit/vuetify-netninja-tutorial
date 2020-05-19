<template>

<v-dialog v-model="dialog" max-width="600px">
      
      <template v-slot:activator="{ on }">
        <v-btn class="success" text v-on="on">
            Add new project
        </v-btn>
      </template>

      <v-card>
        <v-card-title primary-title>
          Add a New Project
        </v-card-title>

        <v-card-text>

          <v-form class="px-3" ref="form">
            <v-text-field label="Title" v-model="title" prepend-icon="mdi-folder" :rules="inputRules"></v-text-field>
            <v-textarea label="Information" v-model="content" prepend-icon="mdi-pencil" :rules="inputRules"></v-textarea>

            <v-menu>
                <template v-slot:activator="{ on }">
                    <v-text-field :value="formattedDate" v-on="on" label="Due date" prepend-icon="mdi-calendar-month" :rules="inputRules"></v-text-field>
                </template>
                <v-date-picker v-model="due"></v-date-picker>            
            </v-menu>
        
            <v-btn text class="success mx-0 mt-3" @click="submit">Add project</v-btn>
          </v-form>

        </v-card-text>

      </v-card>

    </v-dialog>

</template>

<script>
import format from 'date-fns/format'
import parseISO from 'date-fns/parseISO'

export default {  
    data() {
        return {
            title: '',
            content: '',
            due: null,
            inputRules: [
                v => v.length >= 3 || 'Minimum length is 3 characters'
            ]
        }
    },
    methods: {
        submit() {
            if (this.$refs.form.validate()) {
                console.log(this.title, this.content, this.due)
            }            
        }
    },
    computed: {
        formattedDate() {
            return this.due ? format(parseISO(this.due), 'd MMM yyyy') : ''
        }
    }
}


</script>