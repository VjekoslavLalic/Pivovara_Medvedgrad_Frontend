<template>
  <div class="PivovareCard">
    <div class="cardPivovare">
      <div class="infoCardPivovare">
        <h1>{{ info.naziv }}</h1>
        <div class="infoPivovare">
          <p>Adresa: {{ info.adresa }}</p>
          <p>Telefon: {{ info.telefon }}</p>
          <p>Radno vrijeme: {{ info.radnoVrijeme }}</p>
          <button>Više</button>
        </div>
      </div>
      <img :src="info.img" />
    </div>
  </div>
</template>
<script>
export default {
  props: ["info"],
  name: "PivniceCard",
};
</script>
<style>
.cardPivovare {
  display: flex;
  margin: 20px auto 20px auto;
  border: solid rgba(20, 17, 17, 0.64) 2px;
  padding: 0px;
  width: 700px;
}
.cardPivovare img {
  width: 380px;
  height: 156px;
  border: 3px solid rgba(20, 17, 17, 0.64);
  border-radius: 28px;
  margin-top: auto;
  margin-bottom: auto;
}
.infoCardPivovare {
  width: 38%;
  text-align: left;
  margin: 10px 5px 10px 20px;
}
.infoPivovare button {
  background-color: #390d0d;
  color: hsl(0, 0%, 72%);
  border: 2px solid rgba(20, 17, 17, 0.64);
  border-radius: 10px;
  width: 85px;
}
</style>
