---
layout: wiki
title: Guide
categories: tools
description: 主页、团队、成果维护指南
keywords: Guide
---

> 终于做的差不多了

这次整理的主要是三部分 主页、团队、成果，这三部分都是用markdown维护的，只要修改对应markdown里面的内容就行

### 主页

主页的位置在 \pages\home.md, 我在主页里加了一个gallery，目前都是盗别人的图 图片的地址在 \images\slide里面，换掉就行。主页的内容有待丰满，谁有空帮忙更一下

### 团队
团队的主要信息是用YML维护的和markdown差不多，位置在 \_data\memebers.yml, 写法参照下面

``` html
- name: Doohee Cho
  photo: Doohee2.jpg
  info: Postdoc, started May 2017
  email: dooheecho80@gmail.com
  github: 3dincrement.github.io
  number_educ: 4
  education1: B.S. Yonsei University, Korea
  education2: PhD Yonsei University, Korea with <a href="http://web.yonsei.ac.kr/nano/%ED%95%99%EA%B3%BC%EC%86%8C%EA%B0%9C.htm">In-Whan Lyo</a>
  education3: Postdoc POSTECH with <a href="http://caldes.ibs.re.kr/html/caldes_en/">Han Woong Yeom</a>
  education4: Postdoc Rutgers with <a href="http://rcem.rutgers.edu/">Sang-Wook Cheong</a>
```

其中照片需要放在 images\teampic\ 里面, number_educ 不超过5。
Besides,为大家留了一个个人主页空间，在 \memeber\ 目录下建立和自己名字命名的markdown文件即可,附带留言功能， do whatever you want。

### 成果
成果目前只做了论文部分，类似于团队，成果也是用YML维护的，位置在\_data\publists.yml 里面，具体用法参考已有实例。照片最好放teaser，否则太长了。pdf、video 最好在主目录下新建file video文件夹，然后链接