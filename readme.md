# vue-chat-scroll

Forked from [sj82516/vue-chat-scroll-top-load](https://github.com/sj82516/vue-chat-scroll-top-load)

## Installation

- #### NPM
  Run `npm i --save IlyaVorozhbit/vue-chat-scroll#master`

- #### With Modules

  ``` js
  // ES6
  import Vue from 'vue'
  import VueChatScroll from 'vue-chat-scroll'
  Vue.use(VueChatScroll)

  // ES5
  var Vue = require('vue')
  Vue.use(require('vue-chat-scroll'))
  ```

- #### `<script>` Include

  Just include `./dist/vue-chat-scroll.js` after Vue itself.

## Usage

There's nothing you need to do in JavaScript except for installation. To use the plugin, simply use the `v-chat-scroll` directive.

``` html
<ul class="messages" v-chat-scroll @scroll-top="loadNewData()">
  <li class="message" v-for="n in messages">{{ n }}</li>
</ul>
```

#### Prevent scroll down when user has scrolled up & smooth scrolling

Alternatively, you can pass a config value to the directive:

``` html
<ul class="messages" v-chat-scroll="{always: false, smooth: true}">
  <li class="message" v-for="n in messages">{{ n }}</li>
</ul>
```

## License

[MIT](http://opensource.org/licenses/MIT)
