<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a specified trajectory, the [nonconserved order-parameter dynamics](../../../../../../nonconserved-order-parameter-dynamics.md) equation determines the noise realization

$$
\mathbf f_F
=\dot{\mathbf p}
+\Gamma\frac{\delta F}{\delta\mathbf p}.
$$

The forward [Onsager--Machlup path probability for Model A dynamics](../../../../../../onsager-machlup-path-probability-for-model-a-dynamics.md) is therefore

$$
P_F[\mathbf p]
=N_F\exp\left[
-\frac1{2\sigma^2}
\int_{t_1}^{t_2}dt\int d\mathbf r\,
\left|
\dot{\mathbf p}
+\Gamma\frac{\delta F}{\delta\mathbf p}
\right|^2
\right].
$$

Assume the order-parameter field is even under [time-reversal symmetry](../../../../../../t-symmetry.md) and its free-energy functional is time-reversal invariant. The reversed path is

$$
\mathbf p^R(t)=\mathbf p(t_1+t_2-t).
$$

Its time derivative changes sign, so

$$
P_B[\mathbf p^R]
=N_B\exp\left[
-\frac1{2\sigma^2}
\int_{t_1}^{t_2}dt\int d\mathbf r\,
\left|
-\dot{\mathbf p}
+\Gamma\frac{\delta F}{\delta\mathbf p}
\right|^2
\right].
$$

For additive [Gaussian white noise](../../../../../../gaussian-white-noise.md), the trajectory-to-noise Jacobian is the same in the two directions. We assume it and all path-independent normalization factors are absorbed into equal constants $N_F=N_B$. A time-reversal-odd order parameter would require the corresponding parity transformation as well.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 344](../../../paper-344-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
