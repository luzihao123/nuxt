<template>
	<div>
		<h2>news 首页</h2>
		<h3>News ID:{{$route.params.id}}</h3>
		<ul>
			<li>
				<!-- <a href="/">home</a>
				<a href="/news/123">123NEWS</a>
				<a href="/news/456">456news</a> --><a href="/news/123">123NEWS</a>
				<nuxt-link :to="{name:'index'}">home</nuxt-link>
				<nuxt-link :to="{name:'news-id',params:{'id':123,'title':'i am news'}}">123NEWS</nuxt-link>
				<nuxt-link :to="{path:'/news/456'}">456news</nuxt-link>
			</li>
		</ul>
	</div>
</template>
<script>
export default {
	transition:'test'
}
</script>

