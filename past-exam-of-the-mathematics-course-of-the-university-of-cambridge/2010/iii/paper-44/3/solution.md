<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Locally in the space of [worldsheet metrics](../../../../../worldsheet-metric.md), divide out the volume of [worldsheet diffeomorphisms](../../../../../worldsheet-diffeomorphism.md) and [Weyl transformations](../../../../../weyl-transformation.md). With stabilizer zero modes omitted, the inverse [Faddeev-Popov determinant](../../../../../faddeev-popov-determinant.md) at a metric $g$ is

$$
\boxed{\Delta_{\rm FP}^{-1}[g]=\int D\omega\,Dv\ \delta\!\left[2\omega g_{ab}+\nabla_a v_b+\nabla_b v_a\right].}
$$

This is the linearized orbit integral: the delta functional is the product of the metric-component delta functions, and its Jacobian is the inverse determinant of the gauge-orbit map. The omitted zero modes and any metric moduli must be handled separately; this local formula is not an integration over the physical moduli themselves.

The [trace elimination in string Faddeev-Popov gauge fixing](../../../../../trace-elimination-in-string-faddeev-popov-gauge-fixing.md) is essential. In two dimensions, split the variation as

$$
\delta g_{ab}=(2\omega+\nabla\cdot v)g_{ab}+(P_1v)_{ab},\qquad (P_1v)_{ab}=\nabla_av_b+\nabla_bv_a-g_{ab}\nabla\cdot v.
$$

