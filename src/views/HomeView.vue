<template>
  <div class="home">
    
    <homeHeader/>
    <HomeCommunity/>
    <mission/>
    <directions/>
    <end/>
  </div>
</template>

<script>
// @ is an alias to /src

import homeHeader from '@/components/homeHeader';
import HomeCommunity from '@/components/HomeCommunity';
import mission from '@/components/mission';
import directions from '@/components/directions';
import end from '@/components/end.vue'

export default {

  components: {
    homeHeader,
    HomeCommunity,
    mission,
    directions,
    end
  }
}
</script>
<style lang="scss">

</style>
