# tween
原生JS实现一个tween动画库

## 使用方法

引入tween.js

Animate(curEle, target, duration, effect, callBack)

curEle->当前要操作运动的元素

target->当前动画的目标位置,存储的是每一个方向的目标位置{left:xxx,top:xxx,...}

duration->当前动画的总时间

effect支持以下的情况

1. 如果传递进来的是一个数字：0->Linear 1->Circ-easeInOut 2->Elastic-easeOut 3->Back-easeOut 4->Bounce-easeOut 5->Expo-easeIn

2. 如果传递进来的是一个数组：move(curEle, target, duration,["Elastic","easeOut"]) ->Effect.Elastic.easeOut
3. 如果不传递的话,默认就使用Effect.Linear匀速效果