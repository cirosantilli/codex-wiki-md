<h1 id="2/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Since $n=1+W$ with small variance,

$$
V=k_0^2(2W+W^2)
=2k_0^2W+O(W^2).
$$

To leading order, $V$ is therefore a centered [stationary Gaussian random field](../../../../../../stationary-gaussian-random-field.md). Let its [autocorrelation function of a random field](../../../../../../autocorrelation-function-of-a-random-field.md) be

$$
C_V(\mathbf s)
=\left\langle
V(\mathbf r')V(\mathbf r'+\mathbf s)
\right\rangle.
$$

The $W^2$ contribution gives higher-order mean and non-Gaussian corrections and is consistently omitted at this order.

The far-field [Rytov approximation](../../../../../../rytov-approximation.md) from part ii has unit incident intensity and

$$
I(\mathbf r)
=\left\langle
e^{\phi_1+\phi_1^*}
\right\rangle,
\qquad
\phi_1=a\widetilde V(\mathbf q).
$$

The real random variable $X=\phi_1+\phi_1^*$ is centered Gaussian. Its [moment-generating function](../../../../../../moment-generating-function.md) gives

$$
I=\exp\left(\frac12\langle X^2\rangle\right).
$$

Define

$$
J_-(\mathbf q)
=\int_D\int_D
C_V(\mathbf r_1-\mathbf r_2)
e^{-i\mathbf q\cdot(\mathbf r_1-\mathbf r_2)}
\,d^3r_1d^3r_2,
$$



$$
J_+(\mathbf q)
=\int_D\int_D
C_V(\mathbf r_1-\mathbf r_2)
e^{-i\mathbf q\cdot(\mathbf r_1+\mathbf r_2)}
\,d^3r_1d^3r_2.
$$

Then

$$
\langle|\phi_1|^2\rangle=|a|^2J_-,
\qquad
\langle\phi_1^2\rangle=a^2J_+,
$$

and hence

$$
\boxed{
I(\mathbf r)
=\exp\left\{
|a(\mathbf r)|^2J_-(\mathbf q)
+\operatorname{Re}
\left[a(\mathbf r)^2J_+(\mathbf q)\right]
\right\}}.
$$

This expression depends only on the two-point autocorrelation of the [scattering potential](../../../../../../scattering-potential.md). In the weak-fluctuation expansion it becomes

$$
\boxed{I=1+|a|^2J_-
+\operatorname{Re}(a^2J_+)
+O(C_V^2).}
$$

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [2](../../2.md)
3. [Paper 335](../../../paper-335-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
