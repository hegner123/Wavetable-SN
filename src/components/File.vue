<template>
    <div class="row bg-light p-lg-4 p-2">
      <div class="col-6 ">
        <h4> {{title}}</h4>
        <ul>
        <li v-for="tags in tags" :key="tags.tag" class="tags">
         <a v-bind:href="tags.link"> <span>{{ tags.tag }} </span></a>
          </li>
        </ul>
      </div>
      <div class="col-6">
        <div class="download-link">
          <a :href="download"> Download </a>
        </div>
        
      </div>
    </div>
</template>

<script>


export default {
  name: 'File',
  props: {
    title: String
  },

  data(){
      return {
          tags:[
            {tag:"saw",
            link:"#"},
            {tag:"soft",
            link:"#"}
            ],
            download:"link"
      }
  }
}
</script>

<style scoped>
a{
  text-decoration: none;
  color:#636363;
}
.tags{
  list-style: none;
  display:inline;
  padding-left:5px;
}
.tags:first-child{
  padding-left:0px;
}
ul{
  padding:0px;
  margin:0px;
}

.download-link{
  align-items: center;
  display:flex;
  height:100%;
  justify-content: flex-end;
  padding:10px;
}

</style>
