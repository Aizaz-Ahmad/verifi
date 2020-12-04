<template>
  <div>
    <Header v-if="false"/>
    <Platforms id="second-section" v-if="false"/>
    <HowItWorks/>
    <ContactUs v-if="false"/>
    <PopupOne v-if="false" />
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
