<h1 id="5d/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

After multiplication by $\sec^2x$, recognize both sides as derivatives:

$$
yy''+(y')^2=\sec^2x,\qquad
\frac{d}{dx}(yy'-\tan x)=0.
$$

The nontrivial [first integral](../../../../../../first-integral.md) is therefore

$$
\boxed{h(x,y,y')=yy'-\tan x=C_1.}
$$

It necessarily depends on the derivative, correcting the printed notation $h(x,y)$. A second integration gives

$$
\boxed{y^2=-2\log(\cos x)+2C_1x+C_2}
$$

on the specified interval. Since $y(0)=0$, $C_2=0$. A finite derivative at zero also implies $yy'\to0$ there, forcing $C_1=0$. A positive [particular solution](../../../../../../particular-solution.md) is consequently

$$
\boxed{y(x)=\sqrt{-2\log(\cos x)},\qquad 0\le x<\pi/2.}
$$

The negative of this function is the other sign choice. Near zero, $-2\log(\cos x)=x^2+x^4/6+O(x^6)$, so the positive branch has $y=x+x^3/12+O(x^5)$ and $y'(0)=1$; the negative branch has derivative $-1$.

For the positive branch, $y'=\tan x/y>0$. Its second derivative has numerator $-2\log\cos x-\sin^2x$, multiplied by a positive factor. This numerator is zero at zero and has derivative $2\sin^3x/\cos x>0$, so the curve is convex for positive $x$. It starts tangent to $y=x$ and rises without bound as $x\uparrow\pi/2$, with $y\sim\sqrt{-2\log(\pi/2-x)}$. The third panel of the sketch above shows this branch.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5D](../../5d.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
