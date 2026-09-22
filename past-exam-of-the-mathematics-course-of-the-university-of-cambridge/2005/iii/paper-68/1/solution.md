<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use the [uniform norm](../../../../../supremum-norm.md) and the central second difference $\delta_h^2f(x)=f(x+h)-2f(x)+f(x-h)$, with

$$
\omega_2(f,a)=\sup_{|h|\leq a}\|\delta_h^2f\|_\infty.
$$

The [Jackson kernel](../../../../../jackson-kernel.md) is even, nonnegative and normalized. Pairing $t$ and $-t$ in its integral therefore gives

$$
j_n f(x)-f(x)=\frac12\int_{-\pi}^{\pi}\delta_t^2f(x)J_n(t)\,dt.
$$

We will estimate this expression directly in terms of the [second modulus of smoothness](../../../../../second-modulus-of-smoothness.md).

First prove the modulus scaling bound. With translations $T_hf(x)=f(x+h)$, the forward difference obeys

$$
(T_{mh}-I)^2=(T_h-I)^2\left(\sum_{r=0}^{m-1}T_{rh}\right)^2.
$$

Each [function translation](../../../../../translation-of-a-function.md) preserves the [uniform norm](../../../../../supremum-norm.md), so $\|\delta_{mh}^2f\|_\infty\leq m^2\|\delta_h^2f\|_\infty$. For $t\ne0$, take $m=\lceil n|t|\rceil$ and $h=t/m$. Then $|h|\leq1/n$ and

$$
\|\delta_t^2f\|_\infty\leq(1+n|t|)^2\omega_2(f,1/n).
$$

The same bound is immediate at $t=0$.

For $|t|\leq\pi$, $|\sin(t/2)|\geq|t|/\pi$. Also $|\sin(nt/2)/\sin(t/2)|\leq n$, as follows by expressing the ratio, up to a unit-modulus factor, as a sum of $n$ complex exponentials. The given normalizing coefficient is at most a constant times $n^{-3}$. Consequently

$$
J_n(t)\leq Cn,\qquad
J_n(t)\leq\frac{C}{n^3|t|^4}\quad(t\ne0),
$$

and these two estimates combine into

$$
J_n(t)\leq\frac{C'n}{(1+n|t|)^4}.
$$

Indeed splitting at $n|t|=1$ shows this with an absolute change of constant. Hence

$$
\int_{-\pi}^{\pi}(1+n|t|)^2J_n(t)\,dt
\leq2C'\int_0^{n\pi}\frac{du}{(1+u)^2}\leq2C'.
$$

Substitute the modulus bound in the symmetrized [convolution](../../../../../convolution.md) and take the supremum over $x$ to obtain the [Jackson operator estimate](../../../../../jackson-operator-estimate.md)

$$
\boxed{\|j_nf-f\|_\infty\leq C'\omega_2(f,1/n).}
$$

The constant is independent of $f$ and the positive integer $n$; the kernel's quartic decay is what makes the weighted second-difference integral uniformly bounded.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 68](../../paper-68-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
