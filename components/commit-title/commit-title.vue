<template>
	<view class="content">
		<view class="left">
			每日推荐
		</view>
		<view class="right">
			<uni-icons type="calendar-filled" size="28"></uni-icons>
			<uni-dateformat :date="Date.now()" format="dd号"></uni-dateformat>
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
	.left{
		font-size: 38rpx;
	}
	.right
	{
		display: flex;
		justify-content: center;
		align-items: center;
		font-size: 28rpx;
	}
}
</style>