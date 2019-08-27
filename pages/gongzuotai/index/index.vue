<template>
	<view class="container">
		<view class="content">
			<!-- 顶部是管理员操作选项，权限足够才可以显示 -->
			<!-- 项目列表九宫格 -->
			<view class="example-body">
				<uni-grid :column="3" :show-border="true" :square="true" :hor="35" :ver="-45" @change="change">
					<uni-grid-item marker="dot">
						<image class="image" src="https://img-cdn-qiniu.dcloud.net.cn/uni-ui/grid-1.png" mode="aspectFill" />
						<text class="text">新浪</text>
					</uni-grid-item>
					<uni-grid-item marker="badge" text="99" type="success">
						<image class="image" src="https://img-cdn-qiniu.dcloud.net.cn/uni-ui/grid-2.png" mode="aspectFill" />
						<text class="text">微信</text>
					</uni-grid-item>
					<uni-grid-item marker="badge" type="error" text="热">
						<image class="image" src="https://img-cdn-qiniu.dcloud.net.cn/uni-ui/gird-3.png" mode="aspectFill" />
						<text class="text">QQ</text>
					</uni-grid-item>
					<uni-grid-item :hor="35" :ver="-45" :img-width="25" marker="image" src="https://img-cdn-qiniu.dcloud.net.cn/uni-ui/recommend.png">
						<image class="image" src="https://img-cdn-qiniu.dcloud.net.cn/uni-ui/grid-6.png" mode="aspectFill" />
						<text class="text">抖音</text>
					</uni-grid-item>
				</uni-grid>
			</view>
		</view>
	</view>
</template>

<script>
	import uniGrid from '@/components/uni-grid/uni-grid.vue'
	import uniGridItem from '@/components/uni-grid-item/uni-grid-item.vue'
	export default {
		components: {
			uniGrid,
			uniGridItem
		},
		data() {
			return {

			}
		},
		methods: {

		}
	}
</script>

<style>
	.image {
		width: 50upx;
		height: 50upx;
	}
	
	.text {
		font-size: 26upx;
		margin-top: 10upx;
	}
</style>
