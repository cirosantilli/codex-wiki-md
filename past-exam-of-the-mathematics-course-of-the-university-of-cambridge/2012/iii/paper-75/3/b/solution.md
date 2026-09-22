<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

With no net body force, the tensile resultant is constant along the thread: $3\mu Aw_z=F(t)$. In material coordinates $z_0$, volume conservation gives $D_tA=-F/(3\mu)$. Thus

$$
\boxed{A=A_0(z_0)-\Delta(t),\qquad
\Delta(t)=\frac1{3\mu}\int_0^tF(t')\,dt'.}
$$

The material Jacobian satisfies $A\,\partial z/\partial z_0=A_0$. Integrating with $z(0,t)=0$ gives

$$
\boxed{z=z_0+\int_0^{z_0}\frac{\Delta\,dz'_0}{A_0(z'_0)-\Delta}.}
$$

This remains valid while $\Delta<\min A_0$. The even profile now specified ensures symmetric endpoints $\pm L(t)$.

For $A_0=C(1+k^2z_0^2)$ and $k\ne0$, direct integration yields

$$
L=L_0+\frac{\Delta}{|k|\sqrt{C(C-\Delta)}}
\tan^{-1}\left(|k|L_0\sqrt{\frac C{C-\Delta}}\right).
$$

For $k=0$, instead $L=CL_0/(C-\Delta)$. A constant tensile $F>0$ gives $\Delta=Ft/(3\mu)$ and **the finite blow-up time**

$$
\boxed{t^*=\frac{3\mu C}{F}.}
$$

Put $\alpha=F/(3\mu)$ and $\delta=C-\Delta=\alpha(t^*-t)$. For fixed nonzero $k$, the arctangent tends to $\pi/2$, whereas for the uniform profile the whole length has the same thinning. Consequently **the [localized-neck and uniform-thread stretching exponents](../../../../../../localized-neck-and-uniform-thread-stretching-exponents.md) are**

$$
\boxed{
\begin{aligned}
k\ne0:\quad&\beta=-\tfrac12,\qquad
B=\frac{\pi}{2|k|}\sqrt{\frac{3\mu C}{F}},\\
k=0:\quad&\beta=-1,\qquad B=\frac{3\mu CL_0}{F}.
\end{aligned}}
$$

A nonuniform thread's divergent integral is concentrated in a material interval $|z_0|\sim\sqrt{\delta/C}/|k|$ near its quadratic minimum. Its width shrinks like $\delta^{1/2}$ while the Jacobian grows like $\delta^{-1}$, yielding $\delta^{-1/2}$. The remote ends no longer affect this leading coefficient, explaining independence from $L_0$. For $k=0$ every element contributes the same $\delta^{-1}$ stretch. The limits $k\to0$ and $t\to t^*$ do not commute.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 75](../../../paper-75-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
