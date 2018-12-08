<template>
	<div>
		<h2 v-if="error.statusCode==404">404页面。你需要的没有找到</h2>
		<h2 v-else>500页面</h2>
	</div>
</template>

<!--自定义错误页面  error.statusCode中包含错误代码-->
<script>
export default {
	props:['error']
}
</script>
