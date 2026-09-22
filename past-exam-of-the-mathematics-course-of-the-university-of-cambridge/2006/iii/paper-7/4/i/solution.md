<h1 id="4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For the [Riemann-Lebesgue lemma](../../../../../../riemann-lebesgue-lemma.md), a half-period shift of the oscillation gives a direct proof. For a nonzero integer $r$, set $h=\pi/r$. Periodicity and a change of variable show that the [Fourier coefficient](../../../../../../fourier-coefficient.md) of $t\mapsto f(t+h)$ at $r$ is $e^{irh}\widehat f(r)=-\widehat f(r)$. Thus

$$
2\widehat f(r)=\frac1{2\pi}\int_{-\pi}^{\pi}(f(t)-f(t+h))e^{-irt}\,dt,\qquad |\widehat f(r)|\leq\frac12\sup_t|f(t)-f(t+\pi/r)|.
$$

The right side tends to zero as $|r|\to\infty$ by [uniform continuity](../../../../../../uniform-continuity.md) on the [circle](../../../../../../circle.md). Consequently $\boxed{\widehat f(r)\to0\text{ as }|r|\to\infty}$.

There is nevertheless no prescribed rate shared by all continuous functions. Choose increasing positive integers $n_j$ with $k(n_j)\geq j2^j$, which is possible since $k(r)\to\infty$. Define

$$
g(t)=\sum_{j=1}^{\infty}2^{-j}e^{in_jt}.
$$

The series converges absolutely and uniformly, so $g$ is continuous. Termwise integration is justified by [uniform convergence](../../../../../../uniform-convergence.md), and the orthogonality of distinct exponential modes gives $\widehat g(n_j)=2^{-j}$. Hence

$$
k(n_j)|\widehat g(n_j)|\geq j,\qquad \boxed{\limsup_{r\to\infty}k(r)|\widehat g(r)|=\infty.}
$$

This [arbitrarily slow Fourier coefficient decay](../../../../../../arbitrarily-slow-fourier-coefficient-decay.md) is compatible with the [Riemann-Lebesgue lemma](../../../../../../riemann-lebesgue-lemma.md): for this particular function all [Fourier coefficients](../../../../../../fourier-coefficient.md) still tend to zero, but along the selected subsequence they beat the proposed decay scale by an unbounded factor.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [4](../../4.md)
3. [Paper 7](../../../paper-7-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
