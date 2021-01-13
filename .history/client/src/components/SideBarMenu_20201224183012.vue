<template>
 <side-bar-menu :menu="menu" />
</template>
<script>
 export default {
   data() {
     return {
       menu: [
         {
           header: true,
           title: "Main Navigation",
           hiddenOnCollapse: true
         },
         {
           href: "/",
           title: "Home"
         }
       ]
     }
   }
 }
</script>
