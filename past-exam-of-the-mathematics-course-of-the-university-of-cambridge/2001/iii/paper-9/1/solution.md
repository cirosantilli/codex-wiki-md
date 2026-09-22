<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Let $f$ be a nonzero [meromorphic function](../../../../../meromorphic-function.md) in a neighborhood of the closed disk $|z|\le R$, with no boundary zero or [pole](../../../../../pole.md). List its interior zeros $a_j$ with [multiplicities](../../../../../multiplicity-mathematics.md) $m_j$ and its interior [poles](../../../../../pole.md) $b_k$ with orders $n_k$. Define the disk [Green function](../../../../../green-s-function.md) and [Poisson kernel](../../../../../poisson-kernel-for-the-upper-half-plane.md) by

$$
G_R(z,a)=\log\left|\frac{R^2-\overline a z}{R(z-a)}\right|,\qquad P_R(z,\theta)=\frac{R^2-|z|^2}{|Re^{i\theta}-z|^2}.
$$

At every interior point that is neither a zero nor a [pole](../../../../../pole.md), the [Poisson-Jensen formula](../../../../../poisson-jensen-formula.md) is

$$
\boxed{\log|f(z)|=\frac1{2\pi}\int_0^{2\pi}P_R(z,\theta)\log|f(Re^{i\theta})|\,d\theta-\sum_jm_jG_R(z,a_j)+\sum_kn_kG_R(z,b_k).}
$$

In particular, at $z=0$ when $f(0)$ is finite and nonzero, this becomes [Jensen's formula](../../../../../jensen-s-formula.md), with each zero contributing $-m_j\log(R/|a_j|)$ and each [pole](../../../../../pole.md) contributing $n_k\log(R/|b_k|)$.

Here is a proof that also explains the signs. The disk [Blaschke factors](../../../../../blaschke-factor.md)

$$
B_a(z)=\frac{R(z-a)}{R^2-\overline a z}
$$

have a simple zero at $a$, no [poles](../../../../../pole.md) in the disk and boundary [modulus](../../../../../modulus.md) one. Therefore

$$
F(z)=f(z)\frac{\prod_kB_{b_k}(z)^{n_k}}{\prod_jB_{a_j}(z)^{m_j}}
$$

extends to a zero-free [holomorphic function](../../../../../holomorphic-function.md) throughout the disk. Its logarithmic [modulus](../../../../../modulus.md) is a [harmonic function](../../../../../harmonic-function.md) and agrees with $\log|f|$ on the boundary. The [Poisson integral](../../../../../poisson-integral.md) represents $\log|F(z)|$ by that boundary data. Since $\log|B_a|=-G_R(\cdot,a)$, substitution gives the displayed [Poisson-Jensen formula](../../../../../poisson-jensen-formula.md). Boundary zeros or [poles](../../../../../pole.md) can be handled by taking limiting radii: their logarithmic singularities are integrable. When zero is itself a zero or [pole](../../../../../pole.md), factor out its signed power of $z$ before evaluating [Jensen's formula](../../../../../jensen-s-formula.md) there.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 9](../../paper-9-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
