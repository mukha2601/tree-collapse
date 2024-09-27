<template>
  <div class="wrapper">
    <tree-select :data="data" />
  </div>
</template>

<script setup>
import { ref } from "vue";

const data = ref([
  {
    id: 1,
    name: "Users",
    level: 0,
    children: [
      {
        id: 11,
        name: "Teachers",
        level: 1,
        children: [
          {
            id: 1,
            name: "Students",
            level: 0,
            children: [
              {
                id: 11,
                name: "boys",
                level: 1,
                children: [
                  {
                    id: 111,
                    name: "mukha",
                    level: 2,
                  },
                ],
              },
              {
                id: 12,
                name: "girls",
                level: 1,
              },
            ],
          },
        ],
      },
      {
        id: 12,
        name: "Admins",
        level: 1,
      },
    ],
  },
]);
</script>


