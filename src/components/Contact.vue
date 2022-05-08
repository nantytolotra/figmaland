<script>

export default {

  data() {
    
    return {
       email :"" ,
       name :"" ,
       massage :"" , 

       errors : []

  }  
  },
   mounted() {
            console.log('Upload component', this.message);
        }, 
   methods : {
     checkForm: function(e){
        

       this.errors = [];
       if(!this.email){
         this.errors.push('Email Required ! ')
       }else if(!this.validEmail(this.email)) {
                   this.errors.push('Valid email required. ')
       }

       if(!this.name){
         this.errors.push('Name Required ! ')
       }

       if(!this.message){
         this.errors.push('Message Required ! ')
       }
      e.preventDefault()
     },
     validEmail : function(email){
       var re=/^(([^<>()[\]\\.,;:\s@"]+(\.[^<>()[\]\\.,;:\s@"]+)*)|(".+"))@((\[[0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}\])|(([a-zA-Z\-0-9]+\.)+[a-zA-Z]{2,}))$/;
       re.test(email)

     }
   }
} 
</script>
<template>
 <form    v-on:submit.prevent="checkForm"  method="POST" action="https://herotofu.com/start" enctype="multipart/form-data" class="m-8">
      <h3 class="text-[20px] leading-10">Contact Us</h3> 
       <p v-if="errors.length">
            <b>Please correct the following error(s):</b>
            <ul>
              <li v-for="error in errors">{{ error }}</li>
            </ul>
        </p>
    
      <div class="grid grid-row py-6 w-64 " > 
    
      <div class="py-6">          
        <input name="name" type="text" id="name" v-model="name" class="bg-gray-200 appearance-none border-2 border-gray-200 rounded-full w-full py-2 px-4 text-gray-700 leading-tight focus:outline-none focus:bg-white focus:border-purple-500"
          placeholder="Your Name"
        />
      </div>
      
      <div class="py-6">          
        <input name="email" type="email" id="email" v-model="email" class=" bg-gray-200 appearance-none border-2 border-gray-200 rounded-full w-full py-2 px-4 text-gray-700 leading-tight focus:outline-none focus:bg-white focus:border-purple-500"
          placeholder="Your Email"
        />
      </div>
      <div class="">          
        <textarea name="message" type="text" id="message" v-model="message"  class="bg-gray-200 appearance-none border-2 border-gray-200  w-full h-32 py-2 px-4 text-gray-700 leading-tight focus:outline-none focus:bg-white focus:border-purple-500"
          placeholder="Your Message"
        />
      </div> 
      <div class="mb-6">
        <button type="submit" class="h-10 px-5 text-indigo-100 bg-[#2091F9] rounded-full transition-colors duration-150 focus:shadow-outline  hover:bg-indigo-800">
          Send
        </button>
       </div>
      </div>      
    </form>
</template>

<style scoped>

</style>
