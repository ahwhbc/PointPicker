## [软件] PointPicker 选取模型上的点并保存

最近想拾取一个模型上的点的坐标并保存下来，首先用了meshlab软件，真鸡儿难用，弄了半天也不知道怎么搞，其他大型的软件（maya等）也不想安装不想学操作，最后决定自己写一个。

本软件的主要思想是使用opengl中的射线拾取，具体方法就不阐述了，直接介绍本软件如何使用。

1. 打开软件PointPicker

   emmm 界面一般般，没有对界面进行优化

<img src="C:\Users\WK\Desktop\wk\markdown document\img\pointPicker1.png" alt="image-20191126193653455" style="zoom: 25%;" />

2. 点击loadModel 按钮

   注意：文件路径不能包含中文路径，目前只支持打开.obj格式的文件

   选择一个obj模型的结果如下

   <img src="C:\Users\WK\Desktop\wk\markdown document\img\pointPicker2.png" alt="image-20191126193930762" style="zoom:25%;" />

3. 选择复选框Point和picker

   如下面选择了三个点，被选中的点被红色标志，以及在日志中有输出相关信息

   本软件也提供了选取精度控制，默认是可以直接使用的，如果有选取操作不准确的情况下，可以适当调整精度的值。

   <img src="C:\Users\WK\Desktop\wk\markdown document\img\pointPicker3.png" alt="image-20191126194250992" style="zoom:25%;" />

4. 点击savePointsFile的按钮

   默认保存在模型所在的目录下，默认选择保存即可

<img src="C:\Users\WK\Desktop\wk\markdown document\img\pointPicker4.png" alt="image-20191126194630541" style="zoom:25%;" />

5. 文件格式

   已选择的点已经保存到pickedPoints.txt文件中

   文件中只需要读取以P开头的有效行，对每一有效行，第一列为标志位P，第二列为所选点在模型中的索引位置，第三四五列为所选点的xyz的坐标值

   <img src="C:\Users\WK\Desktop\wk\markdown document\img\pointPicker5.png" alt="image-20191126194912133" style="zoom: 33%;" />

   有软件相关的任何问题可以联系我