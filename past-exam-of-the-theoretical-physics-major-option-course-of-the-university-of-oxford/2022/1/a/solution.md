<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For the [sawtooth Ising chain](../../../../sawtooth-ising-chain.md), there is a source inconsistency: the printed [Ising spin](../../../../ising-spin-variable.md) values are $\{-1,r+1\}$, with no definition of $r$. The requested [transfer matrix](../../../../transfer-matrix.md) follows for $r=0$, namely the usual [Ising model](../../../../ising-model.md) with values $\{-1,+1\}$. For arbitrary $r$, summing an apex [spin](../../../../spin.md) actually gives

$$
A^{(r)}_{ss'}=e^{-\beta Jss'}\left[e^{\beta\bar J(s+s')}+e^{-\beta\bar J(r+1)(s+s')}\right].
$$

For example, $r=1$, $s=s'=-1$ and $\beta\bar J=1$ give the bracket $e^{-2}+e^4$, whereas the claimed [hyperbolic cosine](../../../../hyperbolic-cosine.md) gives $e^{-2}+e^2$. Thus the printed identity is false literally. The rest of Question 1 uses the intended symmetric [Ising spin](../../../../ising-spin-variable.md) values, $r=0$.

For a fixed configuration of base [spins](../../../../spin.md), each apex [spin](../../../../spin.md) appears in only one local [Boltzmann factor](../../../../boltzmann-factor.md). The apex [spins](../../../../spin.md) are therefore conditionally independent, and their finite sums factorize:

$$
\begin{aligned}
Z&=\sum_{s_0,\ldots,s_{L-1}=\pm1}\prod_{i=0}^{L-1}\left[e^{-\beta Js_is_{i+1}}\sum_{\bar s_i=\pm1}e^{-\beta\bar J\bar s_i(s_i+s_{i+1})}\right]\\
&=\sum_{s_0,\ldots,s_{L-1}=\pm1}\prod_i A_{s_i s_{i+1}},\qquad s_L=s_0,\\
&\boxed{A_{ss'}=2e^{-\beta Jss'}\cosh[\beta\bar J(s+s')],\qquad Z=\operatorname{Tr}A^L.}
\end{aligned}
$$

Only the base [spins](../../../../spin.md) carry information from one triangle to the next. The apex [spins](../../../../spin.md) have already been summed out, so no apex index remains in the [transfer matrix](../../../../transfer-matrix.md); the final [trace](../../../../matrix-trace.md) implements the [periodic boundary condition](../../../../periodic-boundary-conditions.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the theoretical physics major option course of the University of Oxford](../../../split.md)
5. [Theoretical physics major option course of the University of Oxford](../../../../theoretical-physics-major-option-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
