<template src="js/three.js">
  <!-- <div></div> -->
</template>

<script>
// import { Clock, PerspectiveCamera, Scene, WebGLRenderer } from 'three'
import * as THREE from 'three'
// import { render } from 'vue';
const renderer = new THREE.WebGLRenderer();
renderer.setSize(window.innerWidth, window.innerHeight);

document.body.appendChild(renderer.domElement);

const scene = new THREE.Scene();
const camera = new THREE.PerspectiveCamera(
  75,
  window.innerWidth / window.innerHeight,
  0.1,
  1000,
)
renderer.render(scene, camera);
export default {

}
</script>
<!-- <style src="../assets/css/canvas.css" lang="scss"></style> -->
