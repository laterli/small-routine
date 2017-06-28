<template>
	<div class="div">
		<h3>评论</h3>
		<ul class="ul">
			<li class="li" v-for="contents in content">
				{{contents}}
			</li>
		</ul>
	</div>
</template>
<script>
	export default {
		computed:{
			content:function(){
				return this.$store.state.content
			}
		}
	}
</script>
<style>
.div{
	height:8rem;
}
	h3{
		margin:0;
		padding:0;
		font-size: 0.5rem;
	}
	li{
		font-size: 0.5rem;
	}
	.ul{
		height:8rem;
		border:0.1rem solid #000;
		overflow: hidden;
	}
</style>