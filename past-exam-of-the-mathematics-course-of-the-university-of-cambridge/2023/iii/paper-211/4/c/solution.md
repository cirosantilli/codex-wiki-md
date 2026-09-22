<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Define the risk-neutral claim value

$$
V(t,s)=e^{-r(T-t)}
\int_{\mathbb R}g\left(
s e^{(r-\sigma^2/2)(T-t)+\sigma\sqrt{T-t}\,z}
\right)\phi(z)\,dz.
$$

Then $V(0,S_0)=x$, $V(T,s)=g(s)$, and the [Black-Scholes equation](../../../../../../black-scholes-equation.md) holds. Differentiation under the integral gives the delta

$$
\partial_sV(t,s)=e^{-r\tau}
\mathbb E\left[
g'(se^{(r-\sigma^2/2)\tau+\sigma\sqrt\tau Z})
e^{(r-\sigma^2/2)\tau+\sigma\sqrt\tau Z}
\right],
\qquad \tau=T-t.
$$

A Gaussian shift $Z\mapsto Z+\sigma\sqrt\tau$ rewrites this as

$$
\partial_sV(t,s)=
\int_{\mathbb R}
g'(se^{(r+\sigma^2/2)\tau+\sigma\sqrt\tau z})\phi(z)\,dz,
$$

which is exactly the stated $\theta_t$ at $s=S_t$.

Apply [Itô formula](../../../../../../ito-s-lemma.md) to $V(t,S_t)$. The PDE gives

$$
dV(t,S_t)=r\{V-\theta_tS_t\}\,dt+\theta_t\,dS_t.
$$

This is the same wealth equation as part a, with the same initial value $x$. Uniqueness therefore gives $X_t^{x,\theta}=V(t,S_t)$ and hence

$$
\boxed{X_T^{x,\theta}=V(T,S_T)=g(S_T).}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 211](../../../paper-211-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
