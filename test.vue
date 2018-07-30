<template>
<div class="test">
<h1>This is my first app</h1>
<h2>{{title}}</h2>
<div><button v-on:click="todos">todos</button></div>
<div><button v-on:click="photos">photos</button></div>
<div><button v-on:click="posts">posts</button></div>
<div><button v-on:click="comments">comments</button></div>
<div><button v-on:click="albums">albums</button></div>
<div><button v-on:click="users">users</button></div>

</div>
</template>


<script>
export default {
	name: 'test',
	data() {
		return {
			title:'Hello App',
		}
	},
methods:{
        todos:function(){
        	   return
                  fetch('https://jsonplaceholder.typicode.com/todos/1')
                 .then(response => response.json())
                  .then(json => console.log(json))
         }
         
    },

methods:{
      	photos:function(){
      		  return
      		fetch('https://jsonplaceholder.typicode.com/photos')
                 .then(response => response.json())
                  .then(json => console.log(json))
      	}
      },

methods:{
      	photos:function(){
      		  return
      		fetch('https://jsonplaceholder.typicode.com/posts')
                 .then(response => response.json())
                  .then(json => console.log(json))
           }
},
          
methods:{
      	photos:function(){
      		  return
      		fetch('https://jsonplaceholder.typicode.com/comments')
                 .then(response => response.json())
                  .then(json => console.log(json))
           }
        

	},
methods:{
      	photos:function(){
      		  return
      		fetch('https://jsonplaceholder.typicode.com/albums')
                 .then(response => response.json())
                  .then(json => console.log(json))
           }
},
methods:{
      	photos:function(){
      		  return
      		fetch('https://jsonplaceholder.typicode.com/users')
                 .then(response => response.json())
                  .then(json => console.log(json))
     
          }
      }
}

</script>

<style scoped>


</style>

