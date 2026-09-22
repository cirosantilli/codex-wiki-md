<h1 id="7/solution">Solution</h1>

↑ **Parent:** [7](../7.md)

Suppose a semidiscrete linear PDE is $u_t=(A+B)u$. Direct evaluation of $e^{h(A+B)}$ may be expensive, while $e^{hA}$ and $e^{hB}$ can be cheap, parallelizable, or exactly structure-preserving. Splitting is especially effective when $A$ and $B$ represent different spatial directions, kinetic and potential energy, diffusion and reaction, or linear and nonlinear pieces.

The [Lie-Trotter splitting commutator error](../../../../../lie-trotter-splitting-commutator-error.md) follows from multiplying the exponential series:

$$
e^{hA}e^{hB}
=e^{h(A+B)}+\frac{h^2}{2}[A,B]+O(h^3).
$$

It therefore has local error $O(h^2)$ and global order one. Reversing the factors changes the sign of the leading commutator. The symmetric average in composition form is [Strang splitting](../../../../../strang-splitting.md),

$$
S_h=e^{hA/2}e^{hB}e^{hA/2},
$$

whose symmetry $S_{-h}=S_h^{-1}$ removes even powers from the modified generator. Its local error is $O(h^3)$, involving nested commutators such as $[A,[A,B]]$ and $[B,[A,B]]$, and its global order is two.

For multidimensional diffusion, directional splitting replaces one large elliptic solve by successive one-dimensional tridiagonal solves; alternating-direction implicit methods are standard examples. For the [Schrödinger equation](../../../../../schrodinger-equation.md), take $A=i\partial_x^2$ and $B=-iV(x)$. The kinetic subflow is diagonal in Fourier space, the potential subflow is pointwise multiplication, and Strang splitting is both second order and exactly norm-preserving.

A symmetric method has even global order. If its leading modified-flow defect is $h^{2p+1}E$, a symmetric composition $S_{a_1h}\cdots S_{a_sh}$ raises the order when $\sum a_i=1$ and $\sum a_i^{2p+1}=0$, together with the required higher commutator conditions. In particular, the [higher-order composition of a symmetric splitting](../../../../../higher-order-composition-of-a-symmetric-splitting.md)

$$
S_{\gamma h}S_{\delta h}S_{\gamma h},
\qquad
\gamma=\frac1{2-2^{1/3}},
\qquad
\delta=-\frac{2^{1/3}}{2-2^{1/3}},
$$

is fourth order because $2\gamma+\delta=1$ and $2\gamma^3+\delta^3=0$. Its negative middle step is harmless for reversible unitary problems but can be ill-posed or strongly unstable for parabolic semigroups. Higher-order parabolic splittings therefore use more specialized complex coefficients, commutator corrections, or extrapolation.

## ↑ Ancestors (10)

1. [7](../7.md)
2. [Paper 341](../../paper-341-split.md)
3. [Iii](../../split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
