<template>
  <div class="hello">
    <Tooltip :style="{'background':item.HEX}"
             class="item"
             v-for="(item, index) in ColorList"
             :key="index"
             :content="'HEX:' + '\xa0\xa0\xa0' + item.HEX + '\xa0\xa0\xa0RGB:\xa0\xa0\xa0' + item.RGB"
             placement="top">
      <li class="children">
        {{item.name}}
      </li>
    </Tooltip>

    <div class="bottom">Contact us: ckl5975@126.com</div>
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
        HEX: '#FFC0CB',
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
      {
        name: 'DarkVoilet',
        HEX: '#9400D3',
        RGB: '148,0,211'
      },
      {
        name: 'DarkOrchid',
        HEX: '#9932CC',
        RGB: '153,50,204'
      },
      {
        name: 'Indigo',
        HEX: '#4B0082',
        RGB: '75,0,130'
      },
      {
        name: 'BlueViolet',
        HEX: '#8A2BE2',
        RGB: '138,43,226'
      },
      {
        name: 'MediumPurple',
        HEX: '#9370DB',
        RGB: '147,112,219'
      },
      {
        name: 'MediumSlateBlue',
        HEX: '#7B68EE',
        RGB: '123,104,238'
      },
      {
        name: 'SlateBlue',
        HEX: '#6A5ACD',
        RGB: '106,90,205'
      },
      {
        name: 'DarkSlateBlue',
        HEX: '#483D8B',
        RGB: '72,61,139'
      },
      {
        name: 'Lavender',
        HEX: '#E6E6FA',
        RGB: '230,230,250'
      },
      {
        name: 'GhostWhite',
        HEX: '#F8F8FF',
        RGB: '248,248,255'
      },
      {
        name: 'Blue',
        HEX: '#0000FF',
        RGB: '0,0,255'
      },
      {
        name: 'MediumBlue',
        HEX: '#0000CD',
        RGB: '0,0,205'
      },
      {
        name: 'MidnightBlue',
        HEX: '#191970',
        RGB: '25,25,112'
      },
      {
        name: 'DarkBlue',
        HEX: '#00008B',
        RGB: '0,0,139'
      },
      {
        name: 'Navy',
        HEX: '#000080',
        RGB: '0,0,128'
      },
      {
        name: 'RoyalBlue',
        HEX: '#4169E1',
        RGB: '65,105,225'
      },
      {
        name: 'CornflowerBlue',
        HEX: '#6495ED',
        RGB: '100,149,237'
      },
      {
        name: 'LightSteelBlue',
        HEX: '#B0C4DE',
        RGB: '176,196,222'
      },
      {
        name: 'LightSlateGray',
        HEX: '#778899',
        RGB: '119,136,153'
      },
      {
        name: 'SlateGray',
        HEX: '#708090',
        RGB: '112,128,144'
      },
      {
        name: 'DodgerBlue',
        HEX: '#1E90FF',
        RGB: '30,144,255'
      },
      {
        name: 'AliceBlue',
        HEX: '#F0F8FF',
        RGB: '240,248,255'
      },
      {
        name: 'SteelBlue',
        HEX: '#4682B4',
        RGB: '70,130,180'
      },
      {
        name: 'LightSkyBlue',
        HEX: '#87CEFA',
        RGB: '135,206,250'
      },
      {
        name: 'SkyBlue',
        HEX: '#87CEEB',
        RGB: '135,206,235'
      },
      {
        name: 'DeepSkyBlue',
        HEX: '#00BFFF',
        RGB: '0,191,255'
      },
      {
        name: 'LightBLue',
        HEX: '#ADD8E6',
        RGB: '173,216,230'
      },
      {
        name: 'PowDerBlue',
        HEX: '#B0E0E6',
        RGB: '176,224,230'
      },
      {
        name: 'CadetBlue',
        HEX: '#5F9EA0',
        RGB: '95,158,160'
      },
      {
        name: 'Azure',
        HEX: '#F0FFFF',
        RGB: '240,255,255'
      },
      {
        name: 'LightCyan',
        HEX: '#E1FFFF',
        RGB: '225,255,255'
      },
      {
        name: 'PaleTurquoise',
        HEX: '#AFEEEE',
        RGB: '175,238,238'
      },
      {
        name: 'Cyan',
        HEX: '#00FFFF',
        RGB: '0,255,255'
      },
      {
        name: 'Aqua',
        HEX: '#00FFFF',
        RGB: '0,255,255'
      },
      {
        name: 'DarkTurquoise',
        HEX: '#00CED1',
        RGB: '0,206,209'
      },
      {
        name: 'DarkSlateGray',
        HEX: '#2F4F4F',
        RGB: '47,79,79'
      },
      {
        name: 'DarkCyan',
        HEX: '#008B8B',
        RGB: '0,139,139'
      },
      {
        name: 'Teal',
        HEX: '#008080',
        RGB: '0,128,128'
      },
      {
        name: 'MediumTurquoise',
        HEX: '#48D1CC',
        RGB: '72,209,204'
      },
      {
        name: 'LightSeaGreen',
        HEX: '#20B2AA',
        RGB: '32,178,170'
      },
      {
        name: 'Turquoise',
        HEX: '#40E0D0',
        RGB: '64,224,208'
      },
      {
        name: 'BabyGreen',
        HEX: '#7FFFAA',
        RGB: '127,255,170'
      },
      {
        name: 'MediumAquamarine',
        HEX: '#00FA9A',
        RGB: '0,250,154'
      },
      {
        name: 'MediumSpringGreen',
        HEX: '#F5FFFA',
        RGB: '245,255,250'
      },
      {
        name: 'MintCream',
        HEX: '#00FF7F',
        RGB: '0,255,127'
      },
      {
        name: 'SpringGreen',
        HEX: '#3CB371',
        RGB: '60,179,113'
      },
      {
        name: 'SeaGreen',
        HEX: '#2E8B57',
        RGB: '46,139,87'
      },
      {
        name: 'Honeydew',
        HEX: '#F0FFF0',
        RGB: '240,255,0'
      },
      {
        name: 'LightGreen',
        HEX: '#90EE90',
        RGB: '144,238,144'
      },
      {
        name: 'PaleGreen',
        HEX: '#98FB98',
        RGB: '152,251,152'
      },
      {
        name: 'DarkSeaGreen',
        HEX: '#8FBC8F',
        RGB: '143,188,143'
      },
      {
        name: 'LimeGreen',
        HEX: '#32CD32',
        RGB: '50,205,50'
      },
      {
        name: 'Lime',
        HEX: '##00FF00',
        RGB: '0,255,0'
      },
      {
        name: 'ForestGreen',
        HEX: '#228B22',
        RGB: '34,139,34'
      },
      {
        name: 'Green',
        HEX: '#008000',
        RGB: '0,128,0'
      },
      {
        name: 'DarkGreen',
        HEX: '#006400',
        RGB: '0,100,0'
      },
      {
        name: 'Chartreuse',
        HEX: '#7FFF00',
        RGB: '127,255,0'
      },
      {
        name: 'LawnGreen',
        HEX: '#7CFC00',
        RGB: '124,252,0'
      },
      {
        name: 'GreenYellow',
        HEX: '#ADFF2F',
        RGB: '173,255,47'
      },
      {
        name: 'OliveDrab',
        HEX: '#556B2F',
        RGB: '85,107,47'
      },
      {
        name: 'Beige',
        HEX: '#6B8E23',
        RGB: '107,142,35'
      },
      {
        name: 'LightGoldenrodYellow',
        HEX: '#FAFAD2',
        RGB: '250,250,210'
      },
      {
        name: 'Ivory',
        HEX: '#FFFFF0',
        RGB: '255,255,240'
      },
      {
        name: 'LightYellow',
        HEX: '#FFFFE0',
        RGB: '255,255,224'
      },
      {
        name: 'Yellow',
        HEX: '#FFFF00',
        RGB: '255,255,0'
      },
      {
        name: 'Olive',
        HEX: '#808000',
        RGB: '128,128,0'
      },
      {
        name: 'DarkKhaki',
        HEX: '#BDB76B',
        RGB: '189,183,107'
      },
      {
        name: 'LemonChiffon',
        HEX: '#FFFACD',
        RGB: '255,250,205'
      },
      {
        name: 'PaleGodenrod',
        HEX: '#EEE8AA',
        RGB: '238,232,170'
      },
      {
        name: 'Khaki',
        HEX: '#F0E68C',
        RGB: '240,230,140'
      },
      {
        name: 'Gold',
        HEX: '#FFD700',
        RGB: '255,215,0'
      },
      {
        name: 'Cornislk',
        HEX: '#FFF8DC',
        RGB: '255,248,220'
      },
      {
        name: 'GoldEnrod',
        HEX: '#DAA520',
        RGB: '218,165,32'
      },
      {
        name: 'FloralWhite',
        HEX: '#FFFAF0',
        RGB: '255,250,240'
      },
      {
        name: 'OldLace',
        HEX: '#FDF5E6',
        RGB: '253,245,230'
      },
      {
        name: 'Wheat',
        HEX: '#F5DEB3',
        RGB: '245,222,179'
      },
      {
        name: 'Moccasin',
        HEX: '#FFE4B5',
        RGB: '255,228,181'
      },
      {
        name: 'Orange',
        HEX: '#FFA500',
        RGB: '255,165,0'
      },
      {
        name: 'PapayaWhip',
        HEX: '#FFEFD5',
        RGB: '255,239,213'
      },
      {
        name: 'BlanchedAlmond',
        HEX: '#FFEBCD',
        RGB: '255,235,205'
      },
      {
        name: 'NavajoWhite',
        HEX: '#FFDEAD',
        RGB: '255,222,173'
      },
      {
        name: 'AntiqueWhite',
        HEX: '#FAEBD7',
        RGB: '250,235,215'
      },
      {
        name: 'Tan',
        HEX: '#D2B48C',
        RGB: '210,180,140'
      },
      {
        name: 'BrulyWood',
        HEX: '#DEB887',
        RGB: '222,184,135'
      },
      {
        name: 'Bisque',
        HEX: '#FFE4C4',
        RGB: '255,228,196'
      },
      {
        name: 'DarkOrange',
        HEX: '#FF8C00',
        RGB: '255,140,0'
      },
      {
        name: 'Linen',
        HEX: '#FAF0E6',
        RGB: '250,240,230'
      },
      {
        name: 'Peru',
        HEX: '#CD853F',
        RGB: '205,133,63'
      },
      {
        name: 'PeachPuff',
        HEX: '#FFDAB9',
        RGB: '255,218,185'
      },
      {
        name: 'SandyBrown',
        HEX: '#F4A460',
        RGB: '244,164,96'
      },
      {
        name: 'Chocolate',
        HEX: '#D2691E',
        RGB: '210,105,30'
      },
      {
        name: 'SaddleBrown',
        HEX: '#8B4513',
        RGB: '139,69,19'
      },
      {
        name: 'SeaShell',
        HEX: '#FFF5EE',
        RGB: '255,245,238'
      },
      {
        name: 'Sienna',
        HEX: '#A0522D',
        RGB: '160,82,45'
      },
      {
        name: 'LightSalmon',
        HEX: '#FFA07A',
        RGB: '255,160,122'
      },
      {
        name: 'Coral',
        HEX: '#FF7F50',
        RGB: '255,127,80'
      },
      {
        name: 'OrangeRed',
        HEX: '#FF4500',
        RGB: '255,69,0'
      },
      {
        name: 'DarkSalmon',
        HEX: '#E9967A',
        RGB: '233,150,122'
      },
      {
        name: 'Tomato',
        HEX: '#FF6347',
        RGB: '255,99,71'
      },
      {
        name: 'MistyRose',
        HEX: '#FFE4E1',
        RGB: '255,228,225'
      },
      {
        name: 'Salmon',
        HEX: '#FA8072',
        RGB: '250,128,114'
      },
      {
        name: 'Snow',
        HEX: '#FFFAFA',
        RGB: '255,250,250'
      },
      {
        name: 'LightCoral',
        HEX: '#F08080',
        RGB: '240,128,128'
      },
      {
        name: 'RosyBrown',
        HEX: '#BC8F8F',
        RGB: '188,143,143'
      },
      {
        name: 'IndianRed',
        HEX: '#CD5C5C',
        RGB: '205,92,92'
      },
      {
        name: 'Red',
        HEX: '#FF0000',
        RGB: '255,0,0'
      },
      {
        name: 'Brown',
        HEX: '#A52A2A',
        RGB: '165,42,42'
      },
      {
        name: 'FireBrick',
        HEX: '#B22222',
        RGB: '178,34,34'
      },
      {
        name: 'DarkRed',
        HEX: '#8B0000',
        RGB: '139,0,0'
      },
      {
        name: 'Maroon',
        HEX: '#800000',
        RGB: '128,0,0'
      },
      {
        name: 'White',
        HEX: '#FFFFFF',
        RGB: '255,255,255'
      },
      {
        name: 'WhiteSmoke',
        HEX: '#F5F5F5',
        RGB: '245,245,245'
      },
      {
        name: 'Gainsboro',
        HEX: '#DCDCDC',
        RGB: '220,220,220'
      },
      {
        name: 'LightGray',
        HEX: '#D3D3D3',
        RGB: '211,211,211'
      },
      {
        name: 'Silver',
        HEX: '#C0C0C0',
        RGB: '192,192,192'
      },
      {
        name: 'DarkGray',
        HEX: '#A9A9A9',
        RGB: '169,169,169'
      },
      {
        name: 'Gray',
        HEX: '#808080',
        RGB: '128,128,128'
      },
      {
        name: 'DimGray',
        HEX: '#696969',
        RGB: '105,105,105'
      },
      {
        name: 'Black',
        HEX: '#000000',
        RGB: '0,0,0'
      }
    ]
  },
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
/* 淘宝初始化样式 */
body,
html {
  width: 100%;
  height: 100%;
}

body,
li {
  margin: 0;
  padding: 0;
}
.hello {
  padding: 20px 15px;
}
li {
  list-style: none;
}
.item {
  float: left;
  width: 150px;
  height: 150px;
  margin: 3px;
  white-space: pre-line;
}
.children {
  width: 100%;
  height: 150px;
  display: flex;
  align-items: center;
  justify-content: center;
  font-size: 16px;
  font-weight: bold;
}
.bottom {
  background: #fff;
  font-size: 14px;
  text-align: center;
}
</style>
