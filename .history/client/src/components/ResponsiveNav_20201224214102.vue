<template>
  <nav :style="{ background: background || '#333' }">
    <ul :style="{ background: background || '#333' }"ref="nav">
      <figure class="image-logo" @click="toggleNav">
        <img :src="imagePath" height="40px" width="40px" />
      </figure>
      <li v-for="(link, index) navLinks" :key="index" 
        @mouseenter="$event.currentTarget.style.background = hoverBackground || '#999'"
				@mouseleave="$event.currentTarget.style.background = background || '#333'"
        >
        <router-link
					:to="link.path"
					:style="{ color: linkColor || '#DDD' }"
				>
					{{ link.text }}
					<i :class="link.icon" />
				</router-link>
      </li>
    </ul>
  </nav>
</template>
<script>
export default {
  
}
</script>
<style scoped>

</style>
