# swing-demo

> 这是使用 java swing 写的一个练手小游戏

> 主要 用到的技术有:

     java swing 
     java io
     java 多线程
     java 集合
     
 > 实现原理:
   
   在Jpanel绘制坦克 进行事件监听
   
   绘制敌人的坦克 并将其假如vector(为什么是vector 因为每个坦克是一个线程，vector是线程安全)
   
   绘制自己的坦克 并设置不一样的颜色
   
   敌方坦克移动时 采用的是random 改变方向后移动
   
   自己的坦克是采用事件监听的方式进行移动
   
   坦克的灭亡都是采用轮询的方式 将敌方发射的子弹加入vector 然后不断获取子弹的位置是否和自己坦克的位置重叠，一旦发生重叠，则销毁坦克
