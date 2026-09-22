<h1 id="16a/solution">Solution</h1>

↑ **Parent:** [16A](../16a.md)

For a [variation](../../../../../variation.md) $y+\varepsilon\eta$ preserving both endpoint values and slopes, $\eta=\eta'=0$ at the endpoints. The [first variation](../../../../../first-variation.md) is

$$
\delta J=\int_a^b(f_y\eta+f_{y'}\eta'+f_{y''}\eta'')\,dx.
$$

Integrate the last term twice and the middle term once. All boundary terms vanish, giving

$$
\delta J=\int_a^b\left(f_y-\frac{d}{dx}f_{y'}+\frac{d^2}{dx^2}f_{y''}\right)\eta\,dx.
$$

The [fundamental lemma of the calculus of variations](../../../../../fundamental-lemma-of-the-calculus-of-variations.md) yields the [higher-order Euler-Lagrange equation](../../../../../higher-order-euler-lagrange-equation.md)

$$
\boxed{f_y-\frac{d}{dx}f_{y'}+\frac{d^2}{dx^2}f_{y''}=0.}
$$

For the present functional this becomes $1+y-y^{(4)}=0$. Its general solution is $y=-1+A\cosh x+B\sinh x+C\cos x+D\sin x$. The left endpoint gives $C=-A$ and $D=-B$. The right endpoint then gives

$$
A(\cosh\pi+1)+B\sinh\pi=\cosh\pi+1,\qquad A\sinh\pi+B(\cosh\pi+1)=\sinh\pi.
$$

The coefficient [determinant](../../../../../determinant.md) is $2(1+\cosh\pi)>0$, so $A=1$, $B=0$. **The stationary function is $y_*(x)=-1+\cosh x-\cos x$.**

For any admissible perturbation $\eta$, exact quadratic expansion, followed by the stationarity equation and integration by parts, gives

$$
J[y_*+\eta]-J[y_*]=\frac12\int_0^\pi\left(\eta^2-(\eta'')^2\right)dx.
$$

Apply the supplied [Poincaré inequality](../../../../../poincare-inequality.md) first to $\eta$, then to $\eta'$, whose endpoint values also vanish:

$$
\int\eta^2\le\int(\eta')^2\le\int(\eta'')^2.
$$

Thus **$J[y_*+\eta]\le J[y_*]$ for every admissible perturbation**, proving a global maximum through the [clamped second-variation inequality](../../../../../clamped-second-variation-inequality.md).

## ↑ Ancestors (10)

1. [16A](../16a.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
