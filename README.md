# Fit a line in 3D
**Author:** 
Sergio Esteban Gamboa Muñoz  
Data Analytics and Agricultural Engineer.  
segamboam@gmail.com  
https://www.linkedin.com/in/segamboam/

_______________________________________________________________________________________________________________
## Example of fitting a 3D line for peach fruit data and their respective equations

For this project we will create data that has as a reference the growth and development of peach fruits, for which we have the time (time), the equatorial diameter (dEcua) and the Longitudinal diameter (dLong).
<center>
<img src="notebooks/Points.png" height=455 width=650 >
</center>
Using singular value decomposition (SVD) we create a 3D line that best fits the point cloud.
For this example we use 2 methods.
1. Calculations were performed using numpy
2. The scikit-spatial library was used
<center>
<img src="notebooks/Line3D.png" height=455 width=650 >
</center>

## 3D line equations:

The vector equation for a 3D line can be defined as follows:  
<img src = "https://render.githubusercontent.com/render/math?math=(x,y,z)=(x_{0},y_{0},z_{0})+ \alpha(v_{1},v_{2},v_{3})"  height=30px >  
For our 3D line of peach fruits it would be:   
<img src = "https://render.githubusercontent.com/render/math?math=(x,y,z)=(100.07,3.149, 3.051)+ \alpha(0.999198, 0.02996106,0.02656469)" height=30px >  
The parametric equation for a 3D line can be defined as follows:  
<img src = "https://render.githubusercontent.com/render/math?math=\frac{x-x_{0}}{v1}=\frac{y-y_{0}}{v2}=\frac{z-z_{0}}{v3}" height=50px >   
For our 3D line of peach fruits it would be: 
<img src = "https://render.githubusercontent.com/render/math?math=\frac{9975x}{9967}-\frac{849628}{8483} = \frac{12583y}{377}-\frac{653630}{6217}=\frac{71260z}{1893}-\frac{891467}{7760}" height=50px >  
