<template>           
	<div>
		<h2>newsContent</h2>
		<p>newsID:{{$route.params.id}}</p>
		<ul>
			<li><nuxt-link :to="{name:'index'}">Home</nuxt-link></li>
		</ul>
	</div>
</template>
<script>
// 动态路由
export default {
	validate({params}){
		return /^\d+$/.test(params.id);    // id错误情况跳转至404页面
	},
	data(){
		return{
			title:this.$route.params.title
		}
	},
	head(){
		return {
			title:this.title,
			meta:[
				{hid:'description',name:'news1',content:'this is news page'}
			]
		}
	}
}
</script>
