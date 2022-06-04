<template>
  <header-test :esta_logado="false"/>
  <FirstComponent />
  <life-cycle />
  <people-data />
</template>

<script>
import HeaderTest from "./components/HeaderTest.vue";
import FirstComponent from "./components/FirstComponent.vue";
import LifeCycle from "./components/LifeCycle.vue";
import PeopleData from "./components/PeopleData.vue";

export default {
  name: "App",
  components: { FirstComponent, LifeCycle, PeopleData, HeaderTest },
};
</script>


<style>
body {
  background-color: #333;
  color: #fff;
}
a{
  color: red;
}
</style>