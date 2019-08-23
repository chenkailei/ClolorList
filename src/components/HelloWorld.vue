<template>
  <div class="hello">
    <li v-for="(item, index) in ColorList"
        :key="index"
        class="item"
        :style="{'background':item.HEX}">
      {{item.name}}
    </li>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data () {
    return {
      ColorList: []
    }
  },
  mounted () {
    this.ColorList = [
      {
        name: 'LightPink',
        HEX: '#FFB6C1',
        RGB: '255,182,193'
      },
      {
        name: 'Pink',
        HEX: '#Pink',
        RGB: '255,192,203'
      },
      {
        name: 'Crimson',
        HEX: '#DC143C',
        RGB: '220,20,60'
      },
      {
        name: 'LavenderBlush',
        HEX: '#FFF0F5',
        RGB: '255,240,245'
      },
      {
        name: 'PaleVioletRed',
        HEX: '#DB7093',
        RGB: '219,112,147'
      },
      {
        name: 'HotPink',
        HEX: '#FF69B4',
        RGB: '255,105,180'
      },
      {
        name: 'DeepPink',
        HEX: '#FF1493',
        RGB: '255,20,147'
      },
      {
        name: 'MediumVioletRed',
        HEX: '#C71585',
        RGB: '199,21,133'
      },
      {
        name: 'Orchid',
        HEX: '#DA70D6',
        RGB: '218,112,214'
      },
      {
        name: 'Thistle',
        HEX: '#D8BFD8',
        RGB: '216,191,216'
      },
      {
        name: 'plum',
        HEX: '#DDA0DD',
        RGB: '221,160,221'
      },
      {
        name: 'Violet',
        HEX: '#EE82EE',
        RGB: '238,130,238'
      },
      {
        name: 'Magenta',
        HEX: '#FF00FF',
        RGB: '255,0,255'
      },
      {
        name: 'Fuchsia',
        HEX: '#FF00FF',
        RGB: '255,0,255'
      },
      {
        name: 'DarkMagenta',
        HEX: '#8B008B',
        RGB: '139,0,139'
      },
      {
        name: 'Purple',
        HEX: '#800080',
        RGB: '128,0,128'
      },
      {
        name: 'MediumOrchid',
        HEX: '#BA55D3',
        RGB: '186,85,211'
      },
    ]
  },
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
li {
  list-style: none;
}
.item {
  float: left;
  width: 150px;
  height: 150px;
  display: flex;
  align-items: center;
  justify-content: center;
}
</style>
