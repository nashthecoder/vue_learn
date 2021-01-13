<template>
<sidebar-menu :menu="menu" />
</template>
<script>
export default {
  components: {
    SideBarMenu,
  },
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
