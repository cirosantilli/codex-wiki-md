<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

First assume global [four-dimensional N=1 supersymmetry](../../../../../four-dimensional-n-1-supersymmetry.md), canonical positive [Kähler potential](../../../../../kahler-potential.md), and tree level. Write $W_i=\partial_i W$ and $m_{ij}=W_{ij}$ at the stationary vacuum. The [chiral-superfield fermion mass matrix](../../../../../chiral-superfield-fermion-mass-matrix.md) is the symmetric matrix $m$, and the sum of squared [Weyl spinor](../../../../../weyl-spinor.md) masses is $\operatorname{tr}(m^\dagger m)$. From the [F-term scalar potential](../../../../../f-term-scalar-potential.md) $V=\sum_k|W_k|^2$, its mixed and holomorphic [Hessian matrix](../../../../../hessian-matrix.md) blocks are

$$
V_{i\bar j}=\sum_kW_{ki}\overline{W_{kj}},
\qquad V_{ij}=\sum_k\overline{W_k}W_{kij}.
$$

For canonically normalized real and imaginary parts of the [scalar fields](../../../../../scalar-field.md), the real [scalar mass matrix](../../../../../scalar-mass-matrix.md) has trace twice the mixed trace. Its holomorphic blocks can split the two real scalar masses but do not change their sum. Hence

$$
\sum_{a=1}^{2n}m_{B,a}^2=2\operatorname{tr}(m^\dagger m),
\qquad 2\sum_{r=1}^{n}m_{F,r}^2=2\operatorname{tr}(m^\dagger m).
$$

A [Weyl spinor](../../../../../weyl-spinor.md) has two spin states, so this proves the [tree-level supertrace mass sum rule](../../../../../tree-level-supertrace-mass-sum-rule.md),

$$
\boxed{\operatorname{STr}M^2=\sum_am_{B,a}^2-2\sum_rm_{F,r}^2=0}.
$$

The paper defines its supertrace with $(-1)^{2j+1}$, the negative of the conventional boson-minus-fermion [supertrace](../../../../../supertrace.md) used here. The asserted zero is the same in either convention. The result requires the stated canonical tree-level hypotheses; a noncanonical [Kähler metric](../../../../../kahler-metric.md), [supergravity](../../../../../supergravity.md), or radiative corrections can change the sum rule.

If vector multiplets are also present, the [gauge contributions to the F-term supertrace](../../../../../gauge-contributions-to-the-f-term-supertrace.md) cancel rather than being omitted. At $D_a=0$, define $C=\sum_a g_a^2\|T_av\|^2$ for the scalar expectation vector $v$. Differentiating $\tfrac12\sum_aD_a^2$ adds $2C$ to the real-scalar trace. The symmetric [gaugino](../../../../../gaugino.md)-matter mass matrix has off-diagonal entries $\sqrt2g_aT_av$, giving an extra $4C$ in its fermion squared-mass trace. The covariant scalar [kinetic term](../../../../../kinetic-term.md) gives vector squared-mass trace $2C$. Thus their contribution is $2C-2(4C)+3(2C)=0$. The gauge-theory result uses all spin states, including the vector weight three; it is not obtained by dropping massive gauge partners.

The [MSSM tree-level sfermion mass constraint](../../../../../mssm-tree-level-sfermion-mass-constraint.md) explains the phenomenological difficulty with direct visible-sector breaking. If [F-term](../../../../../f-term.md) breaking is neutral under an unbroken electric and color [gauge symmetry](../../../../../gauge-invariance.md), and no [D-term](../../../../../d-term.md) shifts are present, the same trace argument applies within each conserved-charge fermion block. Its corresponding scalar partners cannot all have squared masses above the mean of the light fermion squared masses. Thus canonical tree-level visible-sector [supersymmetry breaking](../../../../../supersymmetry-breaking.md) alone cannot make every [squark](../../../../../squark.md) and other scalar partner heavy while leaving the observed fermions light. The usual effective [soft supersymmetry breaking](../../../../../soft-supersymmetry-breaking.md) terms arise after communicating breaking from a separate sector; integrating out that sector, noncanonical interactions and radiative effects evade the hypotheses. The global trace identity alone would not identify a particular light [squark](../../../../../squark.md) without the conserved-charge block argument.

