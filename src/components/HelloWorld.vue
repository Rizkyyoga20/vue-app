<template>
  <h3 style="text-align:left; margin:0px; padding:3px 0px;">Form Entry Produk</h3>
  <input type="text" v-model="id_produk" placeholder="ID Produk" required><br>
  <input type="text" v-model="nama_produk" placeholder="Nama Produk" required><br>
  <input type="number" v-model="harga" placeholder="Harga produk" required><br>
  <input type="number" v-model="stok" placeholder="Stok" required><br>
  <textarea v-model="keterangan" placeholder="Keterangan" />

<h4 style="text-align:left;">
  {{ id_produk }}<br> 
  {{ nama_produk }}<br>
  {{ harga }}<br>
  {{ stok }}<br>
  {{ keterangan }}<br>
</h4>
</template>

<style scoped>
.read-the-docs {
  color: #888;
}
input, textarea{
  padding:10px;
  margin:3px;
  border-radius:5px;
  background:#c0c0c0;
  border:none;
  width:100%;
}
input::placeholder, textarea::placeholder{
  color:#000;
  font-size:15px;
}
</style>


<script setup>
import { ref } from 'vue'

defineProps({
  msg: String,
})

const count = ref(0)

const id_produk = ref('')
const nama_produk = ref('')
const harga = ref('')
const stok = ref('')
const keterangan = ref('')

</script>