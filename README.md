用于PH60 SCV2键盘的keymap改键



1、去fork原生键盘的zmk仓库[https://github.com/ph-design/ph_lite-zmk-config](https://github.com/ph-design/ph_lite-zmk-config)

  最好看着翻译选。



2、然后去自己ph_lite-zmk-config仓库内boards/shields/PH60-SC_V2/的两个文件复制到config/里面，分别是PH60-SC_V2-rgb.dtsi和PH60-SC_V2.keymap。（名字一样，内容一样）。



3、一共三个文件，还需要一个PH60-SC_V2.json，自己新建一个文件，把文件名和内容都复制放进去config/，url中的chrmevl是我用户名，使用要改成自己的。

```JSON
{
  "keyboard_name": "PH60-SC_V2",
  "url": "https://github.com/chrmevl/ph_lite-zmk-config",
  "maintainer": "PHDesign",
  "layouts": {
    "LAYOUT_ansi": {
      "layout": [
        {"label":"Esc",  "x":0,    "y":0, "w":1,   "row":0, "col":0},
        {"label":"1",    "x":1,    "y":0, "w":1,   "row":0, "col":1},
        {"label":"2",    "x":2,    "y":0, "w":1,   "row":0, "col":2},
        {"label":"3",    "x":3,    "y":0, "w":1,   "row":0, "col":3},
        {"label":"4",    "x":4,    "y":0, "w":1,   "row":0, "col":4},
        {"label":"5",    "x":5,    "y":0, "w":1,   "row":0, "col":5},
        {"label":"6",    "x":6,    "y":0, "w":1,   "row":0, "col":6},
        {"label":"7",    "x":7,    "y":0, "w":1,   "row":0, "col":7},
        {"label":"8",    "x":8,    "y":0, "w":1,   "row":0, "col":8},
        {"label":"9",    "x":9,    "y":0, "w":1,   "row":0, "col":9},
        {"label":"0",    "x":10,   "y":0, "w":1,   "row":0, "col":10},
        {"label":"-",    "x":11,   "y":0, "w":1,   "row":0, "col":11},
        {"label":"=",    "x":12,   "y":0, "w":1,   "row":0, "col":12},
        {"label":"BkSp", "x":13,   "y":0, "w":2,   "row":0, "col":13},

        {"label":"Tab",  "x":0,    "y":1, "w":1.5, "row":1, "col":0},
        {"label":"Q",    "x":1.5,  "y":1, "w":1,   "row":1, "col":1},
        {"label":"W",    "x":2.5,  "y":1, "w":1,   "row":1, "col":2},
        {"label":"E",    "x":3.5,  "y":1, "w":1,   "row":1, "col":3},
        {"label":"R",    "x":4.5,  "y":1, "w":1,   "row":1, "col":4},
        {"label":"T",    "x":5.5,  "y":1, "w":1,   "row":1, "col":5},
        {"label":"Y",    "x":6.5,  "y":1, "w":1,   "row":1, "col":6},
        {"label":"U",    "x":7.5,  "y":1, "w":1,   "row":1, "col":7},
        {"label":"I",    "x":8.5,  "y":1, "w":1,   "row":1, "col":8},
        {"label":"O",    "x":9.5,  "y":1, "w":1,   "row":1, "col":9},
        {"label":"P",    "x":10.5, "y":1, "w":1,   "row":1, "col":10},
        {"label":"[",    "x":11.5, "y":1, "w":1,   "row":1, "col":11},
        {"label":"]",    "x":12.5, "y":1, "w":1,   "row":1, "col":12},
        {"label":"\\",   "x":13.5, "y":1, "w":1.5, "row":1, "col":13},

        {"label":"Caps", "x":0,    "y":2, "w":1.75,"row":2, "col":0},
        {"label":"A",    "x":1.75, "y":2, "w":1,   "row":2, "col":1},
        {"label":"S",    "x":2.75, "y":2, "w":1,   "row":2, "col":2},
        {"label":"D",    "x":3.75, "y":2, "w":1,   "row":2, "col":3},
        {"label":"F",    "x":4.75, "y":2, "w":1,   "row":2, "col":4},
        {"label":"G",    "x":5.75, "y":2, "w":1,   "row":2, "col":5},
        {"label":"H",    "x":6.75, "y":2, "w":1,   "row":2, "col":6},
        {"label":"J",    "x":7.75, "y":2, "w":1,   "row":2, "col":7},
        {"label":"K",    "x":8.75, "y":2, "w":1,   "row":2, "col":8},
        {"label":"L",    "x":9.75, "y":2, "w":1,   "row":2, "col":9},
        {"label":";",    "x":10.75,"y":2, "w":1,   "row":2, "col":10},
        {"label":"'",    "x":11.75,"y":2, "w":1,   "row":2, "col":11},
        {"label":"Enter","x":12.75,"y":2, "w":2.25,"row":2, "col":12},

        {"label":"LShift","x":0,   "y":3, "w":2.25,"row":3, "col":0},
        {"label":"Z",    "x":2.25, "y":3, "w":1,   "row":3, "col":2},
        {"label":"X",    "x":3.25, "y":3, "w":1,   "row":3, "col":3},
        {"label":"C",    "x":4.25, "y":3, "w":1,   "row":3, "col":4},
        {"label":"V",    "x":5.25, "y":3, "w":1,   "row":3, "col":5},
        {"label":"B",    "x":6.25, "y":3, "w":1,   "row":3, "col":6},
        {"label":"N",    "x":7.25, "y":3, "w":1,   "row":3, "col":7},
        {"label":"M",    "x":8.25, "y":3, "w":1,   "row":3, "col":8},
        {"label":",",    "x":9.25, "y":3, "w":1,   "row":3, "col":9},
        {"label":".",    "x":10.25,"y":3, "w":1,   "row":3, "col":10},
        {"label":"/",    "x":11.25,"y":3, "w":1,   "row":3, "col":11},
        {"label":"RShift","x":12.25,"y":3,"w":2.75,"row":3, "col":12},

        {"label":"LCtrl","x":0,    "y":4, "w":1.25,"row":4, "col":0},
        {"label":"Win",  "x":1.25, "y":4, "w":1.25,"row":4, "col":1},
        {"label":"Alt",  "x":2.5,  "y":4, "w":1.25,"row":4, "col":2},
        {"label":"Space","x":3.75, "y":4, "w":6.25,"row":4, "col":6},
        {"label":"RAlt", "x":10,   "y":4, "w":1.25,"row":4, "col":10},
        {"label":"Fn",   "x":11.25,"y":4, "w":1.25,"row":4, "col":11},
        {"label":"GUI",  "x":12.5, "y":4, "w":1.25,"row":4, "col":12},
        {"label":"RCtrl","x":13.75,"y":4, "w":1.25,"row":4, "col":13}
      ]
    }
  }
}

```



4、去查看自己的Actions是否完成通过变绿。



5、改键[https://nickcoutsos.github.io/keymap-editor/](https://nickcoutsos.github.io/keymap-editor/)



使用：

1、保存固件[https://nickcoutsos.github.io/keymap-editor/](https://nickcoutsos.github.io/keymap-editor/)



2、会在自己的仓库里的Actions生成固件，等待变绿完成，点击最新一条，进去后到页面最下方下载firmware



3、短接两次，先刷设置文件，再刷键盘
