<template>
    <div id="test"><a href="https://www.digistore24.com/product/238289" class="wuButton">Jetzt bestellen</a></div>
</template>

<script>
export default {
  name: "wu_button"
};
</script>

<style scoped>
.wuButton {
  z-index: 100;
  width: 30%;
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
  text-shadow: 0px 1px 0px #5b8a3c;
}
.wuButton:hover {
  background: linear-gradient(to bottom, #ffcc00 5%, #ffdd54 100%);
  filter: progid:DXImageTransform.Microsoft.gradient(startColorstr='#72b352', endColorstr='#77b55a',GradientType=0);
  background-color: #72b352;
}

#test {
  position: sticky;
  top: 10px;
}
</style>