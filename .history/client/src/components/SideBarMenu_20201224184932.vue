<template>
  <sidebar-menu :menu="menu" />
</template>
<script>
export default {
  components: {},
  data() {
    return {
      menu: [
        {
          header: true,
          title: "Main Navigation",
          hiddenOnCollapse: true
        },
        {
          href: "/dashboard",
          title: "Dashboard"
        }
      ]
    }
  }
}
</script>
