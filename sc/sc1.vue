<template>
	<view class="">
		<view class="" style="width: 100%;height: 10px;background: whitesmoke;"></view>	
		<view class="" style="width: 100%;height: 190px;">
			<view class="" style="width: 100%;height: 30px;">
				<view class="" style="width: 53%;height: 30px;float: left;padding-left: 10px;font-size:18px;line-height: 30px;font-weight: bold;">
					热书榜
				</view>
				<view class="" style="width: 40%;height: 30px;float: left;text-align: right;padding-right: 10px;font-size:12px;line-height: 30px;">
					更多>
				</view>
			</view>
			<view class="" style="width: 100%;height: 150px;">
				<view class="" style="width: 30%;height: 110px;float: left; margin-left: 6px;" v-for="(obj,index) in arr" :key="index">
					<view class="" style="width: 70%;height:100px;margin-top: 10px;margin-left: 15px;">
						<image :src="obj.src" mode="" style="width: 100%;height: 100px;"></image>
					</view>
					<view class="" style="width: 70%;height: 10px;margin-top: 2px;margin-left: 15px;font-size: 12px;font-weight: bold;">
						{{obj.name}}
					</view>
				</view>	
			</view>
		</view>	
		<view class="" style="width: 100%;height: 10px;background: whitesmoke;"></view>
		<view class="" style="width: 100%;height: 190px;">
				<view class="" style="width: 100%;height: 30px;">
					<view class="" style="width: 53%;height: 30px;float: left;padding-left: 10px;font-size:18px;line-height: 30px;font-weight: bold;">
						潜力榜
					</view>
					<view class="" style="width: 40%;height: 30px;float: left;text-align: right;padding-right: 10px;font-size:12px;line-height: 30px;">
						更多>
					</view>
				</view>
				<view class="" style="width: 100%;height: 150px;">
					<view class="" style="width: 30%;height: 110px;float: left; margin-left: 6px;" v-for="(obj1,index1) in arr1" :key="index1">
						<view class="" style="width: 70%;height:100px;margin-top: 10px;margin-left: 15px;">
							<image :src="obj1.src" mode="" style="width: 100%;height: 100px;"></image>
						</view>
						<view class="" style="width: 70%;height: 10px;margin-top: 2px;margin-left: 15px;font-size: 12px;font-weight: bold;">
							{{obj1.name}}
						</view>
					</view>	
				</view>
		</view>
		<view class="" style="width: 100%;height: 10px;background: whitesmoke;"></view>
		<view class="" style="width: 100%;height: 190px;">
				<view class="" style="width: 100%;height: 30px;">
					<view class="" style="width: 53%;height: 30px;float: left;padding-left: 10px;font-size:18px;line-height: 30px;font-weight: bold;">
						收藏榜
					</view>
					<view class="" style="width: 40%;height: 30px;float: left;text-align: right;padding-right: 10px;font-size:12px;line-height: 30px;">
						更多>
					</view>
				</view>
				<view class="" style="width: 100%;height: 150px;">
					<view class="" style="width: 30%;height: 110px;float: left; margin-left: 6px;" v-for="(obj2,index2) in arr2" :key="index2">
						<view class="" style="width: 70%;height:100px;margin-top: 10px;margin-left: 15px;">
							<image :src="obj2.src" mode="" style="width: 100%;height: 100px;"></image>
						</view>
						<view class="" style="width: 70%;height: 10px;margin-top: 2px;margin-left: 15px;font-size: 12px;font-weight: bold;">
							{{obj2.name}}
						</view>
					</view>	
				</view>
		</view>
			<view class="" style="width: 100%;height: 10px;background: whitesmoke;"></view>
			<view class="" style="width: 100%;height: 190px;">
				<view class="" style="width: 100%;height: 30px;">
					<view class="" style="width: 53%;height: 30px;float: left;padding-left: 10px;font-size:18px;line-height: 30px;font-weight: bold;">
						完本榜
					</view>
					<view class="" style="width: 40%;height: 30px;float: left;text-align: right;padding-right: 10px;font-size:12px;line-height: 30px;">
						更多>
					</view>
				</view>
				<view class="" style="width: 100%;height: 150px;">
					<view class="" style="width: 30%;height: 110px;float: left; margin-left: 6px;" v-for="(obj3,index3) in arr3" :key="index3">
						<view class="" style="width: 70%;height:100px;margin-top: 10px;margin-left: 15px;">
							<image :src="obj3.src" mode="" style="width: 100%;height: 100px;"></image>
						</view>
						<view class="" style="width: 70%;height: 10px;margin-top: 2px;margin-left: 15px;font-size: 12px;font-weight: bold;">
							{{obj3.name}}
						</view>
					</view>	
				</view>
			</view>	
			<view class="" style="width: 100%;height: 10px;background: whitesmoke;"></view>
			<view class="" style="width: 100%;height: 190px;">
				<view class="" style="width: 100%;height: 30px;">
					<view class="" style="width: 53%;height: 30px;float: left;padding-left: 10px;font-size:18px;line-height: 30px;font-weight: bold;">
						经典榜
					</view>
					<view class="" style="width: 40%;height: 30px;float: left;text-align: right;padding-right: 10px;font-size:12px;line-height: 30px;">
						更多>
					</view>
				</view>
				<view class="" style="width: 100%;height: 150px;">
					<view class="" style="width: 30%;height: 110px;float: left; margin-left: 6px;" v-for="(obj4,index4) in arr4" :key="index4">
						<view class="" style="width: 70%;height:100px;margin-top: 10px;margin-left: 15px;">
							<image :src="obj4.src" mode="" style="width: 100%;height: 100px;"></image>
						</view>
						<view class="" style="width: 70%;height: 10px;margin-top: 2px;margin-left: 15px;font-size: 12px;font-weight: bold;">
							{{obj4.name}}
						</view>
					</view>	
				</view>
			</view>	
		<view class="" style="width: 100%;height: 30px;background: whitesmoke;line-height: 30px;text-align: center;">
			我是有底线的
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				arr:[{'src':'../../static/img/zqsjxt.jpg','name':'最强升级系统'},{'src':'../../static/img/wgtd.jpg','name':'万古天帝'},
				{'src':'../../static/img/ysdz.jpg','name':'一世独尊'}],
				arr1:[{'src':'../../static/img/jmdy.jpg','name':'将门毒医大小姐'},{'src':'../../static/img/ypl.jpg','name':'穿越网王之音飘零'},
				{'src':'.../../static/img/cyxj.jpg','name':'穿越星际:妻荣夫贵'}],
				arr2:[{'src':'../../static/img/yszt.jpg','name':'一术镇天'},{'src':'../../static/img/btca.jpg','name':'病态宠爱'},
				{'src':'../../static/img/ysdz.jpg','name':'一世独尊'}],
				arr3:[{'src':'.../../static/img/jzjy.jpg','name':'九真九阳'},{'src':'../../static/img/wsfb.jpg','name':'武神风暴'},
				{'src':'../../static/img/jsws.jpg','name':'绝世武神'}],
				arr4:[{'src':'../../static/img/hfxx.jpg','name':'化凡修仙'},{'src':'../../static/img/yzww.jpg','name':'妖者为王'},
				{'src':'../../static/img/tgsz.jpg','name':'太古神主'}],
			}
		},
		onLoad() {
	
		},
		methods: {
			
		}
	}
</script>

<style>
</style>
