<template>
  <div class="content">
    <div class="first"></div>
    <div class="text">
      <p>Эко-парк «Вереск» совместно с куратором Лизой Савиной открывает локальную арт-резиденцию, где художники смогут работать и создавать проекты, вдохновленные местной природой и историей.
      </p>
      <p>Этим летом на территории эко-парка развернется наш первый проект — «Прорастание». Названием проекта мы обязаны нашим первым резидентам — Валерию и Юлии Казасам. Такое название появилось неслучайно: как в первые теплые дни прорастают травы, первоцветы и распускаются листья на деревьях, так и наши мысли, восприятие и эмоции раскрываются под воздействием природы и искусства.</p>
    </div>
    <div><img src="../assets/images/photos/art_2.jpg" alt=""></div>
    <div class="text">
      <p>Основная экспозиция будет расположена под открытым небом, а арт-объекты выполнены художниками из разных городов и стран. Объединит их близость и бережное отношение к природе и цель — создать новые акценты в привычном ландшафте, сместить точку зрения зрителя, пригласить остановиться и задуматься о важном и вечном.</p>
      <p>Проект будет развиваться эволюционным путем, и никто не может точно предположить, каким он станет через несколько месяцев. Но именно в этом — его основная идея: важен путь, а не конечная точка. </p>
    </div>
    <div>
      <img src="../assets/images/photos/art_3.jpg" alt="">
    </div>
    <div class="second"></div>
    <div class="full text">
      <p>Прогуливаясь вдоль берега лесного озера, вы обнаружите валуны, выкрашенные яркой краской, длинной дорожкой уходящие в воду. Или бирюзовые ветви когда-то погибших сухих деревьев, впивающиеся в пространство между камней. Это работы Валерия и Юлии Казас — известных в России и за рубежом художников из Краснодара, наиболее последовательно работающих с ленд-артом. Они неразрывно связывают свои произведения с окружающим природным ландшафтом, расставляя акценты за счет комбинации цветов и текстур.
        В эко-парке «Вереск» художники создали 13 скульптур, выполненных из природных материалов и интегрированных в естественную среду.</p>
      <p>Мы подготовили карту, чтоб каждый гость эко-парка смог найти все арт-объекты и составить новый маршрут по знакомым местам, следуя за взглядом и мыслями художников.</p>
    </div>
  </div>
</template>
<script>
export default {
  name: "Content"
}
</script>

<style scoped>
.content {
  display: grid;
  grid-gap: var(--gap);
  grid-template-columns: 4fr 3fr;
  justify-items: stretch;
}

.content div {
  border-radius: var(--radius);
  background: #f6f6f6;
  overflow: hidden;
  /*object-fit: cover;*/
}

.content div img {
  width: 100%;
  display: flex;
  object-fit: scale-down;
  object-position: center;
}

div.first {
  grid-column-start: 1;
  grid-column-end: 1;
  grid-row-start: 1;
  grid-row-end: span 2;
  background: url("../assets/images/photos/art_1.jpg") center / cover no-repeat;
  display: flex;
}

div.second {
  grid-column-start: 2;
  grid-column-end: 2;
  grid-row-start: 3;
  grid-row-end: span 2;
  background: url("../assets/images/photos/art_4.jpg") center / cover no-repeat;
  /*display: flex;*/
}

div.full {
  grid-column: span 2;
}

.text {
  padding: 20px;
}

@media (max-width: 800px) {
  .content{
    grid-template-columns: 3fr 3fr;
  }
}
@media (max-width: 420px) {
  .content{
    grid-template-columns: 1fr;
  }
  div.first{
    grid-column-start: 1;
    grid-column-end: 1;
    grid-row-start: 1;
    grid-row-end: 1;
    height: 50vh;
  }
  div.second{
    grid-column-start: 1;
    grid-column-end: 1;
    grid-row-start: 7;
    grid-row-end: 7;
    height: 30vh;
  }
  div.full {
    grid-column: unset;
  }
}
</style>