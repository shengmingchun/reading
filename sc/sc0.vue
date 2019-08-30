<template>
	<view class="">
		<view class="" style="width: 100%;height: 10px;background: whitesmoke;"></view>	
		<view class="" style="width: 100%;height: 190px;">
			<view class="" style="width: 100%;height: 30px;">
				<view class="" style="width: 53%;height: 30px;float: left;padding-left: 10px;font-size:18px;line-height: 30px;font-weight: bold;">
					特别热
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
						新秀作
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
						被收藏
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
						小情怀
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
						完结啦
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
				arr:[{'src':'../../static/img/zcdrfsa.jpg','name':'总裁大人,放肆爱'},{'src':'../../static/img/kcnpswsc.jpg','name':'快穿之女配上...'},
				{'src':'../../static/img/ydsj.jpg','name':'医毒双绝:冥...'}],
				arr1:[{'src':'../../static/img/lgsdw.jpg','name':'世纪第一宠婚...'},{'src':'../../static/img/btca.jpg','name':'许你盛世安宁'},
				{'src':'../../static/img/njxfn.jpg','name':'随身空间:农...'}],
				arr2:[{'src':'../../static/img/zcdrfsa.jpg','name':'总裁大人,放肆爱'},{'src':'../../static/img/gykf.jpg','name':'邪王嗜宠:鬼...'},
				{'src':'../../static/img/hslr.jpg','name':'婚色撩人:司...'}],
				arr3:[{'src':'../../static/img/mmxhn.jpg','name':'年先生,慢慢...'},{'src':'../../static/img/jbddxd.jpg','name':'你是我戒不掉...'},
				{'src':'../../static/img/nfbjnqs.jpg','name':'暖风不及你情深'}],
				arr4:[{'src':'../../static/img/mmza.jpg','name':'名门挚爱:帝...'},{'src':'../../static/img/kcnpswsc.jpg','name':'快穿之女配上...'},
				{'src':'../../static/img/hslr.jpg','name':'婚色撩人:司...'}],
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
