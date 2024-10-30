edge: significant local change in image intensity

![[Pasted image 20240911162123.png]]
**edge profiles:** sharp change in some property of the image

We define a function $f(x,y)$ which outputs the intensity of a pixel at position $(x,y)$. We define a gradient vector, $\mathbf{G}[f(x,y)]$, which computes small differences in pixel intensity at every pixel.

$$G[f(x,y)]=\begin{bmatrix}G_{x}\\ G_{y}\end{bmatrix} = \begin{bmatrix}\frac{\partial f}{dx}\\ \frac{\partial f}{dy}\end{bmatrix}$$