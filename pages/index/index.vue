<template>
	<view class="homeLayout">
		<view class="banner">
			<swiper indicator-dots indicator-color="rgb(255,255,255,0.5)" autoplay interval="3000" duration="2000" circular>
				<swiper-item v-for="i in 3">
					<image src="../../common/images/banner3.jpg" mode="aspectFill"></image>
				</swiper-item>
			</swiper>
		</view>
		<view class="notice">
			<view class="left">
				<uni-icons type="sound" size="28" color="#2daf88"></uni-icons>
				<text>
					公告
				</text>
			</view>
			<view class="center">
				<swiper vertical autoplay circular duration="2000">
					<swiper-item v-for="i in 3">
						文字内容文字内容文字内容文字内容文字内容文字内容文字内容文字内容文字内容文字内容文字内容文字内容文字内容文字内容文字内容
					</swiper-item>
				</swiper>
			</view>
			<view class="right">
				<uni-icons type="forward" size="22"></uni-icons>
			</view>
		</view>
		
		<view class="select">
			<commit-title></commit-title>
			<view class="content">
				<scroll-view scroll-x>
					<view class="box" v-for="i in 8">
						<image src="../../common/images/preview_small.webp" mode="aspectFill"></image>
					</view>
				</scroll-view>
			</view>
		</view>
	</view>
</template>

<script setup>
	
</script>

<style lang="scss" scoped>
.homeLayout{
	.banner{
		width: 750rpx;
		// background-color: #ccc;
		padding: 30rpx 0rpx;
		swiper{
			width: 750rpx;
			height: 340rpx;
			swiper-item{
				width: 100%;
				height: 100%;
				padding: 0rpx 30rpx;
				image{
					width: 100%;
					height: 100%;
					border-radius: 10rpx;
				}
			}
		}
	}
	.notice{
		width: 690rpx;
		height: 80rpx;
		background-color: #f9f9f9;
		display: flex;
		margin: 0 auto;
		line-height: 80rpx;
		border-radius: 80rpx;
		.left{
			width: 140rpx;
			display: flex;
			align-items: center;
			justify-content: center;
			text{
				color: #2daf88;
				font-weight: 600;
				font-size: 28rpx;
				padding:0 5rpx;
			}
		}
		.center{
			flex: 1;
			padding-right: 5rpx;
			swiper{
				height: 100%;
				
				&-item{
					height: 100%;
					overflow: hidden;
					white-space: nowrap;
					text-overflow: ellipsis;
				}
			}
		}
		.right{
			width: 70rpx;
			display: flex;
			align-items: center;
			justify-content: center;
		}
	}
	
	.select {
		padding-top:50rpx;
		.content{
			width: 690rpx;
			margin: 30rpx 30rpx 0rpx 30rpx;
			scroll-view{
				white-space: nowrap;
				.box{
					width: 200rpx;
					height: 430rpx;
					display: inline-block;
					margin-right: 15rpx;
					image{
						width: 100%;
						height: 100%;
						border-radius: 15rpx;
						}
				}
				.box:last-child{
					margin-right: 0rpx;
				}
			}
		}
	}
}
</style>
