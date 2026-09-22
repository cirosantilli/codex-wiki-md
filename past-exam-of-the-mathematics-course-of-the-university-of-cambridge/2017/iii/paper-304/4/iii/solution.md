<h1 id="4/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Write $d=4-\epsilon$ and $C_A=C_2(G)$. The pole term is independent of $m$ and external momentum beyond the transverse tensor: $\int_0^1x(1-x)\,dx=1/6$, $\Gamma(\epsilon/2)=2/\epsilon+O(1)$ and $(\mu^2/\Delta)^{\epsilon/2}=1+O(\epsilon)$. The supplied gluon [self-energy](../../../../../../self-energy.md) insertion therefore has

$$
\Pi_{\mu\nu}^{ab}\big|_{\mathrm{pole}}=-\frac{8g^2C_A}{3\epsilon(4\pi)^2}\delta^{ab}(k^2\delta_{\mu\nu}-k_\mu k_\nu).
$$

Using the insertion convention $\Gamma^{(2)}_{AA}=\Gamma^{(2)}_{AA,0}-\Pi$, its cancellation requires the matter contribution $\delta Z_A=-8g^2C_A/[3\epsilon(4\pi)^2]$ to the background gauge-field kinetic factor. One can extract the coupling running from this gauge-invariant matter determinant using the [background gauge-field renormalization identity](../../../../../../background-gauge-field-renormalization-identity.md) $Z_gZ_A^{1/2}=1$. This is a background-field [Ward identity](../../../../../../ward-identity.md), not a claim that the ordinary quantum-gluon wave-function factor alone always determines the full coupling [renormalization](../../../../../../renormalization.md). For this one adjoint [Dirac spinor](../../../../../../dirac-spinor.md),

$$
g_0=\mu^{\epsilon/2}Z_gg=\mu^{\epsilon/2}\left[g+\frac{4C_A}{3\epsilon(4\pi)^2}g^3+O(g^5)\right].
$$

Differentiate at fixed $g_0$. If $a=4C_A/[3(4\pi)^2]$ and $\beta(g)=-\epsilon g/2+b g^3+O(g^5)$, the order-$g^3$ terms in $\mu\,dg_0/d\mu=0$ give $b=a$. Subtracting $-\gamma_E+\log4\pi$ as well as the pole in the [modified minimal subtraction scheme](../../../../../../modified-minimal-subtraction-scheme.md) does not change this one-loop coefficient. Thus the [adjoint Dirac contribution to the Yang-Mills beta function](../../../../../../adjoint-dirac-contribution-to-the-yang-mills-beta-function.md) is

$$
\boxed{\beta_{\mathrm{spinor}}(g)=+\frac{4C_A}{3(4\pi)^2}g^3+O(g^5)\quad(d=4).}
$$

This is screening. The [pure Yang-Mills one-loop beta function](../../../../../../pure-yang-mills-one-loop-beta-function.md) coefficient is $-11C_Ag^3/[3(4\pi)^2]$. With $N_D$ adjoint [Dirac spinors](../../../../../../dirac-spinor.md), the total [renormalization-group beta function](../../../../../../beta-function-physics.md) is consequently

$$
\boxed{\beta(g)=-\frac{C_A}{3(4\pi)^2}(11-4N_D)g^3+O(g^5).}
$$

For a non-Abelian simple factor $C_A>0$, vanishing of the nontrivial one-loop coefficient would require $N_D=11/4$. It cannot be a nonnegative integer, proving the [integer obstruction to one-loop marginality with adjoint Dirac fermions](../../../../../../integer-obstruction-to-one-loop-marginality-with-adjoint-dirac-fermions.md). For a product group the same argument applies to every non-Abelian factor; the statement concerns the beta-function coefficient, not the trivial fixed point $g=0$. The [modified minimal subtraction scheme](../../../../../../modified-minimal-subtraction-scheme.md) is mass independent, so a massive spinor has this ultraviolet contribution; decoupling below its mass instead requires effective-theory threshold matching.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [4](../../4.md)
3. [Paper 304](../../../paper-304-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
