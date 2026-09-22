<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

**Particle gauge fixing and BRST.** Put $C=(p^2+\mu^2)/2$. The classical [constraint](../../../../../constraint-mechanics.md) generates $\delta_\varepsilon x^m=\varepsilon p^m$, $\delta_\varepsilon p_m=0$, $\delta_\varepsilon e=\dot\varepsilon$. Consequently the variation of $e-\bar e$ along a gauge orbit is the operator $\partial_t$ on $\varepsilon$. A [path integral](../../../../../path-integral.md) restricted to that gauge must include its [Faddeev-Popov determinant](../../../../../faddeev-popov-determinant.md); anticommuting [FP ghosts](../../../../../faddeev-popov-ghost.md) represent the determinant, rather than its inverse. Constant gauge zero modes and any [proper-time modulus](../../../../../proper-time-modulus.md) must be treated separately, so the relevant determinant is $\det{}'\partial_t$.

A convenient [point-particle Faddeev–Popov ghost action](../../../../../point-particle-faddeev-popov-ghost-action.md) at $\bar e=1$ is

$$
\boxed{S=\int dt\left[\dot x\cdot p-C+i b\dot c\right].}
$$

The [FP ghost](../../../../../faddeev-popov-ghost.md) normalization has been chosen to give the [graded Poisson bracket](../../../../../graded-poisson-bracket.md) $\{b,c\}=-i$, with the bracket symmetric on two odd variables. The [particle BRST charge and Klein–Gordon constraint](../../../../../particle-brst-charge-and-klein-gordon-constraint.md) are

$$
Q=cC,\qquad\delta F=\{F,\Lambda Q\},
$$

where the odd constant parameter $\Lambda$ is placed on the left. The product $\Lambda Q$ is even. Accounting for the odd parameter in this convention gives

$$
\boxed{\delta x^m=\Lambda c p^m,\quad\delta p_m=0,\quad
\delta c=0,\quad\delta b=i\Lambda C.}
$$

These are canonical [BRST transformations](../../../../../brst-symmetry.md). Direct variation checks the sign: the bosonic kinetic term changes by $\Lambda(\dot c\,p^2+c\,p\cdot\dot p)$, while the [FP ghost](../../../../../faddeev-popov-ghost.md) term changes by $-\Lambda C\dot c$. Hence

$$
\delta\mathcal L=\frac d{dt}\left[\Lambda c(p^2-C)\right],
$$

and the action is invariant for the corresponding boundary conditions. The [BRST charge](../../../../../brst-charge.md) is conserved because $C$ commutes with the gauge-fixed [Hamiltonian](../../../../../hamiltonian.md) and $c$ is constant on the [FP ghost](../../../../../faddeev-popov-ghost.md) equation of motion.

Quantization gives $\{\widehat b,\widehat c\}_+=1$ and $\widehat c^2=0$. Since $C$ commutes with the [FP ghosts](../../../../../faddeev-popov-ghost.md),

$$
\boxed{\widehat Q^2=\widehat c^{\,2}\widehat C^{\,2}=0.}
$$

It generates the same variations by $\delta\widehat F=-i[\widehat F,\Lambda\widehat Q]$, with an ordinary commutator against the even generator. Represent $\widehat c$ by multiplication and $\widehat b$ by differentiation. On a ghost-number-zero wavefunction $\Psi(x)$, $\widehat Q\Psi=0$ is exactly $\widehat C\Psi=0$, namely

$$
\boxed{(-\Box+\mu^2)\Psi=0,}
$$

the [Klein-Gordon equation](../../../../../klein-gordon-equation.md) for the mostly-plus metric. The specified [FP ghost](../../../../../faddeev-popov-ghost.md) sector matters: for an unrestricted wavefunction $\Psi_0+c\Psi_1$, BRST closure only constrains $\Psi_0$, not every component independently. The complete physical prescription uses [BRST cohomology](../../../../../brst-cohomology.md), not an assertion that every vector in the entire ghost-extended kernel is a new Klein–Gordon particle.

**String oscillator algebra and [FP ghost](../../../../../faddeev-popov-ghost.md) Virasoro generators.** Use the same bosonic brackets as above and the odd brackets

