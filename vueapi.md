# api

```js
Vue.config.silent = false
Vue.config.optionMergeStrategies = {}
Vue.config.devtool = {}
Vue.config.errorHandler = {}
Vue.config.ignoredElement = {}
Vue.config.keyCodes = {}
Vue.config.performance = {}
Vue.config.production = {}

// api
Vue.extend('component-name', {})
Vue.nextTick()
Vue.set(obj, key, value)
Vue.delete(obj)
Vue.directive('v-if')
Vue.filter()
Vue.component()
Vue.use('plugin')
Vue.mixin(obj)
Vue.compile()
Vue.version()

// data
new Vue({
  data: {
    someData: ""
  },
  props: {

  },
  propsData: {

  },
  computed: {

  },
  watch: {

  }
})

// dom

var vm = new Vue({
  el: "#root"
})

vm.template
vm.render
vm.renderError

// 钩子函数
create
  beforeCreate
  created
mount
  beforeMount
   mounted
updata
  beforeUpdate
  updated
activated
  deactivated
destory
  beforeDestory
  destroyed
captured
  errorCaptured
```

```js
directives
filters  // TODO: 01
components
```

```js
name
delimiters
functional
model
inheritAttrs
comments
```

```js
// instance props
vm.$data
vm.$props
vm.$el
vm.$options
vm.$parent
vm.$root
vm.$children
vm.$slots
vm.$scopedSlots
vm.$refs
vm.isServer
vm.$attr
vm.$listeners
```

```js
// instance data
vm.$watch
vm.$set
vm.$delete
```

```js
// instance event
vm.$on
vm.$once
vm.$off
vm.$emit
```

```js
// instance left_cycle
vm.$mount
vm.$forceUpdate
vm.$nextTick
vm.$destroy
```

```js

// directive
v-text
v-html
v-show
v-if
v-else
v-else-if
v-for
v-on
v-bind
v-model
v-pre
v-cloak
v-once
```

```js
// special attr
key
ref
slot
slot-scope
scope
is
```

```js
build-in components

component
transition
transition-group
keep-alive
slot
```

VNode 接口
服务端渲染

## 作用域插槽

```html
<todo-list>
  <template slot-scope="slotProps">
    <span v-if="slotProps.todo.isComplete">
      ✅
    </span>
    {{ slotProps.todo.text R}}
  </template>
</todo-list>
```