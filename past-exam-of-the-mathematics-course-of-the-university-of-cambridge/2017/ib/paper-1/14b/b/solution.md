<h1 id="14b/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For smooth rapidly decaying initial data, apply the [Fourier transform](../../../../../../fourier-transform.md) in $x$ and differentiate under the [integral](../../../../../../integral.md). The [Fourier transform of a derivative](../../../../../../fourier-transform-of-a-derivative.md) turns the [wave equation](../../../../../../wave-equation-split.md) into

$$
\widetilde v_{tt}+k^2\widetilde v=0,\quad\widetilde v(k,0)=\widetilde f(k),\quad\widetilde v_t(k,0)=\widetilde g(k).
$$

Solving this constant-coefficient [ordinary differential equation](../../../../../../ordinary-differential-equation.md) gives

$$
\boxed{\widetilde v(k,t)=\widetilde f(k)\cos kt+\widetilde g(k)\frac{\sin kt}{k}}.
$$

At $k=0$ the quotient means its continuous limit $t$, so $\widetilde v(0,t)=\widetilde f(0)+t\widetilde g(0)$.

Since $\cos kt=(e^{ikt}+e^{-ikt})/2$, the [Translation property of the Fourier transform](../../../../../../translation-property-of-the-fourier-transform.md) inverts the first term as $(f(x+t)+f(x-t))/2$. Also $K_t(x)=\tfrac12\mathbf1_{[-t,t]}(x)$ has [Fourier transform](../../../../../../fourier-transform.md) $\sin kt/k$, including its limiting value at zero. The [convolution theorem](../../../../../../convolution-theorem.md) therefore inverts the second term as

$$
(K_t*g)(x)=\frac12\int_{-t}^t g(x-s)\,ds=\frac12\int_{x-t}^{x+t}g(\xi)\,d\xi.
$$

This proves the [D'Alembert formula](../../../../../../d-alembert-s-formula.md)

$$
\boxed{v(x,t)=\frac{f(x-t)+f(x+t)}2+\frac12\int_{x-t}^{x+t}g(\xi)\,d\xi}.
$$

The formula itself extends beyond the rapidly decaying class: $f\in C^2$ and $g\in C^1$ suffice for a classical solution, verified by differentiation and the two initial conditions. The decay assumption above justifies the ordinary transform derivation without distributional qualifications.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [14B](../../14b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
