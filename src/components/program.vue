<template>
	<div class="program">
		<v-header title='我的模板' class="index"></v-header>
		<div class="program-content">
			 <div class="left"><img src="../assets/img/beautiful.jpg" alt=""></div>
			 <div class="right"><img src="../assets/img/beautiful.jpg" alt=""></div>
			 <div class="left"><img src="../assets/img/beautiful.jpg" alt=""></div>
			 <div class="right"><img src="../assets/img/beautiful.jpg" alt=""></div>
			 <div class="left"><img src="../assets/img/beautiful.jpg" alt=""></div>
			 <div class="right"><img src="../assets/img/beautiful.jpg" alt=""></div>
		</div>
		<mt-search
      v-model="value"
      class="search"
    ></mt-search>
	</div>
</template>

<script>
	import header from '../views/header'

	export default {
		components:{'v-header':header},
    data(){
		  return {
		     value:''
      }
    }
	}
</script>

<style>
  .search{
    z-index: 999;
    height: 0.5rem;
    position: fixed;
    width: 100%;
    top: 0.4rem;
  }
	.program-content{
		margin-top: 0.85rem;
		margin-bottom: 0.51rem;
		display: flex;
		justify-content: space-between;
    flex-wrap:wrap;
	}
	.program-content .left img,
	.program-content .right img{
		width: 100%;
		height: 100%;
	}

	.program-content .left,.program-content .right{
    width: 49%;
		height: 2rem;
		margin-top: 0.15rem;
	}
	
		
	.index{
		z-index: 100;
	}
</style>
