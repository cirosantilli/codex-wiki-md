<h1 id="a/2/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

The physically meaningful extension requires $h\geq0$: negative net input removes water where wet and cannot keep removing nonexistent surface water where dry. Keeping the algebraic source $E(t)<0$ unchanged in a dry zone would instead produce negative depths, so the drying-front description implicitly includes this availability condition.

Use the same $H(t)$, increasing until $t^*$ and decreasing afterwards. While $H(t)>0$, there is one earlier wetting time $\tau_d(t)\in[0,t^*]$ such that $H(\tau_d(t))=H(t)$. The boundary-emitted [characteristic](../../../../../characteristic-of-a-field.md) with this label has just exhausted its water. Its position is the [drying front](../../../../../drying-front.md):

$$
\boxed{s_d(t)=\frac53\int_{\tau_d(t)}^t[H(r)-H(t)]^{2/3}\,dr.}
$$

The integrand is nonnegative because $H(r)\geq H(t)$ between these two equal-height times. At $t=t^*$ the interval collapses and $s_d=0$; as net input becomes negative the front moves downstream. Differentiating gives $s_d'=-(10/9)E(t)\int_{\tau_d(t)}^t[H(r)-H(t)]^{-1/3}\,dr>0$, where endpoint singularities are integrable away from the turning-time limit.

The wet solution ahead of the front still follows unexhausted [characteristics](../../../../../characteristic-of-a-field.md). With $S_0(t)=\frac53\int_0^tH(r)^{2/3}\,dr$,

$$
\boxed{h(s,t)=\begin{cases}0,&0\leq s\leq s_d(t),\\H(t)-H(\tau(s,t)),&s_d(t)<s<S_0(t),\\H(t),&s\geq S_0(t),\end{cases}}
$$

where $0\leq\tau<\tau_d(t)$ is determined by the same [characteristic](../../../../../characteristic-of-a-field.md)-position [integral](../../../../../integral-split.md) as in (iv). If cumulative loss reaches $H(t)=0$, all remaining initial-line water has also vanished and the surface is dry thereafter while $E<0$. If the total later loss is smaller, the formula applies for all later times with $H(t)>0$. This is the [drying front in a rainfall-driven Manning kinematic wave](../../../../../drying-front-in-a-rainfall-driven-manning-kinematic-wave.md).

## ↑ Ancestors (13)

1. [V](../v.md)
2. [2](../../2.md)
3. [A](../../../a.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the mathematics and the environment and mathematical physiology course of the University of Oxford](../../../../split.md)
6. [Mathematics and the environment and mathematical physiology course of the University of Oxford](../../../../../mathematics-and-the-environment-and-mathematical-physiology-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
