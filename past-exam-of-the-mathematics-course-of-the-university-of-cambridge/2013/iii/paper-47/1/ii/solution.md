<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Choose the positive-exponential branches from part (i) and set their additive constants to zero. First take $0<b<1$, and define

$$
v=\frac{1-b^2}{1+b^2}\in(0,1),\qquad\gamma=\frac{b+b^{-1}}2=\frac1{\sqrt{1-v^2}},\qquad a=-b^{-1}.
$$

Then $\tan(\phi_b/4)=e^{\gamma(x-vt)}$ and $\tan(\phi_a/4)=e^{-\gamma(x+vt)}$. The tangent subtraction formula gives

$$
\tan\frac{\phi_b-\phi_a}{4}=\frac{\sinh(\gamma x)}{\cosh(\gamma vt)},\qquad\frac{b+a}{b-a}=-v.
$$

Consequently the allowed [Sine-Gordon superposition formula](../../../../../../bianchi-permutability-for-sine-gordon-backlund-transformations.md) produces the smooth field

$$
\boxed{\phi_{a,b}(x,t)=-4\arctan\left[\frac{v\sinh(\gamma x)}{\cosh(\gamma vt)}\right].}
$$

This is the negative of the [Sine-Gordon two-kink solution](../../../../../../sine-gordon-two-kink-solution.md), and hence a two-[antikink](../../../../../../antikink.md) configuration. The auxiliary seeds have opposite [topological charges](../../../../../../topological-charge.md), but their charges cannot simply be added to infer the charge of the nonlinear two-step [Bäcklund transformation](../../../../../../backlund-transformation.md). Indeed, the displayed final field tends to $2\pi$ at the left spatial end and $-2\pi$ at the right, so its total [topological charge](../../../../../../topological-charge.md) is $-2$.

Let $T=|t|$ become large. Near the right transition, $x=vT+O(1)$, the tangent argument has the asymptotic form

$$
\frac{v\sinh(\gamma x)}{\cosh(\gamma vt)}=v e^{\gamma(x-vT)}+o(1),
$$

so the local field is $-4\arctan e^{\gamma(x-vT)+\log v}$, a single [antikink](../../../../../../antikink.md). Near the left transition, the local field is $4\arctan e^{-\gamma(x+vT)+\log v}+o(1)$, again a decreasing [antikink](../../../../../../antikink.md). The resulting asymptotic center lines are

$$
\begin{array}{c|cc}
& t\to-\infty&t\to+\infty\\
x_L(t)&vt+\gamma^{-1}\log v&-vt+\gamma^{-1}\log v\\
x_R(t)&-vt-\gamma^{-1}\log v&vt-\gamma^{-1}\log v.
\end{array}
$$

Thus two incoming [antikinks](../../../../../../antikink.md) with [topological charges](../../../../../../topological-charge.md) $(-1,-1)$ and [velocities](../../../../../../velocity.md) $(+v,-v)$ separate again with exactly the same [topological charges](../../../../../../topological-charge.md) and [velocities](../../../../../../velocity.md). There is no radiative tail in these asymptotic profiles. Labeling the outgoing objects by their preserved [rapidities](../../../../../../rapidity.md) makes this elastic [soliton](../../../../../../soliton.md) scattering; labeling the left and right lumps instead describes reflection with exchanged [velocities](../../../../../../velocity.md).

For the right-moving [soliton](../../../../../../soliton.md), its incoming intercept is $\gamma^{-1}\log v$ and its outgoing intercept is $-\gamma^{-1}\log v$. The spatial shifts are therefore $\Delta x_+=-2\gamma^{-1}\log v$ and $\Delta x_-=2\gamma^{-1}\log v$. Define the [soliton time delay](../../../../../../soliton-time-delay.md) as the change in arrival time at a fixed distant spatial point relative to continuation of the incoming straight line, so $\Delta t=-\Delta x/v_{\mathrm{particle}}$. Both objects have **the same signed [soliton time delay](../../../../../../soliton-time-delay.md), which is an advance:**

$$
\boxed{\Delta t=\frac{2\log v}{\gamma v}<0.}
$$

This is the [Sine-Gordon two-kink time advance](../../../../../../sine-gordon-two-kink-time-advance.md). In physical coordinates $T_{\rm phys}=t/m$, the time shift is $2\log v/(m\gamma v)$. The explicit intercepts fix the sign convention unambiguously.

The remaining real parameter choices are covered without changing the calculation. For any $b\ne0$ with $b^2\ne1$, put $v_b=(1-b^2)/(1+b^2)$, $u=|v_b|$, $\gamma=(|b|+|b|^{-1})/2$ and $\epsilon=\operatorname{sgn}(b v_b)$. The same choice of zero additive constants gives

$$
\phi_{a,b}=-4\epsilon\arctan\left[\frac{u\sinh(\gamma x)}{\cosh(\gamma ut)}\right].
$$

Each scattered object's [topological charge](../../../../../../topological-charge.md) is $-\epsilon$, the [velocities](../../../../../../velocity.md) are $\pm u$, and the signed [soliton time delay](../../../../../../soliton-time-delay.md) is $2\log u/(\gamma u)$. If $b=\pm1$, the superposition coefficient vanishes and this representative is the vacuum; there is no pair of separated moving [solitons](../../../../../../soliton.md) and no scattering delay to assign. Thus the scattering conclusion requires the nondegenerate case $0<u<1$.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 47](../../../paper-47-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
