<template>
  <div id="app">
    <div class="row">
      <Header />
      <div class="col s12 m10 offset-m1">
        <a v-for="tab in tabs" :key="tab" @click="selected = tab.elem;":class="['tab-btn', { active: selected === tab.elem }]">{{ tab.name }}</a>
      </div>
      <Profession />
      <component :is="selected"></component>
      <SideMenu />
      <Footer />
    </div>
  </div>
</template>

<script>
import Header from '@/components/Header'
import Profession from '@/components/Profession'
import CardsBlock from '@/components/CardsBlock'
import CardsBlock2 from '@/components/CardsBlock2'
import CardsBlock3 from '@/components/CardsBlock3'
import CardsBlock4 from '@/components/CardsBlock4'
import SideMenu from '@/components/SideMenu'
import Footer from '@/components/Footer'
export default {
  name: 'App',
  components: {
    Header,
    Profession,
    SideMenu,
    CardsBlock,
    CardsBlock2,
    CardsBlock3,
    CardsBlock4,
    Footer
  },
  data: function() {
   return {
     tabs: [{name:"ОПЫТ", elem:"CardsBlock"}, {name:"ОБРАЗОВАНИЕ", elem:"CardsBlock2"}, {name:"ПОРТФОЛИО", elem:"CardsBlock3"}, {name:"GITHUB", elem:"CardsBlock4"},],
     selected: "CardsBlock"
   };
 }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: left;
  color: #2c3e50;
  background-color: #C9D6FF;
  background-image: linear-gradient(45deg, #C9D6FF 0%, #f2fcfe 100%);

}


.tab-btn {
  color: #0088cc;
  cursor: pointer;
  padding: 10px 30px;
  margin-left: 20px;
}

.active {
  border-radius: 5px;
  background: #29c5e6;
  color: #fff;
  box-shadow: 4px 5px 5px rgba(0,0,0,0.3);
}

.card-panel.grey.lighten-5.z-depth-3 {
  border-radius: 7px;
}

.page-footer {
  background: #297de6;
}

hr {
  color: #7e7e7e;
}

Footer {
  position: fixed;
  bottom: 0;
}

</style>
