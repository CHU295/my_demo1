<template>
	<div class="admin-header">
		<div class="admin-header-left">
			<div class="logo">有家早教</div>
			<div class="mystore" @click='jump'>前台首页</div>
			<div class="logout" @click='jump0'>退出登录</div>
		</div>
	</div>
</template>
<script>
	export default{
		methods:{
			jump(){
				this.$router.push({name:'index'})
			},
			jump0(){
				localStorage.clear()
				this.$router.push({name:'login'})
			}
		}
	}
</script>