<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Choose [measurable sets](../../../../measurable-set.md) $S_i$ carrying $\mu_i^s$ with $\kappa(S_i)=0$, and put $S=\bigcup_iS_i$. Every absolutely continuous component vanishes on $S$, and every singular component vanishes on its complement. The given restriction identity therefore gives

$$
\mu|_S=\bigvee_i\mu_i^s,\qquad
\mu|_{S^c}=\bigvee_i\mu_i^a.
$$

The first is singular with respect to $\kappa$. The second is absolutely continuous because it is bounded above by $\sum_i\mu_i^a$. They sum to $\mu$, so uniqueness identifies them as its Lebesgue components.

Let $h_i=d\mu_i^a/d\kappa$ and $h=\max_i h_i$, using measurable representatives. Each partition sum is at most $\int_Ah\,d\kappa$. For the reverse inequality, partition $A$ measurably by assigning a point to the smallest index attaining this finite maximum. On its assigned cell $h_i=h$, and the partition sum is exactly $\int_Ah\,d\kappa$. Thus

$$
\boxed{\frac{d\mu^a}{d\kappa}=\max_{1\leq i\leq N}\frac{d\mu_i^a}{d\kappa}\quad\kappa\text{-almost everywhere}.}
$$

The maximum of finitely many integrable nonnegative densities is integrable, since it is at most their sum.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the real and harmonic analysis course of the University of Oxford](../../../split.md)
5. [Real and harmonic analysis course of the University of Oxford](../../../../real-and-harmonic-analysis-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
