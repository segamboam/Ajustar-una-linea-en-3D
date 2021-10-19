# Ajustar una linea en 3D
**Autor:**  
Sergio Esteban Gamboa Muñoz  
Agricultural Engineer,data scientist.   
segamboam@gmail.com

_______________________________________________________________________________________________________________
## Ejemplo del ajuste de una linea 3D para datos de frutos de durazno y sus respectivas ecuaciones.

Para este proyecto crearemos unos datos que tiene como referencia el crecimiento y desarrollo de los frutos de durazno por lo cual tenemos el tiempo (time), el diametro ecuatorial (dEcua) y el diametro Longitudinal (dLong).
<center>
<img src="notebooks/Points.png" height=455 width=650 >
</center>
Usando la descomposicion en valores singulares (SVD) creamos una linea 3D que mejor se ajusta a la nube de puntos. 
Para este ejemplo usamos 2 metodos.
1. Se realizaron los calculos usando numpy 
2. Se utilizo la libreria scikit-spatial
<center>
<img src="notebooks/Line3D.png" height=455 width=650 >
</center>

## Ecuaciones de la linea 3D:

La ecuación vectorial para una linea 3D se puede definir de la siguiente manera:  

<img src = "https://render.githubusercontent.com/render/math?math=(x,y,z)=(x_{0},y_{0},z_{0})+ \alpha(v_{1},v_{2},v_{3})"  height=30px >  
Para nuestra linea 3D de frutos de durazno seria:    
<img src = "https://render.githubusercontent.com/render/math?math=(x,y,z)=(100.07,3.149, 3.051)+ \alpha(0.999198, 0.02996106,0.02656469)" height=30px >  
La ecuación parametrica para una linea 3D se puede definir de la siguiente manera:  
<img src = "https://render.githubusercontent.com/render/math?math=\frac{x-x_{0}}{v1}=\frac{y-y_{0}}{v2}=\frac{z-z_{0}}{v3}" height=50px >   
Para nuestra linea 3D de frutos de durazno seria:  
<img src = "https://render.githubusercontent.com/render/math?math=\frac{9975x}{9967}-\frac{849628}{8483} = \frac{12583y}{377}-\frac{653630}{6217}=\frac{71260z}{1893}-\frac{891467}{7760}" height=50px >  
