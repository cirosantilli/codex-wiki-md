<h1 id="1/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Direct [differentiation](../../../../../differentiation.md) gives

$$
\nabla a=(y,x,2z),\qquad \nabla\times\mathbf B=(y,-1,-1),\qquad \nabla a\cdot(\nabla\times\mathbf B)=y^2-x-2z.
$$

On the unit disk $D$, [polar coordinates](../../../../../polar-coordinates.md) give $\int_Dy^2\,dA=\pi/4$, $\int_Dx\,dA=0$ and $\int_DdA=\pi$. Consequently the [volume integral](../../../../../volume-integral.md) is

$$
\int_0^h\left(\frac\pi4-2\pi z\right)dz=\boxed{\frac{\pi h}{4}-\pi h^2}.
$$

For an independent [surface integral](../../../../../surface-integral.md) calculation, the relevant [cross product](../../../../../cross-product.md) is

$$
\mathbf F=\nabla a\times\mathbf B=(x^2+2yz^2,\ 2yz-xy,\ -y^2z-xy).
$$

The bottom face contributes $\int_Dxy\,dA=0$ and the top contributes $\int_D(-hy^2-xy)\,dA=-\pi h/4$. On the cylindrical side, put $x=\cos\theta$, $y=\sin\theta$, $\hat{\mathbf n}=(x,y,0)$ and $dS=d\theta\,dz$. The [flux](../../../../../flux.md) density is $x^3+2xyz^2+2y^2z-xy^2$. All terms except $2y^2z$ integrate to zero because they are [odd functions](../../../../../odd-function.md) of $x$ or $y$, giving

$$
\int_{\mathrm{side}}\mathbf F\cdot\hat{\mathbf n}\,dS=\int_0^h2\pi z\,dz=\pi h^2.
$$

Thus minus the total outward [flux](../../../../../flux.md) is $-(\pi h^2-\pi h/4)$, in agreement with the [volume integral](../../../../../volume-integral.md).

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [1](../../1.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
