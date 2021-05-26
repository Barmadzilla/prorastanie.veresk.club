<template>
  <div class="content">
    <div class="first"></div>
    <div class="text">
      <p>Эко-парк «Вереск» совместно с куратором Лизой Савиной открывает локальную арт-резиденцию, где художники смогут работать и создавать проекты, вдохновленные местной
        природой и историей.
      </p>
      <p>Этим летом на территории эко-парка развернется наш первый проект — «Прорастание». Названием проекта мы обязаны нашим первым резидентам — Валерию и Юлии Казасам. Такое
        название появилось неслучайно: как в первые теплые дни прорастают травы, первоцветы и распускаются листья на деревьях, так и наши мысли, восприятие и эмоции
        раскрываются под воздействием природы и искусства.</p>
    </div>
    <div><img src="../assets/images/photos/6-sklad-2.jpg" alt=""></div>
    <div class="text">
      <p>Основная экспозиция будет расположена под открытым небом, а арт-объекты выполнены художниками из разных городов и стран. Объединит их близость и бережное отношение к
        природе и цель — создать новые акценты в привычном ландшафте, сместить точку зрения зрителя, пригласить остановиться и задуматься о важном и вечном.</p>
      <p>Проект будет развиваться эволюционным путем, и никто не может точно предположить, каким он станет через несколько месяцев. Но именно в этом — его основная идея: важен
        путь, а не конечная точка. </p>
    </div>
    <div>
      <img src="../assets/images/photos/4-cilynder-2.jpg" alt="">
    </div>
    <div class="second"></div>
    <div class="full text">
      <p>Прогуливаясь вдоль берега лесного озера, вы обнаружите валуны, выкрашенные яркой краской, длинной дорожкой уходящие в воду. Или бирюзовые ветви когда-то погибших
        сухих деревьев, впивающиеся в пространство между камней. Это работы Валерия и Юлии Казас — известных в России и за рубежом художников из Краснодара, наиболее
        последовательно работающих с ленд-артом. Они неразрывно связывают свои произведения с окружающим природным ландшафтом, расставляя акценты за счет комбинации цветов и
        текстур.
        В эко-парке «Вереск» художники создали 13 скульптур, выполненных из природных материалов и интегрированных в естественную среду.</p>
      <p>Мы подготовили карту, чтоб каждый гость эко-парка смог найти все арт-объекты и составить новый маршрут по знакомым местам, следуя за взглядом и мыслями
        художников.</p>
    </div>
    <div class="text">
      <h2>Валерий и Юлия Казас</h2>
      <p>Валерий Казас родился в 1965 году в Краснодаре. В 1989 году закончил Краснодарский Политехнический институт. С 1996 года профессионально занимается скульптурой, в
        этом же году состоялась его первая выставка. Казас - один из наиболее последовательных адептов и популяризаторов скульптурного минимализма, и оттолкнувшегося от него
        ленд-арта. Для Казаса путь к минимализму опирается на из два слагаемых. Во-первых отрицание внешнего контекста: заполонившей города плохой бронзы. Во-вторых любовь к
        традиционной японской скульптуре, где за фигуративностью прячется полуабстрактная философская максима, а за обильным декором скрывается пристальное внимание к
        материалу: текстуре, фактуре, цвету. Скульптуры и инсталляции Валерия Казаса вы можете встретить в его родном Краснодаре, в Москве, Перми, Алматы, Черногории, США.
        Интерес к минималистической скульптуре предсказуемо привел его в ленд-арту, сначала в форме художественных интервенций, а в 2018 году Казас выиграл грант Gelnmorangie
        Signet Land Art в Музее современного искусства «Гараж», результатом которого стала огромная инсталляция в московском Парке Горького. В 2020 году Казас стал участником
        проекта Nemoskva с серией макетов музеев современного искусства.
        Художественная карьера Юлии Казас значительно короче, зато она сразу началась с участия в спецпроекте Московской биеннале современного искусства в 2015 году. Интересы
        Юлии лежат в сфере deep media - исследовании свойств различных материалов материалов и формами их трансформации.
      </p>
      <p>
        Валерий Казас - художник, для которого важнее состояние, ощущение, переживание визуального через аскетичную форму. Юлия Казас - опирается на концепцию.
        Их тандем в проекте «Прорастание» - плодотворный союз взаимодополняющих друг друга творческих единиц.
      </p>
    </div>
    <div class="kazas"></div>
    <div class="full">
      <div id="map"></div>
      <div class="contact">
        <img src="../assets/images/logos/logo-veresk-gray.svg">
        <div>
          <h3><a tel="+7 (812) 407-33-01">+7 (812) 407-33-01</a></h3>
          <p><a href="https://veresk.club">veresk.club</a></p>
        </div>
      </div>
    </div>
    <div class="full no-bg">
      <Gallery></Gallery>
    </div>
  </div>
</template>
<script>

import Gallery from "@/components/Gallery";
export default {
  name: "Content",
  components: {Gallery},
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
  background: url("../assets/images/photos/2-red-line-2.jpg") center / cover no-repeat;
  display: flex;
}

div.kazas {
  background: url("../assets/images/photos/kazaas.jpg") center / cover no-repeat;
}

div.second {
  grid-column-start: 2;
  grid-column-end: 2;
  grid-row-start: 3;
  grid-row-end: span 2;
  background: url("../assets/images/photos/3-prorastanie-1.jpg") center / cover no-repeat;
  /*display: flex;*/
}

div.full {
  grid-column: span 2;
  position: relative;
}

.text {
  padding: 20px;
}

.text h2 {
  font-size: 2em;
  margin-bottom: 1em;
}

#map {
  margin: var(--radius);
  height: 440px;
  position: relative;
}
.content .full.no-bg div,
.content .full.no-bg {
  background: unset;
}
div.full .contact {
  --margin: 20px;
  position: absolute;
  z-index: 9999;
  left: 0;
  top: 0;
  height: calc(100% - var(--margin) * 2);
  width: 38%;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  align-items: center;
  box-sizing: border-box;
  margin: var(--margin);
  padding: calc(var(--margin) + 20px ) ;
  border-radius: unset;
  background: rgba(255, 255, 255, 0.5);
  -webkit-backdrop-filter: blur(10px);
}

div.full .contact * {
  border-radius: unset;
  text-align: center;
  background: unset ;
}

div.full .contact h3 {
  font-weight: normal;
  font-size: 2em;
}
div.full .contact a{
  font-weight: 300;
  color: gray;
  text-decoration: none;
}

#map > ymaps {
  border-radius: 20px;
  overflow: hidden;
}

@media (max-width: 800px) {
  .content {
    grid-template-columns: 3fr 3fr;
  }
}

@media (max-width: 420px) {
  .content {
    grid-template-columns: 1fr;
  }

  div.first {
    grid-column-start: 1;
    grid-column-end: 1;
    grid-row-start: 1;
    grid-row-end: 1;
    height: 50vh;
  }

  div.second {
    grid-column-start: 1;
    grid-column-end: 1;
    grid-row-start: 7;
    grid-row-end: 7;
    height: 30vh;
  }
  div.kazas{
    height: 30vh;
  }
  div.full .contact{
    box-sizing: border-box;
    padding: 2em;
    background: none;
    width: calc(100% - 2em);
    position: relative;
  }
  div.full .contact img{
    width: 100%;
    margin: 0;
  }
  div.full .contact{
    font-size: 15px;
  }

  div.full {
    grid-column: unset;
  }
  #map{
    height: 50vh;
  }
}
</style>