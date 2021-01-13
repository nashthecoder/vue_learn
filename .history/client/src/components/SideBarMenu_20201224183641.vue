<template>
<SideBarMenu :menu="menu" />
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
          href: "/",
          title: "Home"
        }
      ]
    }
  }
}
</script>
