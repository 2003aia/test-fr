<template>
  <div class="main">
    <form @submit.prevent="onSubmit">
      <select v-model="select">
        <option value="">Выберите условие</option>

        <option value="type">Тип карты лояльности</option>
        <option value="status">Статус карты лояльности</option>
      </select>
      <br />

      <select v-model="select2" v-if="select == 'type'">
        <option value="">Выберите условие</option>

        <option value="gold">Gold</option>
        <option value="silver">Silver</option>
      </select>

      <select v-model="select3" v-if="select == 'status'">
        <option value="">Выберите условие</option>

        <option value="gold">Активна</option>
        <option value="silver">Неактивна</option>
      </select>
      <br />

      <button>
        Отправить
      </button>
    </form>

    <p>Нажмите чтобы добавить новое условие выборки.</p>
  </div>
</template>
<script>


  
export default {
  data() {
    return {
      select: "",
      select2: "",
      select3: "",
    };
  },
  name: "Form",
  methods: {
    onSubmit() {
        
      console.log(this.select2, this.select3,);
    },
  },
};
</script>
<style scoped>
select {
  margin-top: 20px;
  padding: 10px 10px 10px 10px;
  font-size: 17px;
  border-radius: 10px;
  border-color: rgba(170, 170, 170, 0.753);
  width: 100%;
  max-width: 400px;
}

.main {
  display: flex;
  flex-direction: column;
}
button {
  margin-top: 20px;
  background: rgba(0, 0, 0, 0.055);
  border: none;
  border-radius: 50%;
  width: 50px;
  height: 50px;
}
button:hover {
  background: rgba(0, 0, 0, 0.123);
}
</style>