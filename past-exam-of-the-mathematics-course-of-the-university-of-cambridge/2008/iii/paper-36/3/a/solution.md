<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the PDF's starred image hull $K_t^*$ and write $h_t=\Phi_t=g_{K_t^*}\circ\Phi\circ g_{K_t}^{-1}$. For $t<T$, this map is analytic across a real neighborhood of the driver. Set

$$
a_t=h_t'(\xi_t)=\Sigma_t>0,\qquad
b_t=h_t''(\xi_t),\qquad c_t=h_t'''(\xi_t),\qquad
\xi_t=\sqrt\kappa\,B_t.
$$

Let $u(t)=\operatorname{hcap}(K_t^*)/2$. The classical [conformal change of half-plane capacity](../../../../../../conformal-change-of-half-plane-capacity.md) gives $\dot u(t)=a_t^2$, and the image driver, indexed by original time, is $h_t(\xi_t)$. Differentiating the conjugacy relation gives

$$
\partial_t h_t(z)
=\frac{2a_t^2}{h_t(z)-h_t(\xi_t)}
-\frac{2h_t'(z)}{z-\xi_t}.
$$

These are precisely the standard classical identities allowed in this question. The singularities cancel at $z=\xi_t$. To calculate the remaining [derivative](../../../../../../derivative.md), put $\delta=z-\xi_t$ and expand at fixed $t$:

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

where each $\partial_t$ keeps the spatial variable fixed before evaluation. Applying the [Itô formula](../../../../../../ito-s-lemma.md) to $h_t'(\xi_t)$ gives the [boundary derivative diffusion under conformal Loewner conjugacy](../../../../../../boundary-derivative-diffusion-under-conformal-loewner-conjugacy.md)

$$
da_t=\sqrt\kappa\,b_t\,dB_t+
\left[\frac{b_t^2}{2a_t}+\left(\frac\kappa2-\frac43\right)c_t\right]dt.
$$

At $\kappa=8/3$, the third-derivative drift cancels. A second application of the [Itô formula](../../../../../../ito-s-lemma.md) to $a_t^p$ gives

$$
d(a_t^p)=p\sqrt\kappa\,a_t^{p-1}b_t\,dB_t
+\frac p2[1+\kappa(p-1)]a_t^{p-2}b_t^2\,dt.
$$

Choosing $p=1-1/\kappa=5/8$ cancels the remaining drift. Hence the [SLE eight-thirds restriction martingale](../../../../../../sle-eight-thirds-restriction-martingale.md) is

$$
\boxed{M_t=\Sigma_t^{5/8},\qquad
dM_t=\frac58\sqrt{\frac83}\,\Sigma_t^{-3/8}b_t\,dB_t,quad t<T.}
$$

Localizing away from $T$ and from vanishing [derivatives](../../../../../../derivative.md) makes the displayed [stochastic integral](../../../../../../stochastic-integral.md) a [martingale](../../../../../../martingale-split.md) on each localized interval, so it defines a continuous [local martingale](../../../../../../local-martingale.md) up to $T$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
