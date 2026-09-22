<h1 id="30b/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The real [Lax-Milgram theorem](../../../../../../lax-milgram-theorem.md) states that if $V$ is a [Hilbert space](../../../../../../hilbert-space-split.md), $B:V\times V\to\mathbb R$ is a continuous bilinear form with $B(v,v)\ge\alpha\|v\|_V^2$ for some $\alpha>0$, and $\ell\in V^*$ is continuous, then there is a unique $u\in V$ such that $B(u,v)=\ell(v)$ for all $v\in V$. Moreover $\|u\|_V\le\|\ell\|/\alpha$.

Take the [Sobolev space](../../../../../../sobolev-space-split.md) $V=H_0^1(\Omega)$ with norm $\|v\|_V=\|\nabla v\|_2$. Since $\Omega$ is bounded, the [Poincaré inequality](../../../../../../poincare-inequality.md) gives $\|v\|_2\le C_P\|\nabla v\|_2$, making this norm equivalent to the full Sobolev norm. For the given bounded measurable coefficient define

$$
B(u,v)=\int_\Omega(\nabla u\cdot\nabla v+a(x)uv)dx,\qquad\ell(v)=\int_\Omega fv\,dx.
$$

Then $|B(u,v)|\le(1+\bar a C_P^2)\|u\|_V\|v\|_V$, $B(v,v)\ge\|v\|_V^2$ since $a\ge0$, and $|\ell(v)|\le C_P\|f\|_2\|v\|_V$. The [Lax-Milgram theorem](../../../../../../lax-milgram-theorem.md) therefore gives a unique $u\in H_0^1(\Omega)$ satisfying this identity, which is exactly the required [weak solution](../../../../../../weak-solution.md). Strict positivity of the lower coefficient bound is unnecessary: the zero boundary condition and boundedness supply coercivity through the gradient term.

## ↑ Ancestors (11)

1. [D](../d.md)
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
