---
layout: post
title:  "正经点，我们来聊聊优衣库的虚拟试衣"
categories: Kinect
tags:  Kinect Unity3D
---

![]({{ site.url }}/media/uniqlo-virtual.jpg)

虚拟试衣间分三种:
- 2D 照片 + 2D 衣服
- 3D 模型 + 3D 衣服
- 真人体感




先说第一种，2D 照片+2D衣服
=
为了效果好模特都是真人照片（这不废话么……）。

左边一栏可以选衣服的种类和条目，然后 duang 得模特身上的衣服就变掉了。

是不是觉得衣服很眼熟，恩，这是优衣库官网上的。

![]({{ site.url }}/media/uniqlo-1.jpg)

但是这东西有 X 用啊！
优衣库当然知道，它还提供第二个版本

4D 试衣间
=
（请不要问我 4D 是哪 4D）。

![]({{ site.url }}/media/uniqlo-2.jpg)

好，那我们点进去看看，是一个 Unity3D 的应用，Chrome 跳出来报警说它即将放弃支持 Unity3D Player。

![]({{ site.url }}/media/uniqlo-3.jpg)

果然效果好很多，模特的身材都是可以调整的，有十多个参数，调成和你一样的就行了。这里就出现了第一个坑，你是没办法把参数调成和你一样的，人的身体不能简单得由十多个数字描述。
（这个项目和我当年在盛大创新院时候的项目很像，那会儿 Unity3D 还没流行，我们用的是鬼火引擎。）

左侧条目类似，换成了三维模型和贴图。

但是，衣服穿上去明显不对，劣质 3D 手游的感觉……算了，我们还是讨论下一种方案吧。

真人体感试衣间
=

这种方案是在商场里对着大屏幕+PC+体感设备直接进行互动，用手掌进行 UI 的交互，身体的骨骼点作为骨骼动画的关节点。

传感器选择很多，最常见的是 Kinect 一代。

![]({{ site.url }}/media/kinect-v1.jpg)


还有 Intel 最近在推的 RealSense（以下图片来自 
@英特尔中国 ，很明显，第一张图片是用来忽悠甲方的，第二张是现场情况。

![]({{ site.url }}/media/realsense-1.jpg)

这个方案的问题更严重，深度数据可不知道你的身材多棒，OpenGL 函数也不知道衣服材料棉和麻的区别。但是我们自己都知道。

![]({{ site.url }}/media/realsense-2.jpg)

这三种都介绍完了，想必大家都明白为啥优衣库还是需要试衣间的吧。

ps. 对体感设备感兴趣的可以继续阅读 市售体感设备横评：微软、Intel、苹果、LeapMotion 哪家强！ - 黑客与画家 - 知乎专栏


----
vinjn.com - Democratizing Visual Computing