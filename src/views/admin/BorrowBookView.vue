<template>
    <div class="d-flex justify-space-around">
      <v-menu>
        <template v-slot:activator="{ props }">
          <v-btn color="primary" v-bind="props"> Activator slot </v-btn>
        </template>
        <v-list>
          <v-list-item v-for="(item, index) in items" :key="index" :value="index">
            <v-list-item-title>{{ item.title }}</v-list-item-title>
          </v-list-item>
        </v-list>
      </v-menu>

      <v-btn color="primary">
        Parent activator

        <v-menu activator="parent">
          <v-list>
            <v-list-item v-for="(item, index) in items" :key="index" :value="index">
              <v-list-item-title>{{ item.title }}</v-list-item-title>
            </v-list-item>
          </v-list>
        </v-menu>
      </v-btn>

      <v-btn id="menu-activator" color="primary"> Sibling activator </v-btn>

      <v-menu activator="#menu-activator">
        <v-list>
          <v-list-item v-for="(item, index) in items" :key="index" :value="index">
            <v-list-item-title>{{ item.title }}</v-list-item-title>
          </v-list-item>
        </v-list>
      </v-menu>
    </div>
</template>
<script setup lang="ts">
import { ref } from 'vue'

const items = ref([
  { title: 'huy đẹp trai' },
  { title: 'Click Me' },
  { title: 'Click Me' },
  { title: 'Click Me' },
])
</script>

<style scoped></style>
<!-- đống này chỉ test hãy sửa lại tùy ý -->
