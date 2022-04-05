<template>
  <ul>
    <div class="redCircle"></div>
    <li>
      <NuxtLink exact active-class="active" class="li" to="/quizes">
        <span class="material-icons-outlined">feed</span>
        Опросы
      </NuxtLink>
    </li>
    <li>
      <NuxtLink exact active-class="active" class="li" to="/users"
        ><span class="material-icons-outlined"> people </span> Пользователи
      </NuxtLink>
    </li>
    <li>
      <NuxtLink exact active-class="active" class="li" to="/blacklists"
        ><span class="material-icons-outlined"> flag </span> Черные списки
      </NuxtLink>
    </li>

    <li>
      <NuxtLink exact active-class="active" class="li" to="/center"
        ><span class="material-icons-outlined"> call </span> Колл-центр
      </NuxtLink>
    </li>
  </ul>
</template>

<script>
export default {
  name: "Navbar",
};
</script>

<style scoped>
span {
  width: fit-content;
  font-size: 48px;
}

.li {
  color: black;
  width: 150px;
  height: 100px;
  justify-content: center;
  align-items: center;
  display: flex;
  flex-direction: column;
  font-weight: normal;
  font-size: 17px;
  text-decoration: none;
  border-radius: 10px;
}

.li:hover {
  background: rgba(0, 0, 0, 0.055);
  border-radius: 10px;
  font-weight: bold;
}
ul {
  padding: 0;
  margin: 0;
  list-style: none;
  border-right: 1px solid rgba(170, 170, 170, 0.753);
}
.active{
    border: 2px solid rgba(106, 228, 106, 0.795)
}
</style>