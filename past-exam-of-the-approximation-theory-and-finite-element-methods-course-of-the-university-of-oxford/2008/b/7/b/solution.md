<h1 id="b/7/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $p_*=\min p>0$, $q_*=\min q>0$, $q^*=\max q$, and $P_1=\|p'\|_\infty$. Testing the dual equation with $z$ gives

$$
p_*\|z'\|_2^2+q_*\|z\|_2^2\leq\|e\|_2\|z\|_2.
$$

Consequently $\|z\|_2\leq\|e\|_2/q_*$ and $\|z'\|_2\leq\|e\|_2/\sqrt{p_*q_*}$. From $pz''=qz-e-p'z'$,

$$
\|z''\|_2\leq C_{\rm reg}\|e\|_2,\qquad
C_{\rm reg}=\frac1{p_*}\left(1+\frac{q^*}{q_*}
+\frac{P_1}{\sqrt{p_*q_*}}\right).
$$

On an element of length $h_i$, the [interpolation](../../../../../interpolation-split.md) error vanishes at both endpoints and its [derivative](../../../../../derivative.md) has zero mean. Two [Poincaré inequalities](../../../../../poincare-inequality.md) give

$$
\|z-I_hz\|_{L^2(I_i)}
\leq\frac{h_i^2}{\pi^2}\|z''\|_{L^2(I_i)}.
$$

Apply [Cauchy-Schwarz](../../../../../cauchy-schwarz-inequality.md) to the residual identity, with factors $h_i^2$ and $h_i^{-2}$:

$$
\|e\|_2^2\leq\frac1{\pi^2}
\left(\sum_ih_i^4\|R_h\|_{L^2(I_i)}^2\right)^{1/2}\|z''\|_2.
$$

If the error is nonzero, cancel its [norm](../../../../../norm.md) after the regularity estimate; if it is zero the conclusion is immediate. One explicit reliable constant is

$$
\boxed{C=\frac1{\pi^2p_*}
\left(1+\frac{q^*}{q_*}
+\frac{\|p'\|_\infty}{\sqrt{p_*q_*}}\right).}
$$

This proves the requested dual residual bound entirely in terms of the coefficient [functions](../../../../../function-split.md).

## ↑ Ancestors (13)

1. [B](../b.md)
2. [7](../../7.md)
3. [B](../../../b.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the approximation theory and finite element methods course of the University of Oxford](../../../../split.md)
6. [Approximation theory and finite element methods course of the University of Oxford](../../../../../approximation-theory-and-finite-element-methods-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
