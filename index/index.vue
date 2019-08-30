<template>
	<view class="">
		<view class="top" style="width: 100%;height: 60px;background: #DD524D;position: fixed;">
			<view class="text-area" style="width: 40%;height: 60px;float: left;" @click="ct">
				<image src="../../static/img/qita.png" mode="" style="width: 20%;height: 30px;
				margin-top: 25px;margin-left: 16px;"></image>
			</view>
			<view class="text-area" style="width: 20%;height: 30px;float: left;padding-top: 30px;color: white;text-align: center;">
				阅读
			</view>
			<view class="text-area" style="width: 38%;height: 60px;float: left;" @click="ss">
				<image src="../../static/img/ss.png" mode="" style="width: 15%;height: 20px;
				margin-top: 30px;margin-left: 87px;"></image>
			</view>
		</view>
		<view>
			<uni-drawer :visible="f" @close="f=!f" :mask="true" style="width: 100%;">
			<view class="" style="width: 100%;height: 19%"></view>
			<view class="" style="width: 100%;height: 10%">
				<view class="" style="width: 100%;height: 50%;padding-left: 30px;">阅读记录</view>
				<view class="" style="width: 100%;height: 50%;padding-left: 30px;">下载管理</view>
			</view>
			<view class="" style="width: 100%;height: 3%;background: #C8C7CC;"></view>
			<view class="" style="width: 100%;height:10%">
				<view class="" style="width: 100%;height: 50%;padding-left: 30px;">同步书架</view>
				<view class="" style="width: 100%;height: 50%;padding-left: 30px;">导入本地书籍</view>	
				
			</view>
			<view class="" style="width: 100%;height: 3%;background: #C8C7CC;"></view>
			<view class="" style="width: 100%;height:15%">
				<view class="" style="width: 100%;height: 33%;padding-left: 30px;">平铺排列书籍</view>
				<view class="" style="width: 100%;height: 33%;padding-left: 30px;">隐藏私密</view>
				<view class="" style="width: 100%;height: 33%;padding-left: 30px;">更多设置</view>
			</view>
			<view class="" style="width: 100%;height: 35%"></view>
			<view class="" style="width: 100%;height: 5%;padding-left: 30px;">夜间模式</view>
			</uni-drawer>
		</view>
		<view class="m" style="width: 99%;height: 110px;padding-top: 60px; border-bottom: 1px solid whitesmoke;" v-for="(obj,index) in arr" :key="index">
			<view class="" style="margin-top: 5px;padding-left: 15px;width: 20%;height: 90px; float: left;">
				<image :src="obj.src" mode="" style="width: 100%;height: 90px;"></image>
			</view>
			<view class="" style=" width: 70%;height: 20px; float: left;"></view>
			<view class="" style=" width: 70%;height: 21px; float: left;margin-left: 10px;">
				{{obj.name}}
			</view>
			<view class="" style=" width: 70%;height: 10px; float: left;"></view>
			<view class="" style=" width: 70%;height: 15px; float: left;font-size: 13px;margin-left: 10px;">
				今天  更新 :{{obj.up}}
			</view>
		</view>
	</view>
</template>

<script>
	import uniDrawer from "@/components/uni-drawer/uni-drawer.vue"
	import uniList from '@/components/uni-list/uni-list.vue'
	import uniListItem from '@/components/uni-list-item/uni-list-item.vue'
	export default {
		components: {uniDrawer,uniList,uniListItem},
		data() {
			return {
				title: 'Hello',
				f:false,
				arr:[{'src':'../../static/img/djdh.jpg','name':'大江大河','up':'第一章'}]
			}
		},
		onLoad() {
	
		},
		methods: {
			ct(){
				this.f=true;
			},
			ss(){
				uni.navigateTo({
					url:'search'
				})
			}
		}
	}
</script>

<style>
</style>