$$
\{\alpha_k^m,\alpha_l^n\}_{\mathrm{PB}}=-ik\eta^{mn}\delta_{k+l,0},
\qquad\{b_k,c_l\}_{\mathrm{PB}}=-i\delta_{k+l,0}.
$$

Quantization turns them into

$$
\boxed{[\alpha_k^m,\alpha_l^n]=k\eta^{mn}\delta_{k+l,0},\qquad
\{b_k,c_l\}_+=\delta_{k+l,0},\qquad
\{b_k,b_l\}_+=\{c_k,c_l\}_+=0.}
$$

The $b,c$ here are [worldsheet ghost fields](../../../../../worldsheet-ghost-field.md), not the matter [fermion](../../../../../fermion.md) oscillators used in the NS question.

Contract $b_m$ with the two $c$ factors in the cubic [FP ghost](../../../../../faddeev-popov-ghost.md) term of the given BRST operator. The first contraction contributes $-\tfrac12\sum_q(m-q)c_{-q}b_{m+q}$ and the second contributes $+\tfrac12\sum_p(p-m)c_{-p}b_{p+m}$. Their sum is $\sum_q(q-m)c_{-q}b_{m+q}$. Reordering and [normal ordering](../../../../../normal-ordering.md) therefore give the [ghost oscillator Virasoro generators](../../../../../ghost-oscillator-virasoro-generators.md)

$$
\boxed{L_m=L_m^{(\alpha)}+L_m^{(\mathrm{gh})},\qquad
L_m^{(\alpha)}=\frac12\sum_k:\alpha_k\cdot\alpha_{m-k}:,
\quad L_m^{(\mathrm{gh})}=\sum_k(m-k):b_{m+k}c_{-k}: .}
$$

For $m\ne0$ these formulas have no additive ambiguity. At $m=0$, moving annihilators past creators produces infinite zero-point sums. Their regularized finite constant shifts $L_0$ and corresponds to a term proportional to $c_0$ in $Q$. The convention fixed below has a [ghost oscillator vacuum](../../../../../ghost-oscillator-vacuum.md) weight $-1$, or equivalently the usual intercept-one shift. Whether that shift is written outside the normally ordered sum or incorporated in its definition is a convention; it must not be omitted twice or counted twice. In the chosen oscillator convention this is explicitly

$$
L_0=\frac12\alpha_0^2+\sum_{k>0}\alpha_{-k}\cdot\alpha_k+\sum_{k>0}k(b_{-k}c_k+c_{-k}b_k)-1.
$$

Equivalently, the normally ordered [BRST charge](../../../../../brst-charge.md) contains the intercept term $-c_0$; the formal un-ordered operator in the question includes that choice only after its ordering prescription is fixed.

The oscillator brackets directly give

$$
[L_m,b_n]=(m-n)b_{m+n},\qquad
[L_m,c_n]=-(2m+n)c_{m+n}.
$$

If $Q^2=0$, then $[L_n,Q]=[\{b_n,Q\},Q]=[b_n,Q^2]=0$. The graded Jacobi identity now yields [Virasoro closure from BRST nilpotence](../../../../../virasoro-closure-from-brst-nilpotence.md):

$$
\begin{aligned}
[L_m,L_n]&=[\{b_m,Q\},L_n]\\
&=\{[b_m,L_n],Q\}+\{b_m,[Q,L_n]\}\\
&=(m-n)\{b_{m+n},Q\}=(m-n)L_{m+n}.
\end{aligned}
$$

In particular a central extension cannot remain in the total generators if the quantum [BRST charge](../../../../../brst-charge.md) is nilpotent.

**Low-level descendant calculation.** Let $|\Omega;p\rangle$ be the oscillator ground state, annihilated by $\alpha_{n>0}$, $b_{n\ge0}$ and $c_{n>0}$. All $L_{n>0}$ annihilate it. The nonzero-mode [FP ghost](../../../../../faddeev-popov-ghost.md) generators act as

$$
L_{-1}^{(\mathrm{gh})}|\Omega\rangle=-b_{-1}c_0|\Omega\rangle,
\qquad
L_{-2}^{(\mathrm{gh})}|\Omega\rangle
=-2b_{-2}c_0|\Omega\rangle-3b_{-1}c_{-1}|\Omega\rangle.
$$

