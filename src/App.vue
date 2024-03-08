<script>
import { RouterView } from 'vue-router';
import { onMounted, ref } from 'vue';


export default {
  setup() {
    const vantaRef = ref(null);

    onMounted(() => {
      VANTA.BIRDS({
        el: vantaRef.value,
        mouseControls: true,
        touchControls: true,
        gyroControls: false,
        minHeight: 200,
        minWidth: 200,
        backgroundColor: 0x003d5b,
        color1: 0x00798c,
        color2: 0xedae49,
        birdSize: 1.75
      });
    });
    return {
      vantaRef,
    };
  },
};
</script>

<template>

  <div ref="vantaRef" class="birds">
    <div class="titre">
      <h1 class="text-center mt-3 m-2">Bonjour</h1>
      <h2 class="text-center m-4">Bienvenue sur mon site</h2>
    </div>

    <img class="phone"
      src="https://assets-global.website-files.com/61e3320964dda631e9ba335e/63e92e30cd3678841d6d1ec4_63c6688162d9338f735a916a_iPhone14-space-black.svg"
      alt="téléphone">
    
    <div class="titre">
      <h3 class="text-center mt-3">Pour vivre l'experience veuillez scroller</h3>
    </div>

  </div>
  
  <RouterView />
</template>

<style scoped>

.birds {
  height: 100vh;
  display: flex;
  flex-direction: column;
  align-items: center;
  z-index: 0;
}
h1{
  font-family: "Dancing Script", cursive;
  font-size: 3.5rem;
  font-weight: 400;
}

h2, h3{
  font-weight: 400;
  font-style: italic;
  font-size: 1.5rem;
}
.titre {
  color: #edae49;
  font-family: "Playfair Display", serif;
}

.phone {
  height: 60vh;
  z-index: 16;
  background-image: linear-gradient(75deg,#00798c, #30638e);
  border-radius: 45px;
}


</style>
