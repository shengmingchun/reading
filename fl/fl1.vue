<template>
	<view class="">
		<view class="" style="width: 100%;height: 15px;background: whitesmoke;"></view>	
		<view class="" style="width: 100%;height: 210px;">
			<view class="" style="width: 100%;height: 30px;">
				<view class="" style="width: 53%;height: 30px;float: left;padding-left: 10px;font-size:18px;line-height: 30px;font-weight: bold;text-align: left;">
					男频
				</view>	
			</view>
			<view class="" style="width: 100%;height: 100px;margin-left: 6px;">
				<view class="" 
				style="width: 30%;height: 30px;float: left; margin-left: 6px; 
				background: whitesmoke;line-height: 30px;margin-top: 10px;text-align: center;border-radius: 5px;" v-for="(obj,index) in arr" :key="index">
					{{obj}}
				</view>
				
			</view>
		</view>		
	<view class="" style="width: 100%;height: 15px;background: whitesmoke;"></view>
		<view class="" style="width: 100%;height: 210px;">
			<view class="" style="width: 100%;height: 30px;">
				<view class="" style="width: 99%;height: 30px;float: left;padding-left: 10px;font-size:18px;line-height: 30px;font-weight: bold;text-align: left;">
					女频
				</view>	
			</view>
			<view class="" style="width: 100%;height: 100px;margin-left: 6px;">
				<view class="" 
				style="width: 30%;height: 30px;float: left; margin-left: 6px; 
				background: whitesmoke;line-height: 30px;margin-top:10px;text-align: center;border-radius: 5px;" v-for="(obj,index) in srr" :key="index">
					{{obj}}
				</view>
				
			</view>
		</view>		
	<view class="" style="width: 100%;height: 40px;background: whitesmoke;"></view>
	</view>
</template>

<script>
	export default {
		data() {
			return {				
				arr: ['玄幻奇幻','都市异能','官场职场','武侠奇缘','历史风云','军事战争','转世重生','游戏竞技','科幻时空',
				'无限流派','同人小说','古典仙侠'],
				srr: ['古风古言','穿越重生','幻想言情','宫廷宅斗','女尊王朝','种田经商','都市言情','青春校园','网游情缘',
				'耽美百合','悬疑灵异','短篇小说']
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
