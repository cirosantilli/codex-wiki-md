<h1 id="1/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The exchange graph has one quartic vertex attached to $\mathbf k_1,\mathbf k_2,\mathbf k_3$, a second attached to $\mathbf k_4,\mathbf k_5,\mathbf k_6$, and an internal line of momentum

$$
\mathbf k_I=\mathbf k_1+\mathbf k_2+\mathbf k_3
=-(\mathbf k_4+\mathbf k_5+\mathbf k_6).
$$

Schematically,

$$
(k_1,k_2,k_3)\longrightarrow\bullet
\mathbin{-}_{k_I}\bullet\longleftarrow(k_4,k_5,k_6).
$$

The [Schwinger-Keldysh conjugation relation](../../../../../../schwinger-keldysh-conjugation-relation.md) gives

$$
\boxed{B_6^{(LL)}=(B_6^{(RR)})^*,
\qquad B_6^{(RL)}=(B_6^{(LR)})^*}.
$$

Set $\eta_0=0$ only in integration limits and phases, retaining its leading explicit power from the six external propagators. The scale factors, six external propagators, and one internal propagator leave the common coefficient

$$
\mathcal P=\frac{\lambda^2H^6}
{2^7k_1k_2k_3k_4k_5k_6k_I}.
$$

For two right-branch vertices, split the time-ordered integral into $\eta_1>\eta_2$ and $\eta_2>\eta_1$:

$$
\int_{-\infty}^0d\eta_1d\eta_2,
e^{ik_L\eta_1+ik_R\eta_2-ik_I|\eta_1-\eta_2|}
=-\frac1{k_T}\left(\frac1{E_R}+\frac1{E_L}\right).
$$

The two right-vertex factors contribute the compensating minus sign, so

$$
\boxed{B_6^{(RR)}
=\mathcal P\eta_0^6\frac1{k_T}
\left(\frac1{E_R}+\frac1{E_L}\right)}.
$$

For one vertex on each branch, the two integrals factorize:

$$
\boxed{B_6^{(LR)}
=\mathcal P\eta_0^6\frac1{E_LE_R}}.
$$

Thus the quantities requested in the question are

$$
\boxed{A=B=\mathcal P}.
$$

At late time these expressions are real. Summing all four [in-in formalism](../../../../../../keldysh-formalism.md) assignments gives

$$
B_6=2(B_6^{(RR)}+B_6^{(LR)})
=\boxed{
\frac{\lambda^2H^6\eta_0^6}
{2^5k_1k_2k_3k_4k_5k_6k_I}
\frac{k_T+k_I}{k_TE_LE_R}}.
$$

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [1](../../1.md)
3. [Paper 312](../../../paper-312-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
