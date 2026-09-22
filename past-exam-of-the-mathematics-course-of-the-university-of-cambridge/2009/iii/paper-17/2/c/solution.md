<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

**The direct-sum assertion fails in both degrees when the pieces overlap.** Take genuine [open covers](../../../../../../open-cover.md), so the failure does not depend on any subtle choice of smooth structures on subsets.

For degree zero, let $M=\mathbb R$, $U=(-\infty,1)$ and $V=(-1,\infty)$. By [degree-zero de Rham cohomology](../../../../../../degree-zero-de-rham-cohomology.md), $H^0_{\mathrm{dR}}$ consists of [locally constant functions](../../../../../../locally-constant-function.md). Each of $M,U,V$ is connected and nonempty, so

$$
H^0_{\mathrm{dR}}(M)=\mathbb R,\qquad H^0_{\mathrm{dR}}(U)\oplus H^0_{\mathrm{dR}}(V)=\mathbb R^2.
$$

They are not isomorphic as real [vector spaces](../../../../../../vector-space-split.md). The restriction map is $c\mapsto(c,c)$; the overlap forces equality instead of allowing two independent constants.

For degree one, let $M=S^1$, and remove distinct points $a,b$ to form $U=S^1\setminus\{a\}$ and $V=S^1\setminus\{b\}$. Each is diffeomorphic to an [open interval](../../../../../../open-interval.md). Every one-form $f(t)dt$ on an interval has the smooth primitive $\int_{t_0}^t f(s)ds$, so both pieces have zero first [de Rham cohomology](../../../../../../de-rham-cohomology.md). On the [circle](../../../../../../circle.md), the form $\eta=x\,dy-y\,dx$ is closed because all two-forms on a one-dimensional manifold vanish. The parameterization $(x,y)=(\cos t,\sin t)$ gives

$$
\int_{S^1}\eta=\int_0^{2\pi}dt=2\pi.
$$

An exact form has zero [integral](../../../../../../integral.md) around this loop: the [integral](../../../../../../integral.md) of $dF$ is the difference of the endpoint values of the periodic function $F$. Thus $[\eta]\ne0$, while the proposed right side is zero, disproving the isomorphism.

In fact $H^1_{\mathrm{dR}}(S^1)\cong\mathbb R$. For a periodic one-form $f(t)dt$, subtract $c\,dt$ where $c=(2\pi)^{-1}\int_0^{2\pi}f(t)dt$. The remainder has the periodic primitive $\int_0^t(f(s)-c)ds$, and hence is exact. This also explicitly identifies the nonzero class used above.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 17](../../../paper-17-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
