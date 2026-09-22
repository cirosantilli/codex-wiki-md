<h1 id="30b/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

There is a missing hypothesis in the printed uniqueness claim: on an unbounded domain it is false without a condition at infinity. For example, on $\Omega=\{x_d>0\}$ take $f=0$ and $u_D=0$. Both $u=0$ and $u=x_d$ are classical solutions, although $f_u=0$.

For the intended bounded-domain statement, let $u,v\in C^2(\Omega)\cap C(\overline\Omega)$ be solutions and put $w=u-v$. The derivative assumption makes $f$ nondecreasing in its first argument. On the open set $D=\{x\in\Omega:w(x)>0\}$,

$$
\Delta w=f(u,x)-f(v,x)\ge0.
$$

The difference $w$ vanishes on $\partial\Omega$, and continuity makes it zero on every interior boundary point of $D$ as well. Since $D$ is bounded, the [weak maximum principle](../../../../../../weak-maximum-principle-for-elliptic-operators.md) for subharmonic functions gives $\sup_{\overline D}w\le\sup_{\partial D}w=0$, contradicting $w>0$ there unless $D$ is empty. Thus $u\le v$. Interchanging $u,v$ gives the reverse inequality, proving $\boxed{u=v}$. An appropriate bound or decay at infinity can replace boundedness, but the printed hypotheses alone do not include it.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [30B](../../30b.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