The second term is trace-free. Integration over $\omega$ removes the trace delta function, leaving $\int Dv\,\delta[P_1v]=(\det{}'P_1)^{-1}$, with the measure understood through the metric inner products. Equivalently, a Fourier representation of the metric delta functional introduces a commuting symmetric tensor $\beta^{ab}$. Integration over $\omega$ enforces $g_{ab}\beta^{ab}=0$, and the remaining exponent is proportional to $\int\sqrt g\,\beta^{ab}(P_1v)_{ab}$. This gives the same inverse [Faddeev-Popov determinant](../../../../../faddeev-popov-determinant.md) and explains why its tensor variable must be trace-free.

For the [Polyakov path integral](../../../../../polyakov-path-integral.md), insert the gauge-fixing identity

$$
1=\Delta_{\rm FP}[g]\int D\omega\,Dv\ \delta[g^{\omega,v}-\widehat g(m)],
$$

where $\widehat g(m)$ is a representative depending on the [worldsheet moduli](../../../../../worldsheet-moduli.md) $m$. Gauge invariance of the action, measure, and [Faddeev-Popov determinant](../../../../../faddeev-popov-determinant.md) lets us change variables along the gauge orbit. Its volume cancels the original gauge-group denominator, leaving an integral over $X$, the moduli, and the determinant evaluated at $\widehat g$. This is how the determinant enters the numerator of the gauge-fixed integral, despite the inverse determinant occurring in the orbit integral above.

A [fermionic Gaussian integral](../../../../../grassmann-gaussian-integral.md) exponentiates $\det{}'P_1$ using an anticommuting vector $c^a$ and an anticommuting symmetric trace-free tensor $b^{ab}$:

$$
\det{}'P_1\ \propto\ \int Db\,Dc\ \exp\!\left[-C\int d^2\sigma\sqrt g\,b^{ab}(P_1c)_{ab}\right].
$$

The constant $C$ can be absorbed into $b$. In local complex [conformal gauge](../../../../../conformal-gauge.md), trace-freeness sets $b_{z\bar z}=0$. The only surviving components of the [worldsheet diffeomorphism ghost operator](../../../../../worldsheet-diffeomorphism-ghost-operator.md) are proportional to $\bar\partial c^z$ and $\partial c^{\bar z}$. Rescaling the antighost therefore gives exactly the chiral [worldsheet ghost action](../../../../../worldsheet-ghost-action.md)

$$
\boxed{S_{\rm gh}=\int d^2z\left(b_{zz}\bar\partial c^z+b_{\bar z\bar z}\partial c^{\bar z}\right).}
$$

The chiral [bc ghost system](../../../../../bc-system.md) has weights $h_b=2$, $h_c=-1$, with $b(z)c(w)\sim1/(z-w)$. Its [worldsheet stress tensor](../../../../../worldsheet-stress-energy-tensor.md) is $T_{\rm gh}=-2:b\partial c:-:(\partial b)c:$. Fermionic double [Wick contractions](../../../../../wick-contraction.md) in $T_{\rm gh}T_{\rm gh}$ give the fourth-order coefficient $-13$, hence [central charge](../../../../../central-charge.md) $c_{\rm gh}=-26$. More generally this calculation gives $c=1-3(2h_b-1)^2$. Each embedding scalar contributes one, so the total chiral [central charge](../../../../../central-charge.md) is $D-26$. The gauge-fixed quantum theory must have no [worldsheet Weyl anomaly](../../../../../worldsheet-weyl-anomaly.md); consequently **the [critical dimension of the bosonic string](../../../../../critical-dimension-of-string-theory.md) is $D=26$**. Zero-mode insertions for [Conformal Killing vector fields](../../../../../conformal-killing-vector-field.md) and moduli do not change this local anomaly calculation.

For the [Veneziano amplitude](../../../../../veneziano-amplitude.md), first examine an ordered beta-function term. A pole occurs when $-\alpha's-1=-n$, with $n=0,1,2,\ldots$, so the exchanged masses follow the [open bosonic string mass spectrum](../../../../../open-bosonic-string-mass-spectrum.md)

$$
\boxed{M_n^2=\frac{n-1}{\alpha'},\qquad n=0,1,2,\ldots.}
$$

There is a tachyon at level zero, a massless vector at level one, then an infinite tower with equally spaced squared masses. In oscillator quantization these levels are $N=n$; the poles alone do not determine all oscillator degeneracies or all states that might fail to couple to the chosen external particles.

The [Veneziano amplitude pole residue](../../../../../veneziano-amplitude-pole-residue.md) gives considerably more information than a pole position. Near $s_n=(n-1)/\alpha'$, use $\Gamma(-n+\epsilon)\sim(-1)^n/(n!\epsilon)$ and $\epsilon=-\alpha'(s-s_n)$. The finite [gamma function](../../../../../gamma-function.md) ratio is a product of $n$ linear factors. Thus, for generic $t$,

$$
\operatorname*{Res}_{s=s_n}B(-\alpha's-1,-\alpha't-1)=-\frac1{\alpha'n!}\prod_{j=1}^{n}(\alpha't+j+1).
$$

The empty product at $n=0$ is one. This degree-$n$ angular polynomial decomposes into spin [partial waves](../../../../../partial-wave.md); it reveals the spins that couple, up to maximal spin $n$ in the ordered channel, and the corresponding products of three-point couplings. For example, the level-one linear residue encodes vector exchange. A single external-state amplitude need not separate all states with the same mass and spin.

There is a qualification specific to the sum printed in the question. For four identical on-shell tachyons, $s+t+u=-4/\alpha'$. At $\alpha's=n-1$, put $P_n(t)=\prod_{j=1}^n(\alpha't+j+1)$. Then $\alpha'u=-n-3-\alpha't$, and reversing the product gives $P_n(u)=(-1)^nP_n(t)$. The $t,u$ beta-function term is regular at a generic $s$-channel pole. The residue of the full symmetric amplitude is therefore proportional to

$$
-\frac{1+(-1)^n}{\alpha'n!}\,P_n(t).
$$

This is [odd-level pole cancellation in the symmetric Veneziano amplitude](../../../../../odd-level-pole-cancellation-in-the-symmetric-veneziano-amplitude.md). **The fully symmetrized identical-tachyon amplitude has only even-level poles at generic angle**, including the tachyon but not the massless vector. This is an external-state selection rule, not removal of odd-level states from the string theory. Ordered amplitudes, or suitable amplitudes with color factors and different external states, retain those exchanges. Thus interpreting every candidate [gamma function](../../../../../gamma-function.md) pole as a pole of the printed sum would give a false inference about that amplitude.

At high energy with $x=-t/s\in(0,1)$ fixed, the [gamma function](../../../../../gamma-function.md) reflection formula followed by the [Stirling formula](../../../../../stirling-formula.md) gives the [fixed-angle softness of an open-string amplitude](../../../../../fixed-angle-softness-of-an-open-string-amplitude.md):

$$
\log|A|=-\alpha's\left[-x\log x-(1-x)\log(1-x)\right]+O(\log s),
$$

up to oscillatory factors and possible additional cancellations. The bracket is positive at a genuinely nonforward fixed angle. This is the envelope away from resonance poles, or the corresponding analytically continued asymptotic regime; it is not a uniform bound through real-axis poles. **String scattering is exponentially soft at fixed angle**, unlike the typical power-law behavior of point-particle interactions. The finite string length distributes a hard collision over an extended object. This is evidence of improved ultraviolet behavior, not by itself a proof that every loop amplitude is finite. The fixed-angle limit also differs from the fixed-$t$ [Regge limit](../../../../../regge-limit.md).

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 44](../../paper-44-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
