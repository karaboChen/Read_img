<script setup>
import { ref, onMounted } from 'vue'
import { Get_user } from './backend/api.js'


const aa = ref('')

async function G_img() {

   // export const Get_user = (a) => instance.get(`/quailty/pic?ID=${a}`,{responseType: 'arraybuffer'});
   // let res = await Get_user('1239817')
   // const url = URL.createObjectURL(new Blob([res.data]))
   // aa.value=url
  
  //  export const Get_user = (a) => instance.post(`/quailty/pic`,a,{responseType: 'arraybuffer'});
  //  let res = await Get_user({ ID: '1239817' })
  //  const url = URL.createObjectURL(new Blob([res.data]))
  //  aa.value = url

   // [HttpGet("/quailty/pic")]   HttpPost    FromBody
   // public IActionResult 圖片([FromQuery] 彩色圖片 e)
   // {
   //   using var cn = new SqlConnection(_configuration.GetConnectionString("local"));

   //   var sql = @" SELECT   [Graph_Path]
   //                FROM [#1HSM_DC].[dbo].[5_Color_Graph]
   //                where   Coil_ID =@id and  Direction='1'";
   //   var data = cn.Query<南北回傳>(sql, new { id = e.ID }).ToList();
   //   var  returnValue = System.IO.File.ReadAllBytes(data[0].Graph_Path);
   //   return File(returnValue, "image/jpg");
   // }

   //---------------------------------------------------
 
}
onMounted(() => {
   G_img()
})

</script>

<template>
   <img :src="aa" alt="">
</template>

<style scoped></style>