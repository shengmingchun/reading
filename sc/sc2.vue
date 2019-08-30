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
				arr:[{'src':'../../static/img/djdh.jpg','name':'大江大河'},{'src':'../../static/img/rrz.jpg','name':'如懿传'},
				{'src':'../../static/img/gdjzj.jpg','name':'古董局中局'}],
				arr1:[{'src':'../../static/img/sdyxz.jpg','name':'射雕英雄传'},{'src':'../../static/img/xkx.jpg','name':'侠客行'},
				{'src':'../../static/img/lxfcq.jpg','name':'陆小凤传奇'}],
				arr2:[{'src':'../../static/img/mdzz.jpg','name':'密道追踪'},{'src':'../../static/img/hhgg.jpg','name':'黄河鬼棺全集'},
				{'src':'../../static/img/gmts.jpg','name':'鬼墓天书'}],
				arr3:[{'src':'../../static/img/cndqsjlg.jpg','name':'从你的全世界路过'},{'src':'../../static/img/yzcc.jpg','name':'一座城池'},
				{'src':'../../static/img/ssyp.jpg','name':'四十一炮'}],
				arr4:[{'src':'../../static/img/fyz.jpg','name':'父与子'},{'src':'../../static/img/snwczfn.jpg','name':'少年维持之烦恼'},
				{'src':'../../static/img/bngd.jpg','name':'百年孤独'}],
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
