<h1 id="15d/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Measure the second register of $|f\rangle$. If the result is $f(x_0)$, injectivity within one period collapses the first register to the [periodic coset state](../../../../../../periodic-coset-state.md)

$$
|\alpha\rangle=\frac1{\sqrt A}\sum_{k=0}^{A-1}|x_0+kr\rangle,
\qquad A=\frac Nr.
$$

Apply $\operatorname{QFT}_N$ and measure the first register. By the stated transform identity, the outcome is

$$
c=lA=\frac{lN}{r}
$$

for a uniformly random $l\in\{0,\ldots,r-1\}$.

Reduce the rational number

$$
\frac cN=\frac lr
$$

to lowest terms and call its denominator $q$. The [exact period recovery from a Fourier sample](../../../../../../exact-period-recovery-from-a-fourier-sample.md) gives

$$
q=\frac r{\gcd(l,r)}.
$$

Thus $q=r$ exactly when $l$ is coprime to $r$.

The success can be certified with two classical function evaluations. Compute $f(0)$ and $f(q)$. Since $q\mid r$ and $0\leq q\leq r$, periodicity and injectivity within a period imply

$$
f(q)=f(0)\iff q=r.
$$

Report $q$ only when this equality holds; otherwise report failure. The success probability is

$$
\boxed{\frac{\varphi(r)}r=\Omega\left(\frac1{\log\log N}\right),}
$$

using the standard lower bound for the [Euler totient function](../../../../../../euler-totient-function.md). This is [heralded exact quantum period finding when the period divides the register size](../../../../../../heralded-exact-quantum-period-finding-when-the-period-divides-the-register-size.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [15D](../../15d.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
