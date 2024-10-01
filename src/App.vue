<script setup>
import Card from './components/baitap/Card.vue';
import Bai1 from './components/baitap/Bai1.vue'
import Bai2 from './components/baitap/Bai2.vue'
import Bai3 from './components/baitap/Bai3.vue'
import Bai4 from './components/baitap/Bai4.vue'
import Bai5 from './components/baitap/Bai5.vue'
import Bai6 from './components/baitap/Bai6.vue'
import Bai7 from './components/baitap/Bai7.vue'
import Bai8 from './components/baitap/Bai8.vue'
import { ref } from 'vue'

const Bai1Parent = 'Rikkei Academy'
const Bai2Parent = {
  id:1,
  name:"Bưởi",
  price:11000,
  quantity:4
}
const Bai3Count = ref(0)
const handleMessage=()=>{
  Bai3Count.value++
}
const Bai4Id=ref(0)
const handleMessage4=(id)=>{
  console.log(11111111111,id);
  Bai4Id.value=id;
}
const title='Thông báo từ hệ thống'
const content='Đây là nội dung của modal. Bạn có thể đóng modal bằng cách nhấn vào nút Close'
const Bai5Status=ref(true);
const handleMessage5=(status)=>{
  Bai5Status.value=status;
}
</script>

<template>
  <div>
    <Bai1 :Childen='Bai1Parent'></Bai1>
    <Bai2 :Childen='Bai2Parent'></Bai2>
    <h1>bài 3</h1>
    <p>{{Bai3Count}}</p>
    <Bai3 @messageSent='handleMessage'></Bai3>
    <h1>bài 4</h1>
    <p v-if="Bai4Id==0">id to delete: </p>
    <p v-else>id to delete: {{Bai4Id}}</p>
    <Bai4 @messageSent='handleMessage4'></Bai4>
    <h1>bài 5</h1>
    <p v-if="Bai5Status==true"><Bai5 @messageSent='handleMessage5' :titleProp='title' :contentProp='content'></Bai5></p>
    <p v-else></p>
    <Bai6>
      <template #header>
        <h3>Thông tin sản phẩm</h3>
      </template>
      <template #body>
        <p>Đây là mô tả ngắn gọn về sản phẩm này. Sản phẩm có các tính năng nổi bật và giá cả hợp lý.</p>
      </template>
      <template #footer>
        <button>Xem chi tiết</button>
      </template>
    </Bai6>
  </div>
</template>

<style>

</style>