For the specified [O'Raifeartaigh model](../../../../../o-raifeartaigh-model.md), phases may be chosen so that $\lambda,\mu,M$ are real and positive. Its [superpotential](../../../../../superpotential.md) derivatives are

$$
W_X=\lambda(z^2-\mu^2),\qquad W_Y=Mz,\qquad W_Z=2\lambda xz+My,
$$

and its [F-term scalar potential](../../../../../f-term-scalar-potential.md) is

$$
V=\lambda^2|z^2-\mu^2|^2+M^2|z|^2+|2\lambda xz+My|^2.
$$

For fixed $x,z$, choose $y=-2\lambda xz/M$ to minimize the final square. Since $|z^2-\mu^2|^2\ge(|z|^2-\mu^2)^2$,

$$
V\ge\lambda^2\mu^4+(M^2-2\lambda^2\mu^2)|z|^2+\lambda^2|z|^4.
$$

Thus **$M^2>2\lambda^2\mu^2$** makes $z=y=0$ a global minimum with arbitrary $x$. The hierarchy $M\gg\mu$ ensures this for fixed perturbative $\lambda$, rather than for arbitrarily large $\lambda$. The origin is one member of this classically flat family, with $V_0=\lambda^2\mu^4>0$ and $F_X=\lambda\mu^2$. The complex field $x$ is a [pseudomodulus](../../../../../pseudomodulus.md).

At the origin the [chiral-superfield fermion mass matrix](../../../../../chiral-superfield-fermion-mass-matrix.md), in the $(\psi_X,\psi_Y,\psi_Z)$ basis, is

$$
m=\begin{pmatrix}0&0&0\\0&0&M\\0&M&0\end{pmatrix}.
$$

Its physical fermion masses are **$0,M,M$**; the two massive [Weyl spinors](../../../../../weyl-spinor.md) form one massive four-component fermion. The massless $\psi_X$ is the [goldstino](../../../../../goldstino.md). More generally, stationarity gives $W_{ij}\overline{W_j}=0$, so the nonzero [auxiliary field](../../../../../auxiliary-field.md) direction is a null vector of $m$, proving the [goldstino zero mode from vacuum stationarity](../../../../../goldstino-zero-mode-from-vacuum-stationarity.md).

Writing $z=(z_R+iz_I)/\sqrt2$ and similarly for $x,y$, the quadratic [scalar potential](../../../../../scalar-potential.md) is

$$
V^{(2)}=M^2|y|^2+M^2|z|^2-\lambda^2\mu^2(z^2+\bar z^2).
$$

The [mass spectrum of the quadratic-cubic O'Raifeartaigh model](../../../../../mass-spectrum-of-the-quadratic-cubic-o-raifeartaigh-model.md) is therefore

$$
\boxed{\begin{array}{c|c}
\text{real scalar}&m^2\\\hline
x_R,x_I&0,0\\
y_R,y_I&M^2,M^2\\
z_R,z_I&M^2-2\lambda^2\mu^2,\ M^2+2\lambda^2\mu^2
\end{array}}.
$$

The scalar squared-mass sum is $4M^2$, while twice the fermion squared-mass sum is also $4M^2$, so **the supertrace is zero**, as required. The two massless real $x$ modes are tree-level [pseudomoduli](../../../../../pseudomodulus.md), which can be lifted by a quantum effective potential; their tree-level masslessness is not the exact symmetry protection enjoyed by the [goldstino](../../../../../goldstino.md).

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 307](../../paper-307-split.md)
3. [Iii](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
