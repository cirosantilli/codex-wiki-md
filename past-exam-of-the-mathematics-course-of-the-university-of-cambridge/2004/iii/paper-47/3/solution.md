<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Use the mostly-minus [Minkowski metric](../../../../../minkowski-metric.md), [quantum field theory propagator](../../../../../propagator.md) $i/(p^2-m^2+i0)$ and dimensionally continued interaction $-\mu^{2\epsilon}\lambda\phi^4/4!$, with $d=4-2\epsilon$. Take all four external momenta incoming, so $\sum_jp_j=0$, and set $s=(p_1+p_2)^2$, $t=(p_1+p_3)^2$, $u=(p_1+p_4)^2$.

The three one-loop [one-particle-irreducible Feynman diagrams](../../../../../one-particle-irreducible-feynman-diagram.md) are the bubble graphs with external pairings $(12|34)$, $(13|24)$ and $(14|23)$. Their external [quantum field theory propagators](../../../../../propagator.md) are omitted by [amputation](../../../../../amputation-of-external-propagators.md). Each [Feynman diagram](../../../../../feynman-diagram.md) has [symmetry factor](../../../../../feynman-diagram-symmetry-factor.md) $1/2$ from exchanging the two internal lines; the fixed external labels are already accounted for by the three distinct channels.

<a id="3/image-the-three-labeled-one-loop-scalar-four-point-bubble-channels-with-all-external-momenta-incoming"></a>
![](../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-47-bubble-channels.png)

