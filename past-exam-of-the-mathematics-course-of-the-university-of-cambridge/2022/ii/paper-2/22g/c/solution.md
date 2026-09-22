<h1 id="22g/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For $x=\sum_nx_ne_n$, [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) gives

$$
\|Tx\|
\leq\sum_n|x_n|\,\|Te_n\|
\leq\|x\|\left(\sum_n\|Te_n\|^2\right)^{1/2}.
$$

Thus every $T\in H(V,V)$ is bounded and  
$\|T\|\leq\|T\|_*$. The truncations

$$
T_Nx=\sum_{n\leq N}x_nTe_n
$$

have finite rank and satisfy

$$
\|T-T_N\|\leq
\left(\sum_{n>N}\|Te_n\|^2\right)^{1/2}\to0.
$$

Hence every such [Hilbert-Schmidt operator](../../../../../../hilbert-schmidt-operator.md) is compact.

Define

$$
\langle S,T\rangle_*=\sum_n\langle Se_n,Te_n\rangle.
$$

This is an inner product inducing $\|\cdot\|_*$. If $(T_j)$ is Cauchy in this norm, then each $T_je_n$ converges to some $y_n$, and the usual Fatou/tail argument gives  
$\sum_n\|y_n\|^2<\infty$ and  
$\sum_n\|T_je_n-y_n\|^2\to0$. Defining  
$Tx=\sum_nx_ny_n$ produces a bounded operator by the preceding estimate and gives  
$T_j\to T$ in $\|\cdot\|_*$. Thus $(H(V,V),\|\cdot\|_*)$ is a Hilbert space.

The norms are not equivalent in infinite dimension. The rank-$N$ orthogonal projection has

$$
\|P_N\|=1,\qquad \|P_N\|_*=\sqrt N.
$$

Although $\|T\|\leq\|T\|_*$, no uniform reverse inequality can hold.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [22G](../../22g.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
