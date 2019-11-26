##  PointPicker 

This software is used to select points on the obj model and save them in a file.

## Development environment
This software is developed based on QT5.6/C++

## Instructions 

### 1. Open PointPicker software 

  interface is shown as follow:

<p align="center">
	<img src="https://github.com/kaiwu119/PointPicker/blob/master/img/pointPicker1.png" alt="Sample"  width="600" height="350">
	<p align="center">
		<em></em>
	</p>
</p>

### 2. click loadModel button

   Note: The file path cannot contain Chinese path

   The result of selecting an obj model is as follows

 <p align="center">
	<img src="https://github.com/kaiwu119/PointPicker/blob/master/img/pointPicker2.png" alt="Sample"  width="600" height="350">
	<p align="center">
		<em>demo</em>
	</p>
</p>

### 3. click Check box Point and picker

   You can select points by right-clicking.
   As follows, three points are selected, the selected points are marked in red, and output related information is in the log

   This software also provides selection precision control, which can be used directly by default. If the selection operation is not accurate, you can adjust the precision value appropriately.
   
<p align="center">
	<img src="https://github.com/kaiwu119/PointPicker/blob/master/img/pointPicker3.png" alt="Sample"  width="600" height="350">
	<p align="center">
		<em>demo</em>
	</p>
</p>

### 4. click savePointsFile button

   The file is saved in the directory where the model is located by default, and you can choose to save it directly.

<p align="center">
	<img src="https://github.com/kaiwu119/PointPicker/blob/master/img/pointPicker4.png" alt="Sample"  width="600" height="350">
	<p align="center">
		<em>demo</em>
	</p>
</p>

### 5. file format

   Selected points have been saved to pickedPoints.txt file

   Only the valid lines starting with P need to be read in the file. For each valid line, the first column is the flag P, the second column is the index position of the selected point in the model, and the third and fourth columns are the selected points' Xyz coordinates

 <p align="center">
	<img src="https://github.com/kaiwu119/PointPicker/blob/master/img/pointPicker5.png" alt="Sample"  width="600" height="350">
	<p align="center">
		<em>demo</em>
	</p>
</p>
