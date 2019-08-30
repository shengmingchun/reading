
 <template>
    <view class="content">
        <mSearch @search="search($event,0)"></mSearch>
       <!-- <view class="cnaps  borderBottom">
           <text>所在城市</text>
           <input class='m-bbt' placeholder-class='plhStyle' type='number' maxlength='50' placeholder='' bindinput="bindKeyInput" value='{{province}} {{city}}' disabled></input>
         </view> -->
    </view>
 </template>

 <script>
	 import mSearch from '@/components/mehaotian-search/mehaotian-search.vue';
	 export default {
	    components: {
	        mSearch
	    },
	    data() {
	        return {
	            val0: '',
	            val1: '',
	            val2: '',
	            val3: '',
	            placeholder:'动态占位内容'
	        };
	    },
	 
	    methods: {
	        search(e, val) {
	            console.log(e, val);
	            this['val'+val] = e;
	        }
	    }
	 };
 </script>
 
 