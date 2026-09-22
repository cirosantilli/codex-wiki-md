<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use target-space signature $(-,+,+,+)$ and [conformal gauge](../../../../../conformal-gauge.md) $g_{ab}=e^{2\omega}\operatorname{diag}(-1,1)$. Dots and primes denote differentiation with respect to $\tau$ and $\sigma$. Varying the [Polyakov action](../../../../../polyakov-action.md) with respect to the [string embedding map](../../../../../string-embedding-map.md) gives the [wave equation](../../../../../wave-equation-split.md); varying the [worldsheet metric](../../../../../worldsheet-metric.md) sets the [worldsheet stress tensor](../../../../../worldsheet-stress-energy-tensor.md) to zero. Explicitly,

$$
\boxed{\ddot X^\mu-X^{\mu\prime\prime}=0,\qquad \dot X^2+X'^2=0,\qquad \dot X\cdot X'=0.}
$$

With $\sigma^\pm=\tau\pm\sigma$ and $\partial_\pm=\tfrac12(\partial_\tau\pm\partial_\sigma)$, the two [Virasoro constraints](../../../../../virasoro-constraint.md) are $(\partial_+X)^2=(\partial_-X)^2=0$.

A fixed spatial circle would sweep out a cylindrical [string worldsheet](../../../../../worldsheet.md). In static coordinates its [string embedding map](../../../../../string-embedding-map.md) is $X=(t,R\cos\theta,R\sin\theta,0)$ and its [induced worldsheet metric](../../../../../induced-worldsheet-metric.md) is $\operatorname{diag}(-1,R^2)$. The radial part of the [Nambu–Goto equations of motion](../../../../../nambu-goto-equations-of-motion.md) is proportional to $R^{-2}\partial_\theta^2(R\cos\theta,R\sin\theta)=-(\cos\theta,\sin\theta)/R$, which is nonzero. Thus a nonzero-radius cylinder cannot solve the equations. Motion of labels around this same cylinder is a [worldsheet diffeomorphism](../../../../../worldsheet-diffeomorphism.md) and cannot alter this conclusion.

The familiar [pulsating circular string](../../../../../pulsating-circular-string.md) makes the obstruction particularly explicit. Put $X^0=\kappa\tau$ and $X^1+iX^2=r(\tau)e^{i\sigma}$. The [wave equation](../../../../../wave-equation-split.md) and [Virasoro constraints](../../../../../virasoro-constraint.md) reduce to

$$
\ddot r+r=0,\qquad \dot r^2+r^2=\kappa^2.
$$

A constant $r=R\ne0$ violates the first equation. Even rotating the labels, $X^1+iX^2=Re^{i(\sigma+\Omega\tau)}$, cannot help: the [wave equation](../../../../../wave-equation-split.md) requires $\Omega^2=1$, whereas $\dot X\cdot X'=R^2\Omega$ requires $\Omega=0$.

Nor does a rigid rotation of the circular plane rescue the usual circular ansatz in three spatial dimensions. Write its spatial part as $A(\tau)\cos\sigma+B(\tau)\sin\sigma$, with $A^2=B^2=R^2$ and $A\cdot B=0$. The [wave equation](../../../../../wave-equation-split.md) gives $\ddot A=-A$ and $\ddot B=-B$. The constant norms give $A\cdot\dot A=B\cdot\dot B=0$ and $\dot A^2=\dot B^2=R^2$. The mixed [Virasoro constraint](../../../../../virasoro-constraint.md), together with the derivative of $A\cdot B=0$, gives $\dot A\cdot B=A\cdot\dot B=0$. Differentiating $A\cdot B$ twice gives $\dot A\cdot\dot B=0$. This would require four mutually orthogonal nonzero spatial vectors in $\mathbb R^3$. This obstruction is specific to the stated spatial dimension; a [rigid circular string in four spatial dimensions](../../../../../rigid-circular-string-in-four-spatial-dimensions.md) has more room.

To express the [Virasoro constraints](../../../../../virasoro-constraint.md) in modes, extend the [string oscillators](../../../../../string-oscillator.md) by

