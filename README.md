# RJB
第八届中国软件杯三等奖——基于深度学习的银行卡号识别
<br>项目采用两阶段法进行识别，目标检测部分复现了U-Net，卡号识别部分复现了CRNN。</br>

<h3>主程序启动方式</h3>
<br>运行:python3 demo.py</br>
<br>注意:需识别的图片集放在当前目录的img_dir文件夹下，识别结果保存至./crop/result.txt</br>
<br>目标检测的过程可视化保存在crop文件夹中，可以看到经过检测裁剪出来的银行卡区域。</br>
<br></br>
<ul>
<li>目标检测识别情况</li>
  
![Image text](https://github.com/HuiyanWen/RJB/blob/master/1.png)

<li>crnn识别情况</li>
<br>这部分识别不是特别好，有些过拟合和震荡，导致了整体精度并不是很高，两阶段准确率在70%左右。</br>

![Image text](https://github.com/HuiyanWen/RJB/blob/master/2.png)

</ul>
<h3>数据标注程序启动方式</h3>
<br>python app.py --start 运行，浏览器输入localhost:5000打开标注页面</br>
<br>标注信息存在annotation.txt中</br>
<br>倾斜框用四点式标记</br>
<br>右键标注框红色区域删除标注框，左击标注框红色区域可拖动</br>
<br>label_config.txt中可添加类别</br>
<br>图片名必须连号</br>
<br></br>
<ul>
<li>程序界面(矩形式)</li>

![Image text](https://github.com/HuiyanWen/RJB/blob/master/4.png)

<li>程序界面(四点式)</li>

![Image text](https://github.com/HuiyanWen/RJB/blob/master/5.png)

<li>label截图</li>

![Image text](https://github.com/HuiyanWen/RJB/blob/master/6.png)
</ul>
<h3>数据标注代码说明</h3>

![Image text](https://github.com/HuiyanWen/RJB/blob/master/annotation.png)

<h3>目标检测代码说明</h3>

![Image text](https://github.com/HuiyanWen/RJB/blob/master/iam.png)

<h3>CRNN代码说明</h3>

![Image text](https://github.com/HuiyanWen/RJB/blob/master/crnn.png)

<h3>参赛感言</h3>
<br>结果并不是很满意，这次比赛以教训为主吧，主要还是花的时间太少。主办方整个流程、安排和评审都比较大气、公正，选出来的确实也是各个高校的大佬。特别是一些非985、211的同学，他们身上那种不受周围环境影响，积极向上对知识的渴求，让我印象极其深刻。</br>

<br>路漫漫其修远兮 吾将上下而求索</br>
