<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

At one loop, plot each inverse squared coupling $g_a^{-2}$ against $\log\mu$. The three Standard Model lines have slopes that do not pass through one common point. Above the superpartner threshold, additional scalar and fermion vacuum-polarization diagrams change the slopes: for example, an $SU(2)$ gauge-boson two-point function receives a loop from a left-handed Standard Model fermion doublet and an additional loop from its scalar superpartner, while the $SU(2)$ gauge multiplet adds a [gaugino](../../../../../gaugino.md) loop alongside the gauge-boson and ghost loops. With the [Minimal supersymmetric Standard Model](../../../../../minimal-supersymmetric-standard-model.md) field content, the three resulting straight lines meet to good accuracy. This is [supersymmetric gauge coupling unification](../../../../../supersymmetric-gauge-coupling-unification.md).

The differential equation

$$
\frac{dg_a}{d\log\mu}=\beta_ag_a^3
$$

implies

$$
\frac{d}{d\log\mu}g_a^{-2}=-2\beta_a.
$$

Hence

$$
\boxed{g_a^{-2}(\mu)=g_a^{-2}(\mu_0)
-2\beta_a\log\frac\mu{\mu_0}},
$$

or

$$
\boxed{g_a(\mu)=\frac{g_a(\mu_0)}
{\sqrt{1-2\beta_ag_a^2(\mu_0)\log(\mu/\mu_0)}}}.
$$

Let $L=\log(M_{GUT}/M_Z)$. Equality of $g_1$ and $g_2$ at the unification scale gives

$$
g_1^{-2}(M_Z)-2\beta_1L
=g_2^{-2}(M_Z)-2\beta_2L,
$$

so

$$
\boxed{M_{GUT}=M_Z\exp\!\left[
\frac{g_1^{-2}(M_Z)-g_2^{-2}(M_Z)}{2(\beta_1-\beta_2)}
\right]}.
$$

Similarly,

$$
g_3^{-2}(M_Z)-g_2^{-2}(M_Z)
=2(\beta_3-\beta_2)L,
$$

while

$$
g_2^{-2}(M_Z)-g_1^{-2}(M_Z)
=2(\beta_2-\beta_1)L.
$$

Eliminating $L$ yields

$$
\boxed{g_3^{-2}(M_Z)=g_2^{-2}(M_Z)
+A\left[g_2^{-2}(M_Z)-g_1^{-2}(M_Z)\right]},
$$

with

$$
\boxed{A=\frac{\beta_3-\beta_2}{\beta_2-\beta_1}}.
$$

For the GUT-normalized MSSM one-loop coefficients proportional to $(33/5,1,-3)$, this is $\boxed{A=5/7}$.

Current coupling measurements approximately satisfy this MSSM relation and point to $M_{GUT}$ of order $10^{16}$ GeV, much more accurately than nonsupersymmetric one-loop running. Exact equality is not expected because two-loop evolution and threshold corrections from split superpartner and GUT-scale masses shift the lines; the absence so far of directly observed superpartners also prevents the threshold spectrum from being fixed experimentally.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 307](../../paper-307-split.md)
3. [Iii](../../split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
