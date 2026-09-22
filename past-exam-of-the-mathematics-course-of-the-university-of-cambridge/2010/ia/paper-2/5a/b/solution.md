<h1 id="5a/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Set $v=u''$. The resulting [second-order linear differential equation](../../../../../../second-order-linear-differential-equation.md) is $v''+2v=4t^2$. A [polynomial](../../../../../../polynomial-split.md) [particular solution](../../../../../../particular-solution.md) $v_p=at^2+b$ requires $2a=4$ and $2a+2b=0$, hence $v_p=2t^2-2$. The homogeneous [characteristic roots of a constant-coefficient differential equation](../../../../../../characteristic-root-of-a-constant-coefficient-differential-equation.md) are $\pm i\sqrt2$, so

$$
v=A_1\cos(\sqrt2t)+B_1\sin(\sqrt2t)+2t^2-2.
$$

Integrating twice and renaming constants gives **the general real solution**

$$
\boxed{u(t)=A\cos(\sqrt2t)+B\sin(\sqrt2t)+Ct+D+\frac{t^4}{6}-t^2.}
$$

The four independent homogeneous terms account for the four initial data of the fourth-order [linear ordinary differential equation](../../../../../../linear-ordinary-differential-equation.md).

For the substitution $u(t)=y(t^2)$, repeated use of the [chain rule](../../../../../../chain-rule.md), with $x=t^2$, gives

$$
u''=2y'+4t^2y'',\qquad
u''''=12y''+48t^2y'''+16t^4y''''.
$$

Therefore

$$
u''''+2u''=4\bigl(4x^2y''''+12xy'''+(3+2x)y''+y'\bigr).
$$

For $x>0$, the map $t=\sqrt x$ is invertible, and the transformed equation is exactly the equation just solved. Hence **the general real solution on $x>0$ is**

$$
\boxed{y(x)=A\cos(\sqrt{2x})+B\sin(\sqrt{2x})+C\sqrt x+D+\frac{x^2}{6}-x.}
$$

There is no requirement that $u$ extend as an even function through $t=0$: only the branch $t>0$ is needed, so the sine and square-root terms must be retained.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5A](../../5a.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
