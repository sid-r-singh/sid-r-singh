import Vue from "vue";
import App from "./App.vue";
import TypeIt from "typeit";
[codesandbox](https://codesandbox.io/s/readme-introgif-9fjo5)
Vue.config.productionTip = false;

new Vue({
  render: h => h(App)
}).$mount("#app");

new TypeIt("#inner-demo-2", {
  speed: 100,
  lifelike: true,
  cursor: true,
  cursorSpeed: 300,
  loop: true
})
  .pause(1000)
  .type('<span style="font-family: Segoe UI Emoji">👋</span>', {
    html: true
  })
  .type("&nbspHi&nbspthere!&nbspI'm&nbspSidharth&nbspR")
  .pause(750)
  .delete(7, { deleteSpeed: 150 })
  .pause(500)
  .type("rana.dev")
  .pause(500)
  .move(-10)
  .delete(1)
  .type("s")
  .move(-1)
  .type("https://")
  .move(8)
  .delete(1)
  .type(".")
  .move("END")
  .pause(1000)
  .go();
