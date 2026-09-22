<h1 id="14d/solution">Solution</h1>

↑ **Parent:** [14D](../14d.md)

The inner circle has centre $2/5$ and radius $2/5$. The pole $z=1/2$ of the [Möbius transformation](../../../../../mobius-transformation.md) lies inside that removed disc, so the transformation is holomorphic on $D$, with derivative $3/(2z-1)^2\ne0$.

For $z=x+iy$,

$$
|w|^2=\frac{|z|^2-4x+4}{4|z|^2-4x+1}.
$$

On the outer boundary this is one. On the inner boundary, $|z|^2=4x/5$, and the ratio is four. More directly, inside the outer circle the numerator exceeds the denominator by $3(1-|z|^2)>0$, whereas outside the inner circle four times the denominator exceeds the numerator by $3(5|z|^2-4x)>0$. Thus the image is $1<|w|<2$. The inverse transformation is $z=(w-2)/(2w-1)$, so this is a bijective [conformal map](../../../../../conformal-map.md) onto that annulus.

A radial [harmonic function](../../../../../harmonic-function.md) on an annulus has form $A+B\log|w|$. The two boundary values give $A=1$, $B=1/\log2$. By [conformal invariance of harmonicity](../../../../../conformal-invariance-of-harmonicity.md),

$$
\boxed{\phi(x,y)=1+\frac{\log\left|\dfrac{z-2}{2z-1}\right|}{\log2},\qquad z=x+iy.}
$$

It has the required boundary values, and the [maximum principle for harmonic functions](../../../../../maximum-principle-for-harmonic-functions.md) proves uniqueness among solutions continuous on the closed region.

## ↑ Ancestors (10)

1. [14D](../14d.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
