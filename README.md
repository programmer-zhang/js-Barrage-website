# -web-
需求分析
   用户点击发送按钮 把input的内容展示到box里面
   1.元素 .con .send-btn .box span（创建）
   2.事件：点击事件 键盘事件
   3.行为
       1.点击.send-btn获取.con的内容
           (1)规范发送信息
           (2)禁止空及全空格
           (3)存储value值
       2.根据内容动态生成span标签
           (1)创建节点document.createElement
           (2)改变节点内容innerHTML
           (3)节点 生成初始化位置等
           (4)标签添加到oBox appendChild
       3.message运动
           (1)改变元素的left值
           (2)定时器改变 setInterval
           (3)this代表当前弹幕
           (4)弹幕left = 当前left-1
       4.随机函数
           Math.random 0-1 包括0但不包括1
           (1)top
           (2)color
           (3)fontsize
           (4)textShadow
           (5)timing运动曲线
               linear
               ease-out
       5.业务完善
           (1)过去的删除掉
               停止计时器
               删除自身
               终止函数
           (2)完善回车输入
               在oCon上回车 发送弹幕
