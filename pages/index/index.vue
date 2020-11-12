<template>
	<view class="content">
		<view @click="toDetail">
			<myAudio></myAudio>
		</view>
	</view>
</template>

<script>
	import myAudio from "../../components/myaudio/myaudio"
	export default {
		data() {
			return {
				title: 'Hello'
			}
		},
		components: {
			myAudio
		},
		onLoad() {

		},
		methods: {
			toDetail() {
				uni.navigateTo({
					url: '../music-detail/music-detail'
				})
			}
		}
	}
</script>

<style>
	.content {
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;
	}

	.logo {
		height: 200rpx;
		width: 200rpx;
		margin-top: 200rpx;
		margin-left: auto;
		margin-right: auto;
		margin-bottom: 50rpx;
	}

	.text-area {
		display: flex;
		justify-content: center;
	}

	.title {
		font-size: 36rpx;
		color: #8f8f94;
	}
</style>
