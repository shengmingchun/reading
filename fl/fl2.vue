<template>
	<view class="">
		<view class="" style="width: 100%;height: 15px;background: whitesmoke;"></view>	
		<view class="" style="width: 100%;height: 190px;">
			<view class="" style="width: 100%;height: 30px;">
				<view class="" style="width: 53%;height: 30px;float: left;padding-left: 10px;font-size:18px;line-height: 30px;font-weight: bold;text-align: left;">
					出版读物
				</view>	
			</view>
			<view class="" style="width: 100%;height: 100px;margin-left: 6px;">
				<view class="" 
				style="width: 30%;height: 30px;float: left; margin-left: 6px; 
				background: whitesmoke;line-height: 30px;margin-top: 5px;text-align: center;border-radius: 5px;" v-for="(obj,index) in arr" :key="index">
					{{obj}}
				</view>
				
			</view>
		</view>		
	</view>
</template>

<script>
	export default {
		data() {
			return {				
				arr: ['名家经典','婚姻两性','教育教辅','生活休闲','美食旅行','经管理财','养生保健','励志成功','历史百科',
				'外国名著','童话寓言','社科科普','社会百态','散文诗歌','古典文学','传记纪实','畅销小说','影视文学']				
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