**[Figure 1](#3/image-the-three-labeled-one-loop-scalar-four-point-bubble-channels-with-all-external-momenta-incoming). The three labeled one-loop scalar four-point bubble channels with all external momenta incoming**.

For a channel carrying momentum $q$, its amplitude is

$$
B(q^2)=\frac{(-i\mu^{2\epsilon}\lambda)^2}{2}
\int\frac{d^d\ell}{(2\pi)^d}
\frac{i}{\ell^2-m^2+i0}\frac{i}{(\ell+q)^2-m^2+i0}
=\frac{\mu^{4\epsilon}\lambda^2}{2}
\int\frac{d^d\ell}{(2\pi)^d}\frac1{AB}.
$$

The signs in the last equality follow from the two vertices and two [quantum field theory propagators](../../../../../propagator.md). Apply the [Feynman parameter](../../../../../feynman-parameter.md) identity

$$
\frac1{AB}=\int_0^1\frac{dx}{[xA+(1-x)B]^2}.
$$

After shifting the [loop momentum](../../../../../loop-momentum.md), the denominator is $(k^2-\Delta_q(x)+i0)^2$, with $\Delta_q(x)=m^2-x(1-x)q^2$. For positive Euclidean $\Delta$, [Wick rotation](../../../../../wick-rotation.md) and the Schwinger representation give

$$
\begin{aligned}
\int\frac{d^dk}{(2\pi)^d}\frac1{(k^2-\Delta+i0)^2}
&=i\int\frac{d^dk_E}{(2\pi)^d}\int_0^\infty d\alpha\,\alpha e^{-\alpha(k_E^2+\Delta)}\\
&=\frac{i}{(4\pi)^{d/2}}\int_0^\infty d\alpha\,\alpha^{1-d/2}e^{-\alpha\Delta}\\
&=\frac{i}{(4\pi)^{d/2}}\Gamma(2-d/2)\Delta^{d/2-2}.
\end{aligned}
$$

Analytic continuation to physical momenta keeps the prescription $\Delta_q-i0$. Thus [dimensional regularization](../../../../../dimensional-regularization.md) evaluates the channel as

$$
B(q^2)=\frac{i\mu^{4\epsilon}\lambda^2}{2(4\pi)^{2-\epsilon}}
\Gamma(\epsilon)\int_0^1dx\,[\Delta_q(x)-i0]^{-\epsilon}.
$$

Use $\Gamma(\epsilon)=\epsilon^{-1}-\gamma_E+O(\epsilon)$ and expand the other factors. The [minimal-subtraction scalar four-point bubble channels](../../../../../minimal-subtraction-scalar-four-point-bubble-channels.md) result through the finite part is

$$
B(q^2)=\frac{i\mu^{2\epsilon}\lambda^2}{32\pi^2}
\left[\frac1\epsilon-\gamma_E+\log(4\pi)
-\int_0^1dx\,\log\frac{m^2-x(1-x)q^2-i0}{\mu^2}\right]+O(\epsilon).
$$

The parameter [integral](../../../../../integral.md) is left unevaluated, as requested. The three channel contributions are $B(s)+B(t)+B(u)$. Their pole is momentum independent and is cancelled by the four-point [counterterm](../../../../../counterterm.md) $-i\mu^{2\epsilon}\delta\lambda$, with

$$
\boxed{\delta\lambda=\frac{3\lambda^2}{32\pi^2\epsilon}+O(\lambda^3).}
$$

After pure [minimal subtraction scheme](../../../../../minimal-subtraction-scheme.md) subtraction, the complete vertex through one loop is the tree vertex $-i\lambda$ plus

$$
\frac{i\lambda^2}{32\pi^2}\sum_{r\in\{s,t,u\}}
\left[\log(4\pi)-\gamma_E-\int_0^1dx\,
\log\frac{m^2-x(1-x)r-i0}{\mu^2}\right].
$$

Here the $\epsilon\to0$ limit has been taken. The [modified minimal subtraction scheme](../../../../../modified-minimal-subtraction-scheme.md) would also absorb $\log(4\pi)-\gamma_E$; it is not identical to the specified pure MS finite part.

The bare coupling is scale independent and satisfies

$$
\lambda_B=\mu^{2\epsilon}\left(\lambda+\frac{a\lambda^2}{\epsilon}+O(\lambda^3)\right),
\qquad a=\frac3{32\pi^2}.
$$

Writing $\beta_d=-2\epsilon\lambda+b\lambda^2+O(\lambda^3)$ and differentiating at fixed $\lambda_B$ gives

$$
0=2\epsilon\left(\lambda+\frac{a\lambda^2}{\epsilon}\right)
+\beta_d\left(1+\frac{2a\lambda}{\epsilon}\right).
$$

At order $\lambda^2$, the finite coefficient is $b-2a$, so the [one-loop quartic scalar beta function](../../../../../one-loop-quartic-scalar-beta-function.md) is

$$
\boxed{\beta(\lambda)=\mu\frac{d\lambda}{d\mu}\bigg|_{\lambda_B}
=\frac{3\lambda^2}{16\pi^2}+O(\lambda^3).}
$$

The factor two relative to the pole residue follows from using $d=4-2\epsilon$. With $d=4-\epsilon$ the residue doubles, but the four-dimensional beta function is unchanged.

For pure nonabelian gauge theory, the corresponding [pure Yang-Mills one-loop beta function](../../../../../pure-yang-mills-one-loop-beta-function.md) has the opposite sign:

$$
\beta(g)=-\frac{11C_A}{3(16\pi^2)}g^3+O(g^5),
\qquad f^{acd}f^{bcd}=C_A\delta^{ab}.
$$

Gauge-boson self-interactions and the gauge-consistency ghost contributions give antiscreening. For a compact nonabelian simple factor $C_A>0$, the coupling decreases at high energy: [asymptotic freedom](../../../../../asymptotic-freedom.md). In contrast, positive scalar $\lambda$ increases toward the ultraviolet. Its one-loop extrapolation has a [Landau pole](../../../../../landau-pole.md), indicating breakdown of weak-coupling perturbation theory, not a proof by itself of nonperturbative triviality. Ultraviolet poles should be extracted at infrared-safe mass or nonexceptional kinematics; a scaleless massless zero-momentum [integral](../../../../../integral.md) cannot be used to read off this ultraviolet [counterterm](../../../../../counterterm.md) without separating its infrared behavior.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 47](../../paper-47-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
