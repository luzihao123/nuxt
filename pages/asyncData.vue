<template>
	<div>
		{{name}}
		{{info.name}}
	</div>
</template>
<script>
import axios from 'axios'
export default {
	data(){
		return {
			name:"Hello World"
		}
	},
	// asyncData(){
	// 	return axios.get('https://api.myjson.com/bins/jbopi').then(res=>{
	// 		return {
	// 			info:res.data
	// 		}
	// 	})
	// }
	async asyncData(){
		let {data} = await axios.get('https://api.myjson.com/bins/jbopi')
		return {
			info : data
		}
	}
}
</script>
