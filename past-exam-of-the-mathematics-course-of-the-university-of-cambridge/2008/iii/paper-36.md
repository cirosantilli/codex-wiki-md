# Paper 36

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2008/Paper36.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2008/Paper36.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)

## 1

↑ **Parent:** [Paper 36](paper-36.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Write $D=\mathbb H\setminus K$. By definition of a [compact H-hull](../../../stochastic-process.md#compact-h-hull), $D$ is a proper [simply connected domain](../../../complex-analysis.md#simply-connected-domain), and it agrees with the [complex upper half-plane](../../../complex-analysis.md#upper-half-plane-complex-analysis) outside a sufficiently large disc. The [Riemann mapping theorem](../../../complex-analysis.md#riemann-mapping-theorem) supplies a [conformal isomorphism](../../../complex-analysis.md#biholomorphism) $f:D\to\mathbb H$. Choose its boundary normalization so that the [prime end](../../../geometry-and-topology.md#prime-end) at infinity maps to infinity. This [prime end](../../../geometry-and-topology.md#prime-end) is unambiguous because the domain has an ordinary straight real boundary near infinity.

The [Schwarz reflection principle](../../../complex-analysis.md#schwarz-reflection-principle), applied there in the coordinate $1/z$, extends $f$ across the real boundary near infinity. It has a simple pole there, with [Laurent series](../../../analysis.md#laurent-series)

$$
f(z)=az+b+\frac{c}{z}+O(z^{-2}),\qquad a>0,\quad b,c\in\mathbb R.
$$

The pole is simple because the reflected map is locally conformal at infinity; its leading coefficient is positive because it maps the upper side to the upper side. Postcomposing with the half-plane automorphism $w\mapsto(w-b)/a$ gives

$$
g_K(z)=z+O(1/z),\qquad\boxed{g_K(z)-z\longrightarrow0.}
$$

This is [hydrodynamic normalization at infinity](../../../stochastic-process.md#hydrodynamic-normalization-at-infinity).

If $g_1,g_2$ both satisfy it, $g_2\circ g_1^{-1}$ is a [conformal automorphism of the upper half-plane](../../../complex-analysis.md#conformal-automorphism-of-the-upper-half-plane). The asymptotics force it to fix infinity, so it has the form $w\mapsto\alpha w+\beta$ with $\alpha>0$ and $\beta\in\mathbb R$. The same asymptotics force $\alpha=1$, $\beta=0$. Hence **the normalized [mapping-out function](../../../stochastic-process.md#mapping-out-function-of-a-compact-h-hull) exists and is unique**. The argument requires reflection only outside a large disc, not regularity of the hull's entire boundary.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

For the [Joukowski map](../../../geometry-and-topology.md#joukowski-map) $g(z)=z+z^{-1}$,

$$
\operatorname{Im}g(z)=\operatorname{Im}z\left(1-\frac1{|z|^2}\right).
$$

It maps the exterior upper half-disc $D_0=\{z\in\mathbb H:|z|>1\}$ into $\mathbb H$. It is injective there: $g(z)=g(w)$ gives $(z-w)(1-1/(zw))=0$, and the second factor cannot vanish when both moduli exceed one. It is onto as well. For $v\in\mathbb H$, the two roots of $z^2-vz+1=0$ have product one. Neither lies on the unit circle, since $z+z^{-1}$ is real there. Exactly one root has modulus greater than one, and the displayed imaginary-part formula makes its imaginary part positive. That root belongs to $D_0$ and maps to $v$.

Since $g_{K_0}$ takes values in $\mathbb H$, its domain must be contained in $D_0$. The established injectivity and surjectivity of $g:D_0\to\mathbb H$ mean that no proper subdomain of $D_0$ can map onto all of $\mathbb H$ using this same function. Therefore

$$
\boxed{K_0=\{z\in\mathbb H:|z|\leq1\},\qquad\operatorname{hcap}(K_0)=1.}
$$

The [half-plane capacity](../../../stochastic-process.md#half-plane-capacity) is the coefficient of $1/z$ in the normalized expansion. If hulls are regarded as closed subsets of $\overline{\mathbb H}$, take the closure of this half-disc, including its diameter; its relative half-plane hull and capacity are unchanged. This is the [half-plane capacity of a half-disc](../../../stochastic-process.md#half-plane-capacity-of-a-half-disc).

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

At a real point $x$ outside the hull's closure, the [Schwarz reflection principle](../../../complex-analysis.md#schwarz-reflection-principle) makes the [mapping-out function](../../../stochastic-process.md#mapping-out-function-of-a-compact-h-hull) analytic across the boundary and $g_K'(x)>0$. Use the course's Brownian excursion restriction identity: for an excursion from $x$ to infinity in the [complex upper half-plane](../../../complex-analysis.md#upper-half-plane-complex-analysis),

$$
\mathbb P_x^{\rm exc}(\widehat B\cap K=\varnothing)=g_K'(x).
$$

One way to obtain this identity is to start its [Doob h-transform](../../../markov-process.md#doob-h-transform) at $x+i\varepsilon$: its avoidance probability is $\operatorname{Im}g_K(x+i\varepsilon)/\varepsilon$, which tends to $g_K'(x)$ by reflection. Thus the [boundary derivative is an excursion avoidance probability](../../../brownian-motion.md#boundary-derivative-is-an-excursion-avoidance-probability), and in particular it is at most one.

Let $D$ be the filled unit half-disc. Since $K\subseteq D$, avoiding $D$ implies avoiding $K$. The [monotonicity of boundary derivatives of mapping-out functions](../../../stochastic-process.md#monotonicity-of-boundary-derivatives-of-mapping-out-functions) and part (b) give, for $|x|>1$,

$$
\boxed{1-x^{-2}=g_D'(x)\leq g_K'(x)\leq1.}
$$

The upper bound is attained by the empty hull and the lower by the filled half-disc, so the comparison is sharp on either real tail.

## 2

↑ **Parent:** [Paper 36](paper-36.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

For chordal [SLE](../../../stochastic-process.md#schramm-loewner-evolution) with parameter $\kappa$, the [Loewner trace](../../../stochastic-process.md#trace-of-a-loewner-chain) $\gamma$ starts at zero and is parametrized by [half-plane capacity](../../../stochastic-process.md#half-plane-capacity) $2t$. Let $D_t$ be the unbounded component of $\mathbb H\setminus\gamma[0,t]$, and let $K_t=\mathbb H\setminus D_t$ be its filled [compact H-hull](../../../stochastic-process.md#compact-h-hull). When the trace is not simple, the hull includes the regions it disconnects from infinity. The associated [mapping-out functions of compact H-hulls](../../../stochastic-process.md#mapping-out-function-of-a-compact-h-hull) have expansion

$$
g_t(z)=z+\frac{2t}{z}+O(z^{-2})
$$

and satisfy the [Chordal Loewner equation](../../../stochastic-process.md#chordal-loewner-equation)

$$
\boxed{\partial_tg_t(z)=\frac2{g_t(z)-\xi_t},\qquad
g_0(z)=z,\qquad\xi_t=\sqrt\kappa\,B_t,}
$$

where $B$ is standard real [Brownian motion](../../../brownian-motion.md). The equation is solved until $z$ is swallowed by the hull. The [Loewner transform](../../../stochastic-process.md#loewner-driving-function) $\xi$ records the real boundary point at which the mapped hull grows; its relation to the trace is

$$
\gamma_t=\lim_{y\downarrow0}g_t^{-1}(\xi_t+iy).
$$

Equivalently the tip maps to $\xi_t$ in the appropriate boundary prime-end sense. Thus the flow encodes the surviving domains, the transform drives that flow, and the trace generates its hulls. For $\kappa=0$, the driver is identically zero, $g_t(z)=\sqrt{z^2+4t}$ with the branch asymptotic to $z$, and $\gamma_t=2i\sqrt t$.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

After the fixed time $s$, the [mapping-out function](../../../stochastic-process.md#mapping-out-function-of-a-compact-h-hull) of the uncentered mapped future is

$$
\bar g_t=g_{s+t}\circ g_s^{-1}.
$$

Its expansion is $\bar g_t(z)=z+2t/z+O(z^{-2})$, so the elapsed time $t$ is still the [half-plane-capacity parameterization](../../../stochastic-process.md#half-plane-capacity-parameterization). Differentiating in $t$ yields

$$
\partial_t\bar g_t(z)=\frac2{\bar g_t(z)-\xi_{s+t}},\qquad\bar g_0(z)=z.
$$

Therefore **the [Loewner transform](../../../stochastic-process.md#loewner-driving-function) of $\bar\gamma_t=g_s(\gamma_{s+t})$ is $\xi_{s+t}$**, with starting point $\xi_s$.

Centering gives $\tilde g_t(w)=\bar g_t(w+\xi_s)-\xi_s$, whose driver is $\tilde\xi_t=\xi_{s+t}-\xi_s$. By independent stationary [Brownian increments](../../../brownian-motion.md#brownian-increment), $(B_{s+t}-B_s)_{t\geq0}$ is a standard [Brownian motion](../../../brownian-motion.md) independent of the past through time $s$. Hence

$$
\boxed{(\tilde\gamma_t)_{t\geq0}\text{ is a fresh chordal SLE}(\kappa)
\text{ from }0\text{ to }\infty,\text{ independent of the past}.}
$$

This proves the [domain Markov property of a chordal Loewner chain](../../../stochastic-process.md#domain-markov-property-of-a-chordal-loewner-chain) from the [composition rule for chordal Loewner driving functions](../../../stochastic-process.md#composition-rule-for-chordal-loewner-driving-functions). For possible contacts with the old hull, the mapped trace is understood through the continuous boundary extension or [prime ends](../../../geometry-and-topology.md#prime-end); on the open half-plane the displayed maps are ordinary [conformal maps](../../../geometry-and-topology.md#conformal-map). The PDF asks first for the driver of the uncentered curve $\bar\gamma$; the centered driver is included as well.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

For $0<\kappa\leq4$, use the allowed probability-one event that the whole [SLE](../../../stochastic-process.md#schramm-loewner-evolution) trace lies in $\mathbb H$ at every positive time. At each deterministic rational $s>0$, part (b) makes the centered mapped future a fresh [SLE](../../../stochastic-process.md#schramm-loewner-evolution) with the same property. Consequently, almost surely, for every $t>0$,

$$
\tilde\gamma_t\in\mathbb H,\qquad
\gamma_{s+t}=g_s^{-1}(\tilde\gamma_t+\xi_s)\in D_s=\mathbb H\setminus K_s.
$$

This inverse relation holds through the trace's boundary-extension construction and puts positive-time future points in the open surviving domain. It therefore excludes every contact with the old filled hull, not just contacts with a fixed old point.

Intersect these probability-one events over all positive rational $s$. If $\gamma_u=\gamma_v$ for $0<u<v$, choose rational $s$ with $u<s<v$. The first occurrence belongs to $K_s$, whereas the second lies in $D_s$, a contradiction. A return to $\gamma_0=0$ is excluded by the original positive-imaginary-part assertion. This [simplicity of SLE from boundary-avoiding restarts](../../../stochastic-process.md#simplicity-of-sle-from-boundary-avoiding-restarts) proves

$$
\boxed{\gamma\text{ is almost surely a simple curve for }0<\kappa\leq4.}
$$

## 3

↑ **Parent:** [Paper 36](paper-36.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Use the PDF's starred image hull $K_t^*$ and write $h_t=\Phi_t=g_{K_t^*}\circ\Phi\circ g_{K_t}^{-1}$. For $t<T$, this map is analytic across a real neighborhood of the driver. Set

$$
a_t=h_t'(\xi_t)=\Sigma_t>0,\qquad
b_t=h_t''(\xi_t),\qquad c_t=h_t'''(\xi_t),\qquad
\xi_t=\sqrt\kappa\,B_t.
$$

Let $u(t)=\operatorname{hcap}(K_t^*)/2$. The classical [conformal change of half-plane capacity](../../../stochastic-process.md#conformal-change-of-half-plane-capacity) gives $\dot u(t)=a_t^2$, and the image driver, indexed by original time, is $h_t(\xi_t)$. Differentiating the conjugacy relation gives

$$
\partial_t h_t(z)
=\frac{2a_t^2}{h_t(z)-h_t(\xi_t)}
-\frac{2h_t'(z)}{z-\xi_t}.
$$

These are precisely the standard classical identities allowed in this question. The singularities cancel at $z=\xi_t$. To calculate the remaining [derivative](../../../calculus.md#derivative), put $\delta=z-\xi_t$ and expand at fixed $t$:

$$
\begin{aligned}
\frac{2a_t^2}{h_t(z)-h_t(\xi_t)}
&=\frac{2a_t}{\delta}-b_t+
\left(\frac{b_t^2}{2a_t}-\frac{c_t}{3}\right)\delta+O(\delta^2),\\
\frac{2h_t'(z)}{z-\xi_t}
&=\frac{2a_t}{\delta}+2b_t+c_t\delta+O(\delta^2).
\end{aligned}
$$

Therefore

$$
\partial_t h_t(\xi_t)=-3b_t,\qquad
\partial_t h_t'(\xi_t)=\frac{b_t^2}{2a_t}-\frac43c_t,
$$

where each $\partial_t$ keeps the spatial variable fixed before evaluation. Applying the [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) to $h_t'(\xi_t)$ gives the [boundary derivative diffusion under conformal Loewner conjugacy](../../../stochastic-process.md#boundary-derivative-diffusion-under-conformal-loewner-conjugacy)

$$
da_t=\sqrt\kappa\,b_t\,dB_t+
\left[\frac{b_t^2}{2a_t}+\left(\frac\kappa2-\frac43\right)c_t\right]dt.
$$

At $\kappa=8/3$, the third-derivative drift cancels. A second application of the [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) to $a_t^p$ gives

$$
d(a_t^p)=p\sqrt\kappa\,a_t^{p-1}b_t\,dB_t
+\frac p2[1+\kappa(p-1)]a_t^{p-2}b_t^2\,dt.
$$

Choosing $p=1-1/\kappa=5/8$ cancels the remaining drift. Hence the [SLE eight-thirds restriction martingale](../../../stochastic-process.md#sle-eight-thirds-restriction-martingale) is

$$
\boxed{M_t=\Sigma_t^{5/8},\qquad
dM_t=\frac58\sqrt{\frac83}\,\Sigma_t^{-3/8}b_t\,dB_t,quad t<T.}
$$

Localizing away from $T$ and from vanishing [derivatives](../../../calculus.md#derivative) makes the displayed [stochastic integral](../../../stochastic-calculus.md#stochastic-integral) a [martingale](../../../martingale.md) on each localized interval, so it defines a continuous [local martingale](../../../martingale.md#local-martingale) up to $T$.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Put $A=\mathbb H\setminus U$. The neighborhood assumptions at zero and infinity mean that $A$ is a bounded hull away from the starting boundary point. For $t<T$, the conjugacy map $h_t$ is the hydrodynamically normalized [mapping-out function](../../../stochastic-process.md#mapping-out-function-of-a-compact-h-hull) of the remaining forbidden hull after removing $K_t$. Its closure avoids the driver, so the [boundary derivative is an excursion avoidance probability](../../../brownian-motion.md#boundary-derivative-is-an-excursion-avoidance-probability) yields $0<\Sigma_t\leq1$. Thus $0<M_t\leq1$, and the [bounded local martingale criterion](../../../martingale.md#bounded-local-martingale-criterion) makes the localized [martingales](../../../martingale.md) uniformly bounded and uniformly integrable.

Choose localization times $\tau_n\uparrow T$, also bounded by $n$. Optional stopping gives $\mathbb E M_{\tau_n}=M_0$. The supplied terminal limit and continuity of the power function give

$$
M_{\tau_n}\longrightarrow\mathbf1_{\{T=\infty\}},\qquad
M_0=\Phi'(0)^{5/8}.
$$

Since these variables are bounded by one, dominated convergence yields

$$
\boxed{\mathbb P(\gamma_t\in U\text{ for all positive times})
=\mathbb P(T=\infty)=\Phi'(0)^{5/8}.}
$$

As usual for a chord starting at zero, the time-zero point is understood as the boundary [prime end](../../../geometry-and-topology.md#prime-end) of $U$; the avoidance assertion concerns the subsequent curve. The boundedness step is what upgrades the [local martingale](../../../martingale.md#local-martingale) calculation to an equality of probabilities.

## 4

↑ **Parent:** [Paper 36](paper-36.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Regard a chord as an oriented curve modulo increasing reparameterization, and write $[\gamma]$ for that class. Scale invariance of $\mu$ means that $[r\gamma]$ has the same law for each $r>0$. The [locality of a chord law under conformal changes of neighborhoods](../../../stochastic-process.md#locality-of-a-chord-law-under-conformal-changes-of-neighborhoods) is the following stopped-curve property: if $N,N^*$ are neighborhoods of the starting boundary point and $\Phi:N\to N^*$ is a boundary-preserving [conformal isomorphism](../../../complex-analysis.md#biholomorphism) with $\Phi(0)=0$, then

$$
\boxed{\left[\Phi(\gamma\text{ stopped on leaving }N)\right]
\overset{\rm law}=
\left[\gamma\text{ stopped on leaving }N^*\right].}
$$

The two stopped curves are sampled from the same original law $\mu$; equality is for their unparameterized initial segments. A normalization of $\Phi'(0)$ can be imposed in an equivalent formulation, since scale invariance removes the positive dilation. In a hull-removal formulation, the [Locality property of SLE](../../../stochastic-process.md#locality-property-of-sle) says that a modification away from the starting point leaves the initial law unchanged until the curve reaches the modified part of the domain.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Let $g_t$ map out the original filled hull and let $g_t^*$ map out the filled hull generated by $\Phi(\gamma[0,t])$. Both have [hydrodynamic normalization at infinity](../../../stochastic-process.md#hydrodynamic-normalization-at-infinity). Write

$$
h_t=g_t^*\circ\Phi\circ g_t^{-1},\qquad
W_t=h_t(\xi_t),\qquad a_t=h_t'(\xi_t),\quad b_t=h_t''(\xi_t).
$$

Although the original $\Phi$ is specified only on $N$, this conjugacy is defined in the surviving neighborhood of the tip. Boundary preservation gives a real analytic extension there by the [Schwarz reflection principle](../../../complex-analysis.md#schwarz-reflection-principle), with $a_t>0$. The identities below are first applied on compactly localized intervals before exit and then continued up to $T$.

Set $u(t)=\operatorname{hcap}(K_t^*)/2$, the capacity clock of the image hull. The [Chordal Loewner equation](../../../stochastic-process.md#chordal-loewner-equation) for each flow and the chain rule give

$$
\partial_t h_t(z)
=\frac{2\dot u(t)}{h_t(z)-W_t}
-\frac{2h_t'(z)}{z-\xi_t},\qquad W_t=h_t(\xi_t).
$$

Analyticity at the driving point cancels the coefficient of $(z-\xi_t)^{-1}$, forcing $\dot u(t)=a_t^2$. The constant term, computed as in Question 3, is then $\partial_t h_t(\xi_t)=-3b_t$. For a general [SLE](../../../stochastic-process.md#schramm-loewner-evolution) driver $d\xi_t=\sqrt\kappa\,dB_t$, the [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) consequently gives the [transformed SLE driving function](../../../stochastic-process.md#transformed-sle-driving-function)

$$
dW_t=\sqrt\kappa\,a_t\,dB_t+
\left(\frac\kappa2-3\right)b_t\,dt.
$$

At $\kappa=6$, this becomes

$$
\boxed{dW_t=\sqrt6\,a_t\,dB_t,\qquad
\langle W\rangle_t=6\int_0^t a_s^2ds=6u(t).}
$$

Thus $W$ is a continuous [local martingale](../../../martingale.md#local-martingale) up to the exit time. If the source notation $\xi_t^*$ indexes the image driver by original time, it denotes $W_t$. If it uses the image's own half-plane-capacity time, it denotes $W_{t(u)}$, with $t(u)$ the inverse clock; that time-changed process is also a [local martingale](../../../martingale.md#local-martingale). This distinguishes the two clocks without changing the requested conclusion.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Since $\dot u(t)=a_t^2>0$, invert the image clock before exit and put $\widehat\xi_u=W_{t(u)}$. Its [quadratic variation](../../../stochastic-calculus.md#quadratic-variation) is $6u$ and its initial value is zero, because $\Phi(0)=0$. By the [Lévy characterization of Brownian motion](../../../brownian-motion.md#levy-characterization-of-brownian-motion), or the localized [Dambis-Dubins-Schwarz theorem](../../../martingale.md#dambis-dubins-schwarz-theorem),

$$
\widehat\xi_u=\sqrt6\,\widehat B_u
$$

for a standard [Brownian motion](../../../brownian-motion.md) up to the image exit time. If that lifetime is finite, the stopped [Brownian motion](../../../brownian-motion.md) can be extended beyond it; only the stopped law is used here.

In this clock the image [mapping-out functions](../../../stochastic-process.md#mapping-out-function-of-a-compact-h-hull) obey the ordinary [Chordal Loewner equation](../../../stochastic-process.md#chordal-loewner-equation) with driver $\sqrt6\,\widehat B_u$. Their generated trace therefore has the law of [SLE](../../../stochastic-process.md#schramm-loewner-evolution) with parameter six, stopped when it leaves $N^*$. Meanwhile the original image segment is exactly $\Phi(\gamma)$ up to exit from $N$. The clock change is increasing, so it disappears after passing to $[\gamma]$. This proves **the local stopped-curve equality required in part (a)**.

For completeness, the original law is scale invariant: the maps $r^{-1}g_{r^2t}(rz)$ have driver $r^{-1}\xi_{r^2t}$, whose law is again $\sqrt6 B_t$ by [Brownian scaling](../../../brownian-motion.md#brownian-scaling). Hence $(r^{-1}\gamma_{r^2t})_{t\geq0}$ has the original trace law. Together with the stopped conformal-change argument, this establishes

$$
\boxed{[\gamma]\text{ for SLE}(6)\text{ has the locality property}.}
$$

The conclusion concerns local unparameterized segments up to exit; the capacity parameter itself changes according to $du=h_t'(\xi_t)^2dt$.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2008](../../2008.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
