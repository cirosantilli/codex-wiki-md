<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the printed interaction, so the [Dyson series](../../../../../../dyson-series.md) contributes $-ig$ per vertex before its spinor matrix. The momentum-space [Feynman rules](../../../../../../feynman-rule.md) are

$$
\boxed{D_\phi(q)=\frac{i}{q^2-\mu^2+i0},\qquad
S_\psi(q)=\frac{i(\not q+m)}{q^2-m^2+i0},\qquad
V_{\phi\bar\psi\psi}=-ig\gamma^5.}
$$

Each [interaction vertex](../../../../../../interaction-vertex.md) has one pseudoscalar line and one incoming and one outgoing fermion-number line. Conserve [four-momentum](../../../../../../four-momentum.md) at every vertex, integrate each independent loop momentum with $d^4\ell/(2\pi)^4$, and divide by any [Feynman-diagram symmetry factor](../../../../../../feynman-diagram-symmetry-factor.md). A closed [fermion loop](../../../../../../fermion-loop.md) contributes an extra minus sign. The external wavefunctions are $u$ for incoming fermions, $\bar u$ for outgoing fermions, $\bar v$ for incoming antifermions and $v$ for outgoing antifermions; spinor matrices are multiplied in order along the fermion line. An external pseudoscalar has unit wavefunction factor in standard relativistic normalization. Relative [fermionic signs](../../../../../../fermionic-sign.md) also occur when the external contractions are permuted.

The leading scattering amplitudes are of order $g^2$. Label the incoming momenta $p_1,p_2$ and outgoing momenta $p_3,p_4$, all with positive energy and $p_i^2=m^2$. Use the [Mandelstam variables](../../../../../../mandelstam-variables.md) $s=(p_1+p_2)^2$, $t=(p_1-p_3)^2$ and $u=(p_1-p_4)^2$. The [tree scattering with pseudoscalar exchange](../../../../../../tree-scattering-with-pseudoscalar-exchange.md) is shown below; dashed edges are pseudoscalar propagators, and arrows indicate fermion-number flow, opposite to the motion of an antifermion.

<a id="3/b/image-the-two-pseudoscalar-exchange-tree-diagrams-for-fermion-fermion-scattering-and-the-exchange-and-annihilation-diagrams-for-fermion-antifermion-scattering"></a>
![](../../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-42-scattering.png)

**[Figure 1](#3/b/image-the-two-pseudoscalar-exchange-tree-diagrams-for-fermion-fermion-scattering-and-the-exchange-and-annihilation-diagrams-for-fermion-antifermion-scattering). The two pseudoscalar-exchange tree diagrams for fermion–fermion scattering and the exchange and annihilation diagrams for fermion–antifermion scattering**.

Define the [scattering amplitude](../../../../../../scattering-amplitude.md) by $\langle f|S-1|i\rangle=i(2\pi)^4\delta^4(p_3+p_4-p_1-p_2)\mathcal M$. Use standard relativistic normalization for external states and spinors. To fix even the overall signs, suppress the positive state-normalization factors and write the creator order of the two-fermion states as $|i\rangle=b_1^\dagger b_2^\dagger|0\rangle$, $|f\rangle=b_3^\dagger b_4^\dagger|0\rangle$, and the fermion-antifermion states as $|i\rangle=b_1^\dagger d_2^\dagger|0\rangle$, $|f\rangle=b_3^\dagger d_4^\dagger|0\rangle$. Spin labels on the $u_i,v_i$ are implicit.

For two fermions, the direct $t$ graph connects $1\to3$ and $2\to4$, while the exchanged $u$ graph connects $1\to4$ and $2\to3$. The [canonical anticommutation relations](../../../../../../canonical-anticommutation-relations.md) give signs $+$ and $-$ for these contractions in the chosen state order. Multiplication of the two vertices and the scalar propagator gives $(-ig)^2i=-ig^2$. Hence

$$
\boxed{\mathcal M_{\psi\psi}=-g^2\left[
\frac{(\bar u_3\gamma^5u_1)(\bar u_4\gamma^5u_2)}{t-\mu^2+i0}
-\frac{(\bar u_4\gamma^5u_1)(\bar u_3\gamma^5u_2)}{u-\mu^2+i0}
\right]+O(g^4).}
$$

Interchanging the labels of either pair of identical external fermions reverses this amplitude, as required for the antisymmetric states of [fermionic Fock space](../../../../../../fermionic-fock-space.md).

For a fermion and an antifermion, the graphs are $t$ exchange and $s$ annihilation. Their signs can be derived without guessing an analogy with the first process. The [normal-ordered product](../../../../../../normal-ordered-product.md) of the pseudoscalar bilinear contains terms of the forms

$$
b^\dagger b\,\bar u\gamma^5u,qquad
-d^\dagger d\,\bar v\gamma^5v,qquad
b^\dagger d^\dagger\,\bar u\gamma^5v,qquad
db\,\bar v\gamma^5u.
$$

The minus in the second term is the [antifermion sign of a normal-ordered bilinear](../../../../../../antifermion-sign-of-a-normal-ordered-bilinear.md). Between the chosen external states, exchange has sign $-$ and pair annihilation followed by pair creation has sign $+$. Therefore

$$
\boxed{\mathcal M_{\psi\bar\psi}=g^2\left[
\frac{(\bar u_3\gamma^5u_1)(\bar v_2\gamma^5v_4)}{t-\mu^2+i0}
-\frac{(\bar v_2\gamma^5u_1)(\bar u_3\gamma^5v_4)}{s-\mu^2+i0}
\right]+O(g^4).}
$$

Changing an external-state phase can change the common overall sign; it cannot change the relative minus between the two channels. Both amplitudes use the coefficient exactly as printed. For the Hermitian convention $g=i g_P$ discussed in part (a), substitute $g^2=-g_P^2$ throughout, or equivalently use vertex $g_P\gamma^5$ from the outset.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 42](../../../paper-42-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
