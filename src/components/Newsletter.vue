<script>

export default {

  data() {
    
    return {
       emailme :"" , 
       errors : []

  }  
  },
   methods : {
     checkForm: function(e){
        

       this.errors = [];
       if(!this.emailme){
         this.errors.push('Email Required ! ')
       }else if(!this.validEmail(this.email)) {
                   this.errors.push('Valid email required. ')
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
      <form
      method="POST"
      action="http://localhost:3000"
      enctype="multipart/form-data"
      v-on:submit.prevent="checkForm" 

    >
    <h3 class="text-[20px] leading-10 text-center sm:text-justify">Suscribed to our NewsLetter</h3> 
                 <p class="text-center sm:text-justify ">Available exclusivery on Figmaland</p>
      <div class="grid sm:flex flex-row py-6 sm:py-8"> 
      <div class="py-2 sm:py-0 sm:ml-5">          
      
        <input
          name="emailme" 
          type="emailme"
          id="emailme"
          :value="emailme"
          @input="event => emailme = event.target.value"   
          class="bg-gray-200 appearance-none border-2 border-gray-200 rounded-full w-full py-2 px-4 text-gray-700 leading-tight focus:outline-none focus:bg-white focus:border-purple-500"
          placeholder="Your email "
        />
        <p v-if="errors.length">
            <b>Please correct the following error(s):</b>
            <ul>
              <li v-for="error in errors">{{ error }}</li>
            </ul>
        </p>
        
      </div> 
      <div class="mb-6  ">
        <button
          type="submit"
          class="          
            h-10
            px-5
            text-indigo-100
            bg-[#2091F9]
            rounded-full
            transition-colors
            duration-150
            focus:shadow-outline
            hover:bg-indigo-800
            w-full 
            md:ml-2
          "
        >
          Subscribe 
        </button>
      </div>
      </div>
      
    </form>
        
        

</template>

<style scoped>

</style>
