## Copy the data into system memory for fast access
HDD(CPU)->RAM(CPU)->VRAM(GPU)  

## Set the Render State
vertex and pixel shader, texture, material, lighting, transparency...
## Draw Call
CPU ---command---> GPU

## Pipeline
GPU:  Render State ---> pixels on screen 
```
1. Not everything is done by the “tiny” GPU cores    
2. There can be several parallel running pipelines    
```
### Applicatoin Stage
### Driver Stage
### Read Commands
### Data Fetch
### Vertex Fetch
### Shader Execution
### Patch Assembly
### Hull Shader
### Tessellation
### Domain Shader
### Geometry Shader
### Viewport Transform & Clipping
### Triangles Journey  
### Rasterizing
### Pixel Shader
### Raster Output
moving pixel data, pixel blending(像素混合), coverage information for anti aliasing(抗锯齿) , “atomic operations”.


## Rendering
Rendering is basically doing an immense number of small tasks such as calculate something for thousands of vertices or painting millions of pixels on a screen.                
>=  30fps    

```
Modern CPUs have 4-8 cores that can do each 4-8 float operations at once    
GPUs can have several thousands operation Units    
Just comparing GPU core and CPU core count is not fair due to the different responsibilities and organization     
GPU vendors tend to use “core” for the smallest execution unit, while CPU vendors for the high-level unit  
```
## command buffer (FIFO)
CPU and GPU can work independent from each other   

## ref
https://blog.csdn.net/hexiaolong2009/article/details/104084445   

https://blog.csdn.net/hexiaolong2009/article/details/104088308   

https://blog.csdn.net/hexiaolong2009/article/details/104089572    

https://blog.csdn.net/hexiaolong2009/article/details/104108749     

https://blog.csdn.net/hexiaolong2009/article/details/104108917   


https://simonschreibt.de/gat/renderhell-book1
https://simonschreibt.de/gat/renderhell-book2
https://simonschreibt.de/gat/renderhell-book3
https://simonschreibt.de/gat/renderhell-book4
https://simonschreibt.de/gat/renderhell-book5