For example $L_1(-b_{-1}c_0|\Omega\rangle)=-2b_0c_0|\Omega\rangle=-2|\Omega\rangle$. Similarly $L_2$ on the two level-two terms gives $-8|\Omega\rangle$ and $-9|\Omega\rangle$, hence $-17|\Omega\rangle$. These signs are essential: [FP ghosts](../../../../../faddeev-popov-ghost.md) have an indefinite pairing.

The matter generators create

$$
L_{-1}^{(\alpha)}|\Omega\rangle=\alpha_0\cdot\alpha_{-1}|\Omega\rangle,
\qquad
L_{-2}^{(\alpha)}|\Omega\rangle=
\left(\alpha_0\cdot\alpha_{-2}+\frac12\alpha_{-1}\cdot\alpha_{-1}\right)|\Omega\rangle.
$$

Contracting the level-one term with $L_1$ gives $\alpha_0^2$. At level two the first term gives $2\alpha_0^2$, and the double contraction of the second gives $D/2$; cross terms vanish because oscillator levels differ. Thus the normalized oscillator/Virasoro descendant coefficients, conventionally denoted by the requested norms, are

$$
\boxed{\|L_{-1}|\Omega\rangle\|^2_{\mathrm{osc}}=\alpha_0^2-2,\qquad
\|L_{-2}|\Omega\rangle\|^2_{\mathrm{osc}}=2\alpha_0^2+\frac D2-17.}
$$

Comparing the first with $[L_1,L_{-1}]=2L_0$ gives the oscillator highest weight

$$
\boxed{h_0=\frac12\alpha_0^2-1.}
$$

In this normalization the question's $\langle0|L_0|0\rangle$ is $h_0$. Comparing level two with $[L_2,L_{-2}]=4L_0$ gives

$$
2\alpha_0^2+\frac D2-17=4\left(\frac12\alpha_0^2-1\right),
\qquad\boxed{D=26.}
$$

This is the [bosonic-string critical dimension from ghost descendants](../../../../../bosonic-string-critical-dimension-from-ghost-descendants.md). It checks cancellation of the matter and [FP ghost](../../../../../faddeev-popov-ghost.md) Virasoro anomalies without replacing the [FP ghost](../../../../../faddeev-popov-ghost.md) calculation by a remembered central-charge value.

There is a necessary [ghost zero-mode pairing](../../../../../ghost-zero-mode-pairing.md) qualification to the word “norm”. If $b_0,c_0$ are Hermitian in the full [FP ghost](../../../../../faddeev-popov-ghost.md) space and $b_0|\Omega\rangle=0$, then

$$
\langle\Omega|\Omega\rangle
=\langle\Omega|\{b_0,c_0\}|\Omega\rangle=0.
$$

A bare full-ghost inner product cannot at the same time normalize this ket to one. [FP ghost](../../../../../faddeev-popov-ghost.md) zero modes need saturation in actual amplitudes. The above equations are the coefficients of $L_1L_{-1}|\Omega\rangle$ and $L_2L_{-2}|\Omega\rangle$, or the corresponding normalized contravariant Virasoro form. They are not positive-definite Hilbert norms. The algebraic coefficient calculation is sufficient for the requested critical-dimension argument and remains valid without that false normalization.

Finally, impose the stated ground-state conditions $Q|\Omega;p\rangle=b_0|\Omega;p\rangle=0$. They imply $L_0|\Omega;p\rangle=\{b_0,Q\}|\Omega;p\rangle=0$, so $h_0=0$ and

$$
\boxed{\alpha_0^2=2,\qquad p^2=\frac1{\alpha'},\qquad
M_{\mathrm{ground}}^2=-\frac1{\alpha'}.}
$$

This is the bosonic [tachyon](../../../../../tachyon.md). When using an [oscillator vacuum](../../../../../oscillator-vacuum.md) at arbitrary momentum to establish the coefficients, it need not already be BRST closed; demanding closure selects this ground-state mass shell. The two uses should not be confused.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 46](../../paper-46-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
