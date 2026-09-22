<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use an [assortatively mixed two-risk-group SIS model](../../../../../../assortatively-mixed-two-risk-group-sis-model.md) with equal per-person [recovery rate](../../../../../../recovery-rate.md) $\gamma$. Let $x,y$ be infectious proportions in groups of sizes $pN,(1-p)N$. Let $c_H\gg c_L$ be their fixed contact rates and $\tau$ the transmission [probability](../../../../../../probability.md) per contact. Suppose a small fixed fraction $\epsilon<1/2$ of high-risk contacts is with the low-risk group. [Contact reciprocity in a two-group epidemic](../../../../../../contact-reciprocity-in-a-two-group-epidemic.md) requires

$$
pNc_H\epsilon=(1-p)Nc_L\epsilon_L,
\qquad \epsilon_L=\frac{pc_H\epsilon}{(1-p)c_L}.
$$

For sufficiently small $p$, both groups make most contacts within their own group, and the total cross-group contacts are of order $pN$. Define $A=\tau c_H(1-\epsilon)$, $B=\tau c_H\epsilon$, $D=\tau c_L$ and $C(p)=Bp/(1-p)$. The [forces of infection](../../../../../../force-of-infection.md) give

$$
\boxed{\begin{aligned}
\dot x&=(1-x)(Ax+By)-\gamma x,\\
\dot y&=(1-y)[C(p)x+(D-C(p))y]-\gamma y.
\end{aligned}}
$$

Here $C(p)<D$ and $\epsilon_L<1/2$ hold in the small-$p$ regime. High-risk per-person cross contact is order one but its group size is order $p$; low-risk per-person cross contact is order $p$. These distinctions are needed to count each cross-group partnership consistently.

Linearize about the disease-free state. In infectious fractions the transmission [matrix](../../../../../../matrix.md) is

$$
M(p)=\begin{pmatrix}A&B\\C(p)&D-C(p)\end{pmatrix}.
$$

In infected-individual counts the [next-generation matrix](../../../../../../next-generation-matrix.md) is instead

$$
K=\frac1\gamma\begin{pmatrix}A&C(p)\\B&D-C(p)\end{pmatrix}.
$$

The count and fraction formulations are related by a diagonal change of coordinates, so their [eigenvalues](../../../../../../eigenvalue.md) coincide. The [basic reproduction number](../../../../../../basic-reproduction-number.md) is the [spectral radius](../../../../../../spectral-radius.md) $R_0=\rho(M)/\gamma$, not an average of the two group reproduction numbers. The larger real [eigenvalue](../../../../../../eigenvalue.md) is

$$
\lambda_+(p)=\frac{A+D-C(p)+\sqrt{[A-D+C(p)]^2+4BC(p)}}2.
$$

This model makes a particular reciprocal mixing convention explicit; different defensible contact laws can change the first-order coefficients.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 52](../../../paper-52-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
