<h1 id="3/a/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Use the [smooth periodic partition of unity](../../../../../smooth-periodic-partition-of-unity.md) $\Psi$ above and define the [Fourier coefficients](../../../../../fourier-coefficient.md) of the [periodic distribution](../../../../../periodic-distribution.md) by

$$
c_n=\frac1{2\pi}\langle u,\Psi(x)e^{-inx}\rangle,\qquad n\in\mathbb Z.
$$

These are the [smooth-window Fourier coefficients of a periodic distribution](../../../../../smooth-window-fourier-coefficients-of-a-periodic-distribution.md) for period $2\pi$. The finite [Schwartz seminorm](../../../../../schwartz-seminorm.md) bound for $u$, restricted to the fixed [compact support](../../../../../compact-support.md) of $\Psi$, gives $|c_n|\leq C(1+|n|)^N$ for some $C,N$. Indeed, only finitely many [derivatives](../../../../../derivative.md) of $\Psi e^{-inx}$ occur, and each contributes at most a fixed power of $|n|$.

For a [Schwartz function](../../../../../schwartz-function.md) $\phi$, the preceding [Fourier series](../../../../../fourier-series-split.md) formula and $\widehat{\widehat\phi}(n)=2\pi\phi(-n)$ yield

$$
P\widehat\phi(x)=\sum_{n\in\mathbb Z}\phi(-n)e^{inx}.
$$

All [derivatives](../../../../../derivative.md) of this series converge uniformly. The localization formula in the previous answer therefore gives

$$
\begin{aligned}
\langle\widehat u,\phi\rangle
&=\langle u,\widehat\phi\rangle
=\langle u,\Psi P\widehat\phi\rangle\\
&=\sum_n\phi(-n)\langle u,\Psi e^{inx}\rangle
=2\pi\sum_n c_n\phi(n).
\end{aligned}
$$

Consequently the [Fourier transform of a periodic distribution](../../../../../fourier-transform-of-a-periodic-distribution.md) is

$$
\boxed{\widehat u=2\pi\sum_{n\in\mathbb Z}c_n\delta_n\quad\text{in }\mathcal S'(\mathbb R).}
$$

The polynomial bound on $c_n$ and rapid decay of $\phi(n)$ make every displayed pairing absolutely convergent. In particular there are no [derivatives](../../../../../derivative.md) of [Dirac delta distributions](../../../../../dirac-delta-function.md) in this formula.

The [inverse Fourier transform](../../../../../inverse-fourier-transform.md) of $\delta_n$ is $(2\pi)^{-1}e^{inx}$. Applying continuous [Fourier inversion](../../../../../fourier-inversion-theorem.md) on [tempered distributions](../../../../../tempered-distribution.md) to the symmetric partial sums gives

$$
\boxed{u=\sum_{n\in\mathbb Z}c_ne^{inx}\quad\text{in }\mathcal S'(\mathbb R).}
$$

Explicitly, for every [Schwartz function](../../../../../schwartz-function.md) $\theta$, the pairing of the partial sum with $\theta$ is $\sum_{|n|\leq M}c_n\widehat\theta(-n)$, which converges absolutely to $\langle u,\theta\rangle$. The [Fourier transform](../../../../../fourier-transform-split.md) formula also proves that $c_n$ is independent of the chosen [smooth periodic partition of unity](../../../../../smooth-periodic-partition-of-unity.md). For a locally integrable $2\pi$ [periodic function](../../../../../periodic-function.md) it reduces, by splitting the integral into periods, to $c_n=(2\pi)^{-1}\int_0^{2\pi}u(x)e^{-inx}\,dx$.

## ↑ Ancestors (13)

1. [Iv](../iv.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the fourier analysis course of the University of Oxford](../../../../split.md)
6. [Fourier analysis course of the University of Oxford](../../../../../fourier-analysis-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
