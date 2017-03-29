## 说明
    最近做App对安全要求较高，所以iOS的代码必须要有混淆的措施，初期实施了念茜姐的混淆方案，但是领导说，我们要自动混淆，方法名字不能一个一个的添加到func.list中，所以方法名只能从.m和.h文件中抽取了，但是如何屏蔽系统的方法名，暂行的策略是:将自己定义的方法名全部添加一个前缀。

##  例如 “hsk_funtion1”； “hsk_funtion2”；“hsk_funtion3”；
<img src="https://github.com/AidyBao/BMQConfuse/blob/master/Resoure/1.png" width=200px height=300px></img>

## 通过class-dump 反编译之后：Appdelegate 效果
<img src="https://github.com/AidyBao/BMQConfuse/blob/master/Resoure/2.png" width=200px height=300px></img>

## 通过class-dump 反编译之后：ViewController 效果
<img src="https://github.com/AidyBao/BMQConfuse/blob/master/Resoure/3.png" width=200px height=300px></img>

