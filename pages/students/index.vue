<template>
  <div class="students">
    <h2>生徒一覧</h2>
    <ul>
      <li><NuxtLink :to="{path: '/students/0',}">{{ students[0].name }}</NuxtLink></li>
      <li><NuxtLink :to="{path: '/students/1',}">{{ students[1].name }}</NuxtLink></li>
      <li><NuxtLink :to="{path: '/students/2',}">{{ students[2].name }}</NuxtLink></li>
    </ul>
    <NuxtLink to="/">戻る</NuxtLink>  </div>
</template>


<script>
export default {
  data() {
    return {
      students: [
        {
          id: "qnfungqxllc3m1ak",
          name: "生徒A",
        },
        {
          id: "7j9cumkgsq6l264c",
          name: "生徒B",
        },
        {
          id: "eo34bhey9m0d92ou",
          name: "生徒C",
        },
      ],
    };
  },
};
</script>


<style>
.students {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  text-align: center;
}
</style>