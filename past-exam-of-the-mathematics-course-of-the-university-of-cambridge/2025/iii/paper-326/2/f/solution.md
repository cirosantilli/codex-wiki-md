<h1 id="2/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

The [total variation distance](../../../../../../total-variation-distance.md) is

$$
d_{\rm TV}(\mu,\nu)=\sup_{B\in\mathcal B(X)}|\mu(B)-\nu(B)|.
$$

The problem is a [well-posed Bayesian inverse problem in total variation](../../../../../../well-posed-bayesian-inverse-problem-in-total-variation.md) when every $v\in\mathbb R^N$ determines a unique posterior $\mu^v$ and

$$
v_n\to v\quad\Longrightarrow\quad
d_{\rm TV}(\mu^{v_n},\mu^v)\to0.
$$

The heat solution operator at positive time is bounded from $L^2[0,1]$ to $C[0,1]$, so the finite sensor map $G:X\to\mathbb R^N$ is bounded and continuous. Therefore $\Phi(u;v)$ is jointly continuous and $0<e^{-\Phi}\leq1$. The normalizer satisfies $0<Z(v)\leq1$. If $v_n\to v$, the [dominated convergence theorem](../../../../../../dominated-convergence-theorem.md) gives both

$$
Z(v_n)\to Z(v)
$$

and convergence in $L^1(\mu_0)$ of the normalized posterior densities. Since total variation is one half of this $L^1$ distance for absolutely continuous measures, $d_{\rm TV}(\mu^{v_n},\mu^v)\to0$. Existence, uniqueness, and continuous dependence all follow.

## ↑ Ancestors (11)

1. [F](../f.md)
2. [2](../../2.md)
3. [Paper 326](../../../paper-326-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
