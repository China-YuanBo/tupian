<template>
	<view class="content">
		<view class="left">
			<slot name="left"></slot>
		</view>
		<view class="right">
			<slot name="right"></slot>
		</view>	
	</view>	
</template>

<script setup>
	
</script>

<style lang="scss" scoped> 
.content{
			display: flex;
			justify-content: space-between;
			align-items: center;
			padding:0 30rpx 0 30rpx;
			.left{
				font-size: 38rpx;
			}
		
		}
</style>