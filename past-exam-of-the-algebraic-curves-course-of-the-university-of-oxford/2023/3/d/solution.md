<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

An explicit answer, initially written where $yz\ne0$, is the [meromorphic differential on a Riemann surface](../../../../meromorphic-differential-on-a-riemann-surface.md)

$$
\boxed{\eta=\frac{d(x/z)}{y/z}=\frac{z\,dx-x\,dz}{yz}.}
$$

The ratios $x/z$ and $y/z$ are functions on $C$, so the expression does not depend on the representative of its [homogeneous coordinates](../../../../homogeneous-coordinate.md). It is a scalar multiple of an [invariant differential on an elliptic curve](../../../../invariant-differential-on-an-elliptic-curve.md).

On the [complex torus](../../../../complex-torus.md) $\mathbb C/\Lambda$, the differential $dw$ descends from $\mathbb C$ because translation by any element of the [period lattice](../../../../period-lattice.md) leaves $dw$ unchanged. It is [holomorphic](../../../../holomorphic-function-split.md) and nowhere zero. The given [biholomorphism](../../../../biholomorphism.md) satisfies, wherever the displayed quotient is initially defined,

$$
\Phi^*\eta=\frac{d\wp(w)}{\wp'(w)}=dw.
$$

Consequently, $\eta=(\Phi^{-1})^*(dw)$ extends across every apparent denominator zero and across $[0:1:0]$ as a nonzero [holomorphic differential form](../../../../holomorphic-differential-form.md) on all of $C$.

One can also check the apparent exceptional points directly. On $z=1$, put $P(X)=4\prod_i(X-e_i)$, so $Y^2=P(X)$. At $Y=0$ the roots are distinct, and differentiating gives

$$
\frac{dX}{Y}=\frac{2\,dY}{P'(X)},
$$

which is regular and nonvanishing there. At $[0:1:0]$, use $u=x/y$, $v=z/y$. The equation is $v=4\prod_i(u-e_iv)$, so $u$ is a [local parameter on a smooth algebraic curve](../../../../local-parameter-on-a-smooth-algebraic-curve.md) and $v=4u^3+O(u^5)$. Hence

$$
\eta=v\,d(u/v)=du-\frac{u}{v}\,dv=(-2+O(u^2))\,du,
$$

also regular and nonvanishing.

Only distinctness of the $e_i$ is needed. The paper additionally writes $e_i\ne0$, which is not true for every [period lattice](../../../../period-lattice.md): for $\Lambda=\mathbb Z+\mathrm i\mathbb Z$, the symmetry $\wp(\mathrm iw)=-\wp(w)$ makes the half-period value at $w=(1+\mathrm i)/2$ zero, since $\mathrm iw\equiv w\pmod\Lambda$. This unnecessary restriction has no effect on the answer.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [3](../../3.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the algebraic curves course of the University of Oxford](../../../split.md)
5. [Algebraic curves course of the University of Oxford](../../../../algebraic-curves-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
