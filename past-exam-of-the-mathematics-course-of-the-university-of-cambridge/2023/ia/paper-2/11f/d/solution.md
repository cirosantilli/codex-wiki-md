<h1 id="11f/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Take the spatial [Fourier transform](../../../../../../fourier-transform.md) of the [wave equation](../../../../../../wave-equation-split.md). The transformed initial-value problem is

$$
\widetilde u_{tt}+k^2\widetilde u=0,
\qquad
\widetilde u(k,0)=\widetilde f(k),
\qquad
\widetilde u_t(k,0)=\widetilde g(k),
$$

and hence

$$
\widetilde u(k,t)
=\widetilde f(k)\cos(kt)
+\widetilde g(k)\frac{\sin(kt)}k.
$$

Part (c) and the [convolution theorem](../../../../../../convolution-theorem.md) turn the first term into

$$
\frac12\bigl[f(x+t)+f(x-t)\bigr].
$$

For the second term, choose $p$ with $p'=g$. Part (b) says $\widetilde g=ik\widetilde p$, so

$$
\widetilde g(k)\frac{\sin(kt)}k
=i\widetilde p(k)\sin(kt).
$$

Part (c) now makes its inverse transform

$$
\frac12\bigl[p(x+t)-p(x-t)\bigr]
=\frac12\int_{x-t}^{x+t}g(\xi)\,d\xi.
$$

Combining the two terms gives the [D'Alembert formula](../../../../../../d-alembert-s-formula.md)

$$
\boxed{
u(x,t)=\frac12\bigl[f(x+t)+f(x-t)\bigr]
+\frac12\int_{x-t}^{x+t}g(\xi)\,d\xi.
}
$$

Let $A=2V$ and $B=W-V$. Part (c) makes $A$ and $B$ independent identically distributed exponential variables of rate $\lambda$. The change of variables $(A,B)=(rs,(1-r)s)$ has Jacobian $s$, and integrating $\lambda^2se^{-\lambda s}$ over $s>0$ gives density one for $0<r<1$. Therefore the [uniform ratio of independent exponential variables](../../../../../../uniform-ratio-of-independent-exponential-variables.md) gives

$$
\boxed{\frac{2V}{W+V}=\frac A{A+B}\sim\operatorname{Uniform}(0,1).}
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [11F](../../11f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
