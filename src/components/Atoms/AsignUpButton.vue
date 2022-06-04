 <template>
   <button class="signup">SIGN-UP NOW!</button>
 </template>
 
 <script>
 export default {
     name: 'AsignUpButton'
 }
 </script>
 
 <style scoped>
 .signup{
    border: 2px solid var(--primary-color);
    color: white;
    font-weight: 600;
    padding: var(--xs);
    background-color: transparent;
    transition: background-color .2s ease-out;
    max-height: var(--m);
 }
 .signup:hover{
    background-color: var(--primary-color);
    cursor: pointer;
 }
 </style>