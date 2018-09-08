<template>
    <a href="https://www.digistore24.com/product/238289" class="wuButton">Jetzt anfangen! | 14,99€</a>
</template>

<script>
export default {
  name: "wu_button"
};
</script>

<style scoped>
.wuButton {
  /* z-index: 100;
  white-space: nowrap;
  box-shadow: 0px 10px 14px -7px #3e7327;
  background: linear-gradient(to bottom, #ffdd54 5%, #ffcc00 100%);
  filter: progid:DXImageTransform.Microsoft.gradient(startColorstr='#77b55a', endColorstr='#72b352',GradientType=0);
  background-color: #ffcc00;
  border-radius: 4px;
  border: 1px solid #4b8f29;
  cursor: pointer;
  color: rgba(17, 17, 17, 0.8);
  font-weight: bold;
  padding: 0.5em 2em;
  text-decoration: none;
  text-shadow: 0px 1px 0px #5b8a3c; */
  margin: 1em;
  white-space: nowrap;
  display: inline-block;
  height: 40px;
  line-height: 40px;
  padding: 0 14px;
  box-shadow: 0 4px 6px rgba(50, 50, 93, 0.11), 0 1px 3px rgba(0, 0, 0, 0.08);
  background: #ffcc00;
  border-radius: 4px;
  font-size: 15px;
  font-weight: 600;
  text-transform: uppercase;
  letter-spacing: 0.025em;
  color: #111;
  text-decoration: none;
  -webkit-transition: all 0.15s ease;
  transition: all 0.15s ease;
}
.wuButton:hover {
  /* background: linear-gradient(to bottom, #ffcc00 5%, #ffdd54 100%);
  filter: progid:DXImageTransform.Microsoft.gradient(startColorstr='#72b352', endColorstr='#77b55a',GradientType=0);
  background-color: #72b352; */
  background: #ffe066;
  transform: translateY(-1px);
  box-shadow: 0 7px 14px rgba(50, 50, 93, 0.1), 0 3px 6px rgba(0, 0, 0, 0.08);
}
</style>