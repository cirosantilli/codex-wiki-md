<h1 id="4d/solution">Solution</h1>

↑ **Parent:** [4D](../4d.md)

A capacitor consists of two conductors carrying equal and opposite charges. Its [capacitance](../../../../../capacitance.md) is

$$
C=\frac QV,
$$

where $Q$ is the magnitude of the charge on either conductor and $V$ is their potential difference.

For $a<r<b$, a coaxial Gaussian cylinder of length $\ell$ encloses charge $\lambda\ell$. [Gauss's law](../../../../../gauss-s-law.md) gives

$$
E(r)=\frac{\lambda}{2\pi\epsilon_0r}\,e_r.
$$

Taking $V$ to mean the inner potential minus the outer potential,

$$
V=\int_a^bE(r)\,dr
=\frac{\lambda}{2\pi\epsilon_0}\log\frac ba.
$$

Since $Q=\lambda L$,

$$
\boxed{C=\frac{2\pi\epsilon_0L}{\log(b/a)}}.
$$

The field energy is

$$
\begin{aligned}
U
&=\frac{\epsilon_0}{2}
\int_a^bE(r)^2(2\pi rL)\,dr\\
&=\frac{\lambda^2L}{4\pi\epsilon_0}\log\frac ba
=\frac12(\lambda L)
\left(\frac{\lambda}{2\pi\epsilon_0}\log\frac ba\right)
=\frac12QV.
\end{aligned}
$$

These are the standard [coaxial cylindrical capacitor](../../../../../coaxial-cylindrical-capacitor.md) formulas.

## ↑ Ancestors (10)

1. [4D](../4d.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
