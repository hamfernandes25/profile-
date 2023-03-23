<template>
 <div class="cars"><ul>
  <li><CardView />
    </li>
    <li><CardView />
    </li>
    <li><CardView />
    </li>
  </ul>
 
  </div>
</template>



<script>
//import HelloWorld from './components/HelloWorld.vue'
import CardView from './card.vue'

export default {
  name: 'CarasolVieww',
  components: {
   // HelloWorld,
    CardView,
  }
}
</script>

<style>

.dat{
  display: flex;
  position: relative;
  left:-100px;
  max-width:340px;
}
.cars{
  display: flex;
  justify-content:baseline ;
}
</style>
