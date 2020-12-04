<template>
  <div>
    <Header/>
    <PopupOne v-if="false" />
    <ContactUs v-if="false" />
    <HowItWorks v-if="false"/>
    <Platforms v-if="false"/>
  </div>
</template>

<script>
import Header from './components/Header'
import PopupOne from './components/Popup-one';
import ContactUs from './components/Contact-Us'
import HowItWorks from './components/How-It-Works'
import Platforms from './components/Platforms'
export default {
  name: 'App',
  components: {
    PopupOne,
    ContactUs,
    HowItWorks,
    Platforms,
    Header
  },
};
</script>

<style scoped>
  
</style>
