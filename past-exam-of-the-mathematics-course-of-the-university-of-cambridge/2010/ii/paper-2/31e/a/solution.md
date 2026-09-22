<h1 id="31e/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Lax-Milgram theorem](../../../../../../lax-milgram-theorem.md) states that on a real [Hilbert space](../../../../../../hilbert-space-split.md), a bounded bilinear form $a$ satisfying $a(v,v)\geq c\|v\|^2$ for some $c>0$ represents every bounded linear functional uniquely: there is a unique $u$ with $a(u,v)=\ell(v)$ for all $v$.

The clamped trace conditions define a closed subspace $H_\partial^2(\Omega)$ of the [Sobolev space](../../../../../../sobolev-space-split.md) $H^2(\Omega)$. On it take $a(u,v)=\int_\Omega\Delta u\,\Delta v$ and $\ell(v)=\int_\Omega fv$. Both are bounded by the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md). The Dirichlet [elliptic regularity](../../../../../../elliptic-regularity.md) estimate on a smooth bounded domain gives $\|v\|_{H^2}\leq C\|\Delta v\|_{L^2}$ for $v\in H^2\cap H_0^1$, so $a(v,v)\geq C^{-2}\|v\|_{H^2}^2$. The [Lax-Milgram theorem](../../../../../../lax-milgram-theorem.md) now gives exactly one $u$ satisfying

$$
\int_\Omega\Delta u\,\Delta v=\int_\Omega fv\qquad(v\in H_\partial^2(\Omega)).
$$

Testing with compactly supported smooth $v$ and integrating by parts twice gives $\Delta^2u=f$ in distributions; the two boundary conditions hold as traces by the space's definition. **This is the unique weak clamped biharmonic solution.**

## ↑ Ancestors (11)

1. [A](../a.md)
2. [31E](../../31e.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
