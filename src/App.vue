<template>
  <div class="scroll text-center d-flex justify-content-center position-relative">

    <h1 class="scroll-text  ">S</h1>
    <h1 class="scroll-text ">c</h1>
    <h1 class="scroll-text ">r</h1>
    <h1 class="scroll-text ">o</h1>
    <h1 class="scroll-text ">l</h1>
    <h1 class="scroll-text ">l</h1>
    <h1 class="scroll-text "> </h1>
    <h1 class="scroll-text ">d</h1>
    <h1 class="scroll-text ">o</h1>
    <h1 class="scroll-text ">w</h1>
    <h1 class="scroll-text ">n</h1>

  </div>
</template>
<script>
import gsap from "gsap";

export default {
  data:()=>({

  }),
  methods:{
    // text() {
    //   const tl = gsap.timeline({
    //     // repeat: -1,
    //     // yoyo: false,
    //   });
    //   tl.to('.header-letter', {duration: 0.65,top: -100,y: -100,right: 100,x: 100,opacity: 1,stagger: 0.25,ease: "slow"});
    //
    // },

    scrollanimatext(){
      const tl=gsap.timeline({
        repeat:-1,
        yoyo:true
      });
      tl.to('.scroll-text ',{duration: 0.65,top: 35,y:35,right: 100,x: 100,opacity: 1,stagger: 0.25,ease: "slow"})
      tl.to('.scroll ',{duration: 0.65,top: 0,y: 0,right: 0,x: 0,opacity: 1,stagger: 0.25,ease: "slow"})
    },

  },
  mounted() {
    // this.text();

    this.scrollanimatext();
  }

}


</script>



<style lang="scss">

.scroll-text {
  padding-top: 100px;
  opacity: 0;
//&::after {
   //  content: '';
   //  position: absolute;
   //  width: 35px;
   //  height: 35px;
   //  background-image: url("/media/svg/down-arrow-svgrepo-com.svg");
   //  background-size: cover;
   //  transform: rotate(90deg);
   //  animation: scroll-down 1s infinite;
   //}
}
</style>
