<template>
  <div class="pos">
    <div>
        <el-row >
            <el-col :span='7' class="pos_order" id="order_list">
            我是订单栏
            </el-col>
            <!--商品展示-->
            <el-col :span="17">
             我是产品栏
            </el-col>
        </el-row>
    </div>
  </div>
</template>
 
<script>
export default {
  name: 'Pos',
  mounted:function(){
      var orderHeight=document.body.clientHeight;
      document.getElementById("order_list").style.height=orderHeight+'px';
  },
}
</script>
<style scoped>
	.pos_order{
		background-color: #f9fafc;
		border-right: 1px solid #c0ccda;

	}
</style>