$$
\alpha_0^\mu=\widetilde\alpha_0^\mu=\sqrt{\frac{\alpha'}2}\,p^\mu.
$$

Differentiating the two chiral expansions gives $\partial_-X^\mu=\sqrt{\alpha'/2}\sum_n\alpha_n^\mu e^{-in\sigma^-}$ and the corresponding expression with tildes for $\partial_+X$. Equating every [Fourier coefficient](../../../../../fourier-coefficient.md) of their squares to zero yields

$$
L_m=\frac12\sum_{n\in\mathbb Z}\alpha_{m-n}\cdot\alpha_n=0,\qquad \widetilde L_m=\frac12\sum_{n\in\mathbb Z}\widetilde\alpha_{m-n}\cdot\widetilde\alpha_n=0\quad(m\in\mathbb Z).
$$

Reality of the [string embedding map](../../../../../string-embedding-map.md) means $\alpha_{-n}=\alpha_n^*$ and $\widetilde\alpha_{-n}=\widetilde\alpha_n^*$. In particular, define the classical [string level operators](../../../../../string-level-operator.md) by $N=\sum_{n>0}\alpha_{-n}\cdot\alpha_n$ and $\widetilde N=\sum_{n>0}\widetilde\alpha_{-n}\cdot\widetilde\alpha_n$. The zero-mode [Virasoro constraints](../../../../../virasoro-constraint.md) become

$$
0=L_0=\frac{\alpha'}4p^2+N,\qquad 0=\widetilde L_0=\frac{\alpha'}4p^2+\widetilde N.
$$

Consequently the classical [bosonic string mass spectrum](../../../../../bosonic-string-mass-spectrum.md) is

$$
\boxed{M^2=-p^2=\frac{4N}{\alpha'}=\frac{4\widetilde N}{\alpha'},\qquad N=\widetilde N.}
$$

The equality of the two levels is [closed-string level matching](../../../../../closed-string-level-matching.md). There is no [string intercept](../../../../../normal-ordering-constant-of-a-string.md) here: that shift comes from quantum [normal ordering](../../../../../normal-ordering.md), not from these classical equations.

For the [compact boson](../../../../../compact-boson.md), closed-string periodicity permits a winding number $w\in\mathbb Z$, so $X^3(\sigma+2\pi)-X^3(\sigma)=2\pi wR$. Let $q$ be the momentum in this direction. Its zero-mode expansion and the corresponding chiral momenta are

$$
X^3=x^3+\alpha' q\tau+wR\sigma+\text{oscillators},\qquad p_L^3=q+\frac{wR}{\alpha'},\qquad p_R^3=q-\frac{wR}{\alpha'}.
$$

Thus replace the equal left and right zero modes by $\widetilde\alpha_0^3=\sqrt{\alpha'/2}\,p_L^3$ and $\alpha_0^3=\sqrt{\alpha'/2}\,p_R^3$; the nonzero [string oscillators](../../../../../string-oscillator.md) remain integer-moded. Classically $q$ is continuous. Quantizing the [compact boson](../../../../../compact-boson.md) makes momentum wavefunctions single-valued around its circle, giving $q=n/R$ with $n\in\mathbb Z$.

If $k^a$, $a=0,1,2$, is the noncompact momentum and $M^2=-k^ak_a$, the two zero-mode [Virasoro constraints](../../../../../virasoro-constraint.md) give

$$
M^2=\left(q+\frac{wR}{\alpha'}\right)^2+\frac{4\widetilde N}{\alpha'}=\left(q-\frac{wR}{\alpha'}\right)^2+\frac{4N}{\alpha'}.
$$

Averaging and subtracting gives the [momentum and winding modes](../../../../../momentum-and-winding-modes.md) and [compact-circle closed-string level matching](../../../../../compact-circle-closed-string-level-matching.md) formulas

$$
\boxed{M^2=q^2+\frac{w^2R^2}{\alpha'^2}+\frac{2(N+\widetilde N)}{\alpha'},\qquad \widetilde N-N+qwR=0.}
$$

The latter becomes $\widetilde N-N+nw=0$ on imposing quantum momentum quantization. The sign follows from assigning tildes to the left mover $\sigma^+$.

An explicit [winding-supported circular string](../../../../../winding-supported-circular-string.md), valid classically for every $R>0$, is

$$
\boxed{X^0=2R\tau,\quad X^1=R\cos(\sigma+\tau),\quad X^2=R\sin(\sigma+\tau),\quad X^3=R(\sigma-\tau)\pmod{2\pi R}.}
$$

The noncompact projection is a circle of constant radius. Every coordinate obeys the [wave equation](../../../../../wave-equation-split.md). Its compact winding is $w=1$, and a direct calculation gives

$$
\dot X^2=-2R^2,\qquad X'^2=2R^2,\qquad \dot X\cdot X'=R^2-R^2=0.
$$

Thus both [Virasoro constraints](../../../../../virasoro-constraint.md) hold and the [induced worldsheet metric](../../../../../induced-worldsheet-metric.md) is $2R^2\operatorname{diag}(-1,1)$, not a degenerate cylinder. The compact motion cancels the mixed stress that spoiled rotation of labels in flat space. Here $q=-R/\alpha'$, $N=0$ and $\widetilde N=R^2/\alpha'$ satisfy the classical [compact-circle closed-string level matching](../../../../../compact-circle-closed-string-level-matching.md) condition. Requiring this particular classical momentum to equal an individual quantum eigenvalue would impose an additional radius-dependent condition; that is not required to construct the classical solution.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 44](../../paper-44-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
