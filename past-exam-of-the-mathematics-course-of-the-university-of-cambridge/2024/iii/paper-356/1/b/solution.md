<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For a function $h$ on the copy-number state space, define the shift operator

$$
(E_i^kh)(x_1,\ldots,x_i,\ldots,x_4)
=h(x_1,\ldots,x_i+k,\ldots,x_4).
$$

With the propensities from part (a), the [forward operator of a Markov jump process](../../../../../../forward-operator-of-a-markov-jump-process.md) is

$$
\boxed{\begin{aligned}
\mathcal L^*p={}&(E_1^2-1)(a_1p)
+(E_2^{-1}-1)(a_2p)
+(E_2^1-1)(a_3p)\\
&+(E_3^{-1}-1)(a_4p)
+(E_3^1E_4^1-1)(a_5p)
+(E_4^{-1}-1)(a_6p)
+(E_2^1-1)(a_7p).
\end{aligned}}
$$

Equivalently, the [chemical master equation](../../../../../../chemical-master-equation.md) has the gain-minus-loss form

$$
(\mathcal L^*p)(\mathbf x)
=\sum_{r=1}^7
\left[a_r(\mathbf x-\nu_r)p(\mathbf x-\nu_r)
-a_r(\mathbf x)p(\mathbf x)\right],
$$

where terms outside the state space vanish.

The adjoint [Markov jump-process generator](../../../../../../markov-jump-process-generator.md) acts on observables:

$$
\boxed{(\mathcal Lf)(\mathbf x)
=\sum_{r=1}^7a_r(\mathbf x)
\left[f(\mathbf x+\nu_r)-f(\mathbf x)\right].}
$$

Indeed, shifting the summation index in the gain terms gives $\langle f,\mathcal L^*p\rangle=\langle\mathcal Lf,p\rangle$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 356](../../../paper-356-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
