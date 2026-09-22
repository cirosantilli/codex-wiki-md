<h1 id="b/6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

For classical events, $A\setminus C\subset(A\setminus B)\cup(B\setminus C)$: an outcome in $A$ but not in $C$ either fails $B$ or belongs to $B\setminus C$. [Monotonicity](../../../../monotonic-function.md) and the [union bound](../../../../boole-s-inequality.md) prove the [Fréchet-Bell inequality](../../../../frechet-bell-inequality.md)

$$
P(A\setminus C)\leq P(A\setminus B)+P(B\setminus C).
$$

[Malus' law](../../../../malus-law.md) gives transmission $\cos^2\gamma$ for a photon polarized by the first filter, so its conditional rejection [probability](../../../../probability.md) at the second is $\boxed{\sin^2\gamma}$. Conditional and joint probabilities must be distinguished: $P(A\setminus B)=P(A)P(B^c\mid A)$.

For equal unbiased marginals $P(A)=P(B)=1/2$, the quantum two-setting rejection probabilities are $\tfrac12\sin^2(\theta_A-\theta_B)$. A classical common assignment of all three outcomes would therefore require $\sin^2(\theta_A-\theta_B)+\sin^2(\theta_B-\theta_C)\geq\sin^2(\theta_A-\theta_C)$. Choose directions $0,\gamma,2\gamma$. Then

$$
\boxed{2\sin^2\gamma<\sin^2(2\gamma)\quad\text{when }0<\gamma<\pi/4.}
$$

For example $\gamma=\pi/6$ gives $1/2<3/4$. More generally $\sin^2a+\sin^2b-\sin^2(a+b)=-2\sin a\sin b\cos(a+b)$. In a triangle whose side directions are these filters, the internal angle supplementary to $a+b$ is obtuse exactly in this violation range. This specifies the angle convention behind the triangle description: with polarization axes regarded as unoriented lines, a claim that every sufficiently large physical axis separation violates the inequality would not be correct. The contradiction concerns a single classical joint model for all settings, not the validity of ordinary [probability](../../../../probability.md) or a comparison of arbitrarily renormalized sequential experiments.

Use $|0\rangle=|\alpha_0\rangle$ and $|1\rangle=|\alpha_1\rangle$. Projecting the first photon with $|0\rangle\langle0|$ gives the unnormalized product vector $c_0|00\rangle$, with success [probability](../../../../probability.md) $|c_0|^2$. [Projection](../../../../projection-linear-algebra.md) of the second onto $|\theta\rangle=\cos\theta|0\rangle+\sin\theta|1\rangle$ gives

$$
\boxed{c_0\cos\theta\,|0\rangle|\theta\rangle,\qquad P(\text{both transmissions})=|c_0|^2\cos^2\theta.}
$$

Conditioned on success, normalize these vectors; a zero amplitude means that outcome never occurs. For the maximally [entangled](../../../../entangled-state.md) equal-amplitude pair, rotation of both real polarization bases gives the same correlations for arbitrary settings. Comparing the appropriately normalized coincidence/rejection frequencies at three setting pairs tests the inequality above. A general unequal-amplitude state need not reproduce the unbiased rotationally invariant probabilities, so the maximally [entangled](../../../../entangled-state.md) choice supplies the clean explicit example.

For swapping, label the four systems in order $\xi_1,\eta_1,\xi_2,\eta_2$ and let $|\Phi\rangle_\eta=2^{-1/2}\sum_{j=0}^1|\eta_j\eta_j\rangle$. Its overlap with $|\eta_r\eta_s\rangle$ is $\delta_{rs}/\sqrt2$. Applying its rank-one [projector](../../../../projection-linear-algebra.md) to Alice's two systems gives

$$
\boxed{\frac12\sum_{r,k}b_r^2|\xi_r\rangle|\eta_k\rangle|\xi_r\rangle|\eta_k\rangle.}
$$

After regrouping the remote and local systems, this factorizes into $[\sum_rb_r^2|\xi_r\xi_r\rangle/\sqrt2]\otimes|\Phi\rangle_\eta$. The selected outcome has [probability](../../../../probability.md) $p=\tfrac12\sum_r|b_r|^4$. Therefore the normalized conditional remote state is

$$
\boxed{|\chi\rangle_\xi=\frac{\sum_rb_r^2|\xi_r\xi_r\rangle}{\sqrt{\sum_r|b_r|^4}}.}
$$

It has [Schmidt rank](../../../../schmidt-rank.md) at least two whenever the original pair was [entangled](../../../../entangled-state.md), since squaring a nonzero coefficient does not make it zero. Thus the two photons that never interacted become [entangled](../../../../entangled-state.md) **conditional on Alice's joint measurement outcome**. This is [entanglement swapping](../../../../entanglement-swapping.md). Alice is projecting onto a specified [Bell state](../../../../bell-state-split.md), not performing a universal test of whether an arbitrary unknown state is [entangled](../../../../entangled-state.md). Averaging all her outcomes leaves the remote [reduced density operator](../../../../reduced-density-matrix.md) unchanged, so no faster-than-light signal is available without her classical outcome label.

## ↑ Ancestors (12)

1. [6](../6.md)
2. [B](../../b.md)
3. [2009](../../../2009-split.md)
4. [Past exam of the quantum mechanics quantum theory and quantum computers course of the University of Oxford](../../../split.md)
5. [Quantum mechanics quantum theory and quantum computers course of the University of Oxford](../../../../quantum-mechanics-quantum-theory-and-quantum-computers-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
