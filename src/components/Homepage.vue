<template>
  <div class="container mt-5">
    <div class="row">
      <div class="col-12 col-lg-6">
        <div class="row">
          <div class="col-12">
          <h1>Wavetable SN</h1>
          <p>A community driven wavetable sharing platform.</p>
          </div>
        </div>
        <div class="row mt-5">
          <div class="col-12">
            <h2>Uploaded Wavetables</h2>
          </div>
        </div>
        <div class="row">
          <div class="col-12 wavetables">
          <File title="test"></File>
          </div>
        </div>
      </div>
    </div>



  </div>
</template>

<script>
import File from './File'

export default {
  name: 'Homepage',
  components: {
    File
  },
  data(){
    return{
      entry:{
        title:"test"
      }
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.wavetables{
  border:solid 1px black;
  height:500px;
}
</style>
