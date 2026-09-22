<h1 id="31e/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Testing a weak [Neumann Poisson problem](../../../../../../neumann-poisson-problem.md) with the constant function one gives $\int_\Omega f=0$, proving necessity. For sufficiency, use the closed [Hilbert space](../../../../../../hilbert-space-split.md) of mean-zero $H^1$ functions. The given [Poincaré inequality](../../../../../../poincare-inequality.md) makes $\|\nabla v\|_{L^2}$ an equivalent norm there. Set

$$
a(u,v)=\int_\Omega\nabla u\cdot\nabla v,\qquad \ell(v)=-\int_\Omega fv.
$$

The negative sign corresponds to $\Delta u=f$. Poincare's inequality gives boundedness of $\ell$ and coercivity of $a$. The [Lax-Milgram theorem](../../../../../../lax-milgram-theorem.md) supplies a unique mean-zero solution. Every $v\in H^1$ is the sum of its mean-zero part and a constant; since $\int f=0$, the weak identity extends to every $v\in H^1$. This is precisely the weak equation with zero normal derivative as its natural boundary condition. **Existence and uniqueness in the mean-zero space hold exactly when $\bar f=0$.**

## ↑ Ancestors (11)

1. [B](../b.md)
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
