<template>
	<view class="" style="width: 100%;height: auto;">
		<view class="top" style="width: 100%;height: 60px;background: #DD524D;position: fixed;z-index: 5">
			<view class="text-area" style="width: 40%;height: 60px;float: left;"   @click="ct">
				<image src="../../static/img/qita.png" mode="" style="width: 20%;height: 30px;
				margin-top: 25px;margin-left: 16px;"></image>
				
			</view>
			<view class="text-area" style="width: 20%;height: 30px;float: left;padding-top: 30px;color: white;text-align: center;">
				书城
			</view>
			<view class="text-area" style="width: 38%;height: 60px;float: left;" @click="ss">
				<image src="../../static/img/ss.png" mode="" style="width: 15%;height: 20px;
				margin-top: 30px;margin-left: 87px;"></image>
			</view>
		</view>
		<view>
			<uni-drawer :visible="f" @close="f=!f" :mask="!f" style="width: 100%;">
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
		<view class="" style="width: 99%;height: 30px;margin-top: 60px;position: fixed;z-index: 5;">	    
			<wuc-tab :tab-list="tabList" textFlex :tabCur.sync="TabCur" tab-class="text-center text-black bg-white" select-class="text-orange" ></wuc-tab>
		</view>	
		<view class="" style="width: 99%;height: 30px;padding-top: 103px;">
			<swiper :current="TabCur" class="" duration="300" :circular="true" indicator-color="rgba(255,255,255,0)" indicator-active-color="rgba(255,255,255,0)" @change="swiperChange" style="height: 1030px;width: 100%;">
				<swiper-item v-for="(item,index) in tabList" :key="index" >
				  <view class="bg-white padding margin text-center text-black" v-show="index==0">
					    <sc1></sc1>
				  </view>
				  <view class="bg-white padding margin text-center text-black" v-show="index==1">
				  		<sc0></sc0>
				  </view>
				  <view class="bg-white padding margin text-center text-black" v-show="index==2">
				  	    <sc2></sc2>
				  </view>
				</swiper-item>
			</swiper>	
		</view>
			     			
		
		
	</view>
</template>

<script>
	import sc1 from '../sc/sc1.vue'
	import sc0 from '../sc/sc0.vue'
	import sc2 from '../sc/sc2.vue'
	import WucTab from '@/components/wuc-tab/wuc-tab.vue'
	import uniDrawer from "@/components/uni-drawer/uni-drawer.vue"
	import uniList from '@/components/uni-list/uni-list.vue'
	import uniListItem from '@/components/uni-list-item/uni-list-item.vue'
	export default {
		components: {uniDrawer,uniList,uniListItem,WucTab,sc1,sc0,sc2},
		data() {
			return {
				title: 'Hello',
				f:false,
				TabCur: 0,
				tabList: [{ name: '男生' }, { name: '女生' }, { name: '图书' }]
			}
		},
		onLoad() {
	
		},
		methods: {
			ct(){
				this.f=true;
			},
			tabChange(index) {
				if (this.TabCur !=index) {
				    this.TabCur = index;
				}
			},
		    swiperChange(e) {
				let { current } = e.target;
				this.TabCur = current;
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
