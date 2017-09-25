### vue-js-grid

Fixed size grid for Vue.js

### Install
```
npm install --save vue-js-grid
```

```js
import Vue from 'vue'
import Grid from 'vue-js-grid'

Vue.use(Grid)
```

### Usage

```js
data () {
  return {
    items: [
      'a', 
      'b', 
      'c'
    ]
}
```

```vue
<grid
  :draggable="true"
  :sortable="true"
  :items="items"
  :height="100"
  :width="100">
  <template slot="cell" scope="props">
    <div>{{props.item.value}}</div>
  </template>
</grid>
```

### Props

| Name       | Type     | Default   | Description       |
| ---        | ---      | ---       | ---               |
| items      | [Object] | []        | |
| cellWidth  | Number   | 80        | |
| cellHeight | Number   | 80        | |
| draggable  | Boolean  | false     | |
| dragDelay  | Number   | 0         | @TODO |
| sortable   | Boolean  | false     | |
| center     | Boolean  | false     | @TODO |

### Events

| Name    | Description |
| ---     | ---         |
| @change | |
| @remove | |
| @click  | |
| @sort   | |

### Item template




### Roadmap

1. Add element insertion
2. Add tests
