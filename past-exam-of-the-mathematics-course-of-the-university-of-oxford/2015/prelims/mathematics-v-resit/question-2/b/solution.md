<h1 id="question-2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use [cylindrical coordinates](../../../../../../cylindrical-coordinate-system.md). The real square root restricts the [projection](../../../../../../projection-linear-algebra.md) to $0\leq r\leq1$, and there $r-1\leq0\leq\sqrt{1-r^2}$. Since $\nabla x=\mathbf e_x$, the [volume integral](../../../../../../volume-integral.md) is

$$
\begin{aligned}
\iiint_V\nabla x\,dV
&=2\pi\mathbf e_x\int_0^1r\bigl(\sqrt{1-r^2}-r+1\bigr)\,dr\\
&=2\pi\mathbf e_x\left(\frac13-\frac13+\frac12\right)
=\boxed{\pi\mathbf e_x}.
\end{aligned}
$$

For an independent boundary calculation, split $\partial V$ into an upper [hemisphere](../../../../../../hemisphere.md) $S_+$ and a lower [right circular conical surface](../../../../../../right-circular-conical-surface.md) $S_-$. They meet in the [circle](../../../../../../circle.md) $r=1,z=0$ and there is no additional planar face.

On $S_+$, use the [parametrization](../../../../../../parametric-equation.md)

$$
\mathbf R(\alpha,\theta)
=(\sin\alpha\cos\theta,\sin\alpha\sin\theta,\cos\alpha),
\qquad 0\leq\alpha\leq\pi/2,\quad0\leq\theta\leq2\pi.
$$

The outward [unit normal vector](../../../../../../unit-normal.md) is $\mathbf R$, and the [surface area element](../../../../../../surface-area-element.md) is $\sin\alpha\,d\alpha\,d\theta$. The $y$ and $z$ components of $\iint_{S_+}x\mathbf n\,dS$ vanish by the angular [integrals](../../../../../../integral-split.md) of $\sin\theta\cos\theta$ and $\cos\theta$. The $x$ component is

$$
\int_0^{2\pi}\cos^2\theta\,d\theta\int_0^{\pi/2}\sin^3\alpha\,d\alpha
=\pi\cdot\frac23=\frac{2\pi}{3}.
$$

On $S_-$, the [parametrization](../../../../../../parametric-equation.md) $(r\cos\theta,r\sin\theta,r-1)$ has outward [vector area element](../../../../../../vector-area-element.md)

$$
\mathbf n\,dS=(\cos\theta,\sin\theta,-1)r\,dr\,d\theta.
$$

Its negative vertical component points out below the solid. Multiplying by $x=r\cos\theta$ and using the same angular [symmetry in integration](../../../../../../symmetry-in-integration.md) gives

$$
\iint_{S_-}x\mathbf n\,dS
=\mathbf e_x\int_0^1r^2\,dr\int_0^{2\pi}\cos^2\theta\,d\theta
=\frac\pi3\mathbf e_x.
$$

Therefore the independently evaluated [surface integral](../../../../../../surface-integral.md) is

$$
\boxed{\iint_{\partial V}x\mathbf n\,dS
=\left(\frac{2\pi}{3}+\frac\pi3\right)\mathbf e_x
=\pi\mathbf e_x,}
$$

in agreement with the [volume integral](../../../../../../volume-integral.md). The isolated apex of the [cone](../../../../../../cone-geometry.md) does not contribute to the [surface integral](../../../../../../surface-integral.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [Question 2](../../question-2.md)
3. [Mathematics V resit](../../../mathematics-v-resit-split.md)
4. [Prelims](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
