<h1 id="1/c/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The preceding part shows that $\theta(e(t'))\ne0$ in characteristic zero, so $S^{\lambda'}\nsubseteq\ker\theta$. Apply the [James submodule theorem](../../../../../../../james-submodule-theorem.md) to the proper submodule $\ker\theta\leq M^{\lambda'}$ to obtain

$$
\ker\theta\subseteq(S^{\lambda'})^\perp.
$$

The [Hook-length formula](../../../../../../../hook-length-formula.md) gives $\dim S^\lambda=\dim S^{\lambda'}$. Surjectivity of $\theta$ therefore gives

$$
\operatorname{codim}\ker\theta=\dim S^\lambda=\dim S^{\lambda'}
=\operatorname{codim}(S^{\lambda'})^\perp,
$$

and hence

$$
\boxed{\ker\theta=(S^{\lambda'})^\perp}.
$$

Fix the original tableaux $t,u$. For a $\lambda$-tableau $w$, let $g_w$ be the unique permutation satisfying $w=g_wt$ and put $\varepsilon_w=\operatorname{sgn}(g_w)$. Since

$$
\theta(\{w'\})=\varepsilon_w e(w)\otimes e(u),
$$

the quotient pairing $M^{\lambda'}/(S^{\lambda'})^\perp\cong(S^{\lambda'})^*$ gives the explicit [conjugate Specht module as a sign-twisted dual](../../../../../../../conjugate-specht-module-as-a-sign-twisted-dual.md) isomorphism

$$
e(w)\otimes e(u)longmapsto
\left[e(v')\longmapsto
\varepsilon_w\langle\{w'\},e(v')\rangle\right]
$$

for every $\lambda$-tableau $w$.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [C](../../c.md)
3. [1](../../../1.md)
4. [Paper 160](../../../../paper-160-split.md)
5. [Iii](../../../../split.md)
6. [2021](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
