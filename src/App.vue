<script setup>
import NavbarAlert from './components/NavbarAlert.vue';
import CardAlert from './components/CardAlert.vue';
import { ref, onMounted, onUnmounted, computed, nextTick, watch } from 'vue';

const scrolled = ref(false)
const isLoading = ref(true)
const cardToBeHidden = ref(false)

const onScroll = () => {
  if (window.scrollY > 107) {
    scrolled.value = true
  }
}

const hideCard = () => {
  cardToBeHidden.value = true
  localStorage.setItem('cardToBeHidden', 'true')
}

const showCard = computed(() => !isLoading.value && scrolled.value && !cardToBeHidden.value)

onMounted(async () => {
  await nextTick()
  cardToBeHidden.value = localStorage.getItem('cardToBeHidden')
  isLoading.value = false
  window.addEventListener('scroll', onScroll)
})
onUnmounted(() => {
  window.removeEventListener('scroll', onScroll)
})

</script>

<template>
  <main>
    <NavbarAlert/>
    <CardAlert :showCard="showCard" @hideCard="hideCard" />
  </main>
</template>