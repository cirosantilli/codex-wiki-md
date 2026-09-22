<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For the indicated function the cosine substitution gives

$$
\widetilde f_0(\theta)=\sqrt{1-\cos^2\theta}=|\sin\theta|.
$$

The absolute-value function is [Lipschitz continuous](../../../../../../lipschitz-continuity.md) with constant one, and so is sine. Their composition therefore satisfies

$$
\big||\sin(\theta+h)|-|\sin\theta|\big|\le |h|,
\qquad \omega(\widetilde f_0,\delta)\le\delta.
$$

Use the sharper intermediate estimate from the preceding part, rather than the ordinary interval [modulus of continuity](../../../../../../modulus-of-continuity.md):

$$
\boxed{E_n^{\mathrm{alg}}(f_0)\le C/n=O(n^{-1})}.
$$

The usual [inverse theorem for trigonometric approximation](../../../../../../inverse-theorem-for-trigonometric-approximation.md) cannot hold verbatim with the ordinary interval [modulus of continuity](../../../../../../modulus-of-continuity.md). It would imply

$$
\omega(f_0,1/n)\le\frac{C'}n\sum_{\nu=0}^n E_\nu^{\mathrm{alg}}(f_0)
=O\!\left(\frac{\log(n+1)}n\right).
$$

But comparison with the endpoint $1$ gives

$$
\omega(f_0,1/n)\ge |f_0(1-1/n)-f_0(1)|
=\sqrt{\frac2n-\frac1{n^2}},
$$

which is of order $n^{-1/2}$ and contradicts that bound as $n\to\infty$. This is an [endpoint obstruction to an algebraic inverse approximation theorem](../../../../../../endpoint-obstruction-to-an-algebraic-inverse-approximation-theorem.md). The algebraic approximation rate measures smoothness after cosine substitution; cosine compresses distances quadratically near the endpoints. A valid algebraic inverse theorem must account for that endpoint geometry rather than using the unchanged periodic formulation.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 61](../../../paper-61-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
