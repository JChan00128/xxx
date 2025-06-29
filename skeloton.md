## 抽象layout

总计九个card

1. header （3种header）
    - 左右布局
    - 右边（两个小点/一个小点）
    - 坐标（一个长线/两个短线/一个短线）
2. bar
    - bar1 长方块
    - bar2 有一个底部的边框，有一条长线，有一条短线
    - bar3 四个小方块
3. list
    - item1 一条短线，两条长线，底部有边框
    - item2  
        - 一个checkbox小点，一个短线，两条长线
        - 一个checkbox小点，一个左右布局的短线，一条长线
    - item3
        - 左右布局(右边方块会有两种布局，左边方块一种布局)
        - 第一条线（有长有短）
        - 第二条线
4. footer

### card 1 (all)
```json

{
    header:{
        left:`long` // long,2short
        right:[1,2]
    },
    bar:{
        type:"1",//1,2,3
    },
    list:[{
        type:"1",// 1,2,3
        line:["short","line","line"]
    },{
        type:"1",// 1,2,3
        line:["long","line","line"]
    },{
        type:"1",// 1,2,3
        line:["short","line","line"]
    }]


    list2:[{
        type:"2",// 1,2,3
        line:["short","line","line"]
    },{
        type:"1",// 1,2,3
        line:["long-point","line","line"]
    }]

     list3:[{
        type:"3",// 1,2,3
        class:"a",
        line:["short","line","line"]
    },{
        type:"1",// 1,2,3
        line:["long-point","line","line"]
    }]

}
    


