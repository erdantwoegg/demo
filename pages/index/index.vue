<template>
	<view class="out">
		<navigator url="/pages/list/list">跳转其他页面</navigator>
		<video src="@/static/image/video.mp4"></video>
		<image mode="aspectFill" src="@/static/image/微信图片_20240701181103.jpg" class="my_img"></image>
		<view class="box">1</view>
		<icon type="success" size="26" />
		<view>uniapp</view>
		<view>web前端</view>
		<text user-select selectable>nodejs</text>
		<text space="nbsp">aaaaa nodejs</text>
		<scroll-view class="scroll" scroll-x scroll-y>
			<view class="group">
				<view class="item">
					111
				</view>
				<view class="item">
					222
				</view>
				<view class="item">
					333
				</view>
				<view class="item">
					444
				</view>
				<view class="item">
					555
				</view>
				<view class="item">
					111
				</view>
				<view class="item">
					111
				</view>
				<view class="item">
					111
				</view>
				<view class="item">
					111
				</view>
			</view>
		</scroll-view>
		<swiper class="swiper" indicator-dots circular autoplay :interval="3000">
			<swiper-item>
				<view class="swiper-item">
					<image src="../../static/image/jd2.png" mode="scaleToFill"></image>
				</view>
			</swiper-item>
			<swiper-item>
				<view class="swiper-item">
					<image src="../../static/image/barc1.png" mode="scaleToFill"></image>
				</view>
			</swiper-item>
		</swiper>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				title: 'Hello'
			}
		},
		onLoad() {

		},
		methods: {

		}
	}
</script>

<style lang="scss">
	.out {
		.box {
			width: 750rpx;
			height: 200rpx;
			background-color: pink;
		}
	}

	.scroll {
		border: 1px solid red;
		box-sizing: border-box;
		height: 100rpx;

		.group {
			white-space: nowrap;

			.item {
				width: 220rpx;
				height: 220rpx;
				background-color: chartreuse;
				display: inline-block;
				margin-right: 10px;
			}
		}
	}

	.swiper {
		height: 400rpx;

		.swiper-item {
			padding: 0 20rpx;
			box-sizing: border-box;

			image {
				width: 100%;
				height: 400rpx;
			}
		}
	}

	.my_img {
		width: 300rpx;
		height: 300rpx;
	}
</style>