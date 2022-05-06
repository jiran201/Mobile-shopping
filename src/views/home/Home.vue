<template>
  <div class="wrapper">
    <StaticPart />
    <Nearby />
    <Docker :currentIndex="0"/>
  </div>
</template>

<script>
import StaticPart from './StaticPart'
import Nearby from './Nearby'
import Docker from '../../components/Docker'
export default {
  name: 'Home',
  components: { StaticPart, Nearby, Docker }
}
</script>

<style lang="scss" scoped>
.wrapper {
  overflow-y: hidden;
  position: absolute;
  left: 0;
  top: 0;
  bottom: 0;
  right: 0;
  padding: 0 .18rem .1rem .18rem;
}
</style>
