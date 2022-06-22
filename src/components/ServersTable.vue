<template>
  <table class="ui basic unstackable table" id="table">
    <thead>
    <tr>
      <th id="status4">運行狀態</th>
      <th id="name">名稱</th>
      <th id="type">類型</th>
      <th id="location">位置</th>
      <th id="uptime">上線時間</th>
      <th id="load">負載</th>
      <th id="network">网络 ↓|↑</th>
      <th id="traffic">流量 ↓|↑</th>
      <th id="cpu">CPU</th>
      <th id="ram">記憶體</th>
      <th id="hdd">磁碟</th>
    </tr>
    </thead>
    <tbody id="servers">
    <!-- Servers here \o/ -->
    <!--
    use index for the key may cause performance issues when delete a server from array,
    but not a big matter and we cannot find a more suitable data for the unique key.
    -->
    <table-item v-for="(server, index) of servers" :key="index" :server="server"/>
    </tbody>
  </table>
  <p> * 當負載超過了50%(0.50),伺服器處理效能會降低,並會在運行狀態上顯示過載中且背景改為黃色. </p>
  <p> * 當負載超過了150%(1.5),伺服器負載達到極限值,並會在運行狀態上顯示過載中且背景改為紅色. </p>
</template>
<script lang="ts">
import { defineComponent, PropType } from 'vue';
import TableItem from '@/components/TableItem.vue';

export default defineComponent({
  name: 'ServersTable',
  props: {
    servers: {
      type: Array as PropType<Array<StatusItem | BoxItem>>,
      default: () => ([])
    }
  },
  components: {
    TableItem
  }
});
</script>
<style>
#table {
  font-size: 1rem;
  border: none;
  text-align: center;
  vertical-align: middle;
}

#table thead tr th {
  color: #9da2a6;
  white-space: nowrap;
}
</style>
