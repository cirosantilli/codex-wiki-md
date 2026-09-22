<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

An [explicit disk map of a slit half disk](../../../../../explicit-disk-map-of-a-slit-half-disk.md) makes the two [boundary](../../../../../boundary-of-a-set.md) approaches visible without assuming an extension theorem for the [boundary](../../../../../boundary-of-a-set.md). We construct the map as a succession of [bijections](../../../../../bijection.md) and then determine its limits.

First $w=z^2$ maps the upper half-disc of radius two bijectively onto $|w|<4$ slit along $[0,4)$. Indeed, its inverse chooses the [square root](../../../../../square-root.md) whose argument lies in $(0,\pi)$. The removed segment on the [imaginary axis](../../../../../imaginary-axis.md) becomes $[-1,0)$, so the image of $D$ is precisely

$$
\Omega=\{w:|w|<4\}\setminus[-1,4).
$$

The [Möbius transformation](../../../../../mobius-transformation.md) $v=4(w+1)/(w+16)$ maps the radius-four disc bijectively onto the [unit disc](../../../../../unit-disc.md), taking $-1$ to zero and $4$ to one. This follows also by writing it as $(w/4+1/4)/(1+w/16)$, an [automorphism of the unit disk](../../../../../automorphism-of-the-unit-disk.md) after the scaling. It takes the removed real interval to $[0,1)$, so the image is the unit disc with this radial slit removed. Choosing $0<\arg v<2\pi$ defines a single-valued [square root](../../../../../square-root.md) $u=\sqrt v$ and maps that slit disc bijectively onto

$$
U=\{u:|u|<1,\ \operatorname{Im}u>0\}.
$$

All these maps have nonzero [derivatives](../../../../../derivative.md) on their respective domains, since their potentially problematic zero or branch point is on the removed slit.

Next the [Joukowski map](../../../../../joukowski-map.md) $J(u)=u+1/u$ is a [conformal bijection](../../../../../biholomorphism.md) from $U$ onto the [lower half-plane](../../../../../lower-half-plane.md). For $u\in U$,

$$
\operatorname{Im}J(u)=\operatorname{Im}u\,(1-|u|^{-2})<0.
$$

If $J(u)=J(t)$, then $(u-t)(1-1/(ut))=0$, and $|ut|<1$ rules out the second factor vanishing. To prove surjectivity, take $q$ in the [lower half-plane](../../../../../lower-half-plane.md) and consider $u^2-qu+1=0$. Neither root lies on the unit [circle](../../../../../circle.md), where $u+1/u$ is real. Their product is one, so exactly one has modulus less than one. For that root the displayed imaginary-part identity forces $\operatorname{Im}u>0$. Thus it lies in $U$. Also $J'(u)=1-u^{-2}$ cannot vanish there. Finally $C(q)=(q+i)/(q-i)$ maps the [lower half-plane](../../../../../lower-half-plane.md) bijectively onto the [unit disc](../../../../../unit-disc.md): the inequality $|q+i|<|q-i|$ is exactly $\operatorname{Im}q<0$, and its inverse is $q=i(\zeta+1)/(\zeta-1)$. Consequently

$$
F(z)=\frac{u(z)+u(z)^{-1}+i}{u(z)+u(z)^{-1}-i},\qquad
u(z)^2=\frac{4(z^2+1)}{z^2+16},\qquad 0<\arg u(z)<\pi,
$$

is a [conformal bijection](../../../../../biholomorphism.md) of $D$ onto the disc.

At the slit point $z_0=i/2$ the continuous rational expression for $v$ tends to $4/21$. In a sufficiently small neighborhood of $z_0$, points of $D$ have nonzero [real part](../../../../../real-part.md). Since $\operatorname{Im}(z^2)=2\operatorname{Re}z\operatorname{Im}z$ and the real-coefficient [Möbius map](../../../../../mobius-transformation.md) $w\mapsto v$ preserves the sign of the [imaginary part](../../../../../imaginary-part.md), right-side approach gives $\arg v\to0$, while left-side approach gives $\arg v\to2\pi$. Hence

$$
u(z)\longrightarrow\begin{cases}c=2/\sqrt{21},&\operatorname{Re}z>0,\\-c,&\operatorname{Re}z<0,\end{cases}
\qquad
J(u(z))\longrightarrow\begin{cases}L=25/(2\sqrt{21}),&\operatorname{Re}z>0,\\-L,&\operatorname{Re}z<0.\end{cases}
$$

The two limits of $F$ are therefore

$$
\gamma_+=\frac{L+i}{L-i},\qquad \gamma_-=\frac{-L+i}{-L-i}.
$$

They have modulus one and are distinct, since $L>0$ and the [Möbius map](../../../../../mobius-transformation.md) $C$ is [injective](../../../../../injective-function.md) on the extended real line. The [two-sided cluster set at an interior slit point](../../../../../two-sided-cluster-set-at-an-interior-slit-point.md) is a geometric consequence of opening the slit into two [boundary](../../../../../boundary-of-a-set.md) intervals.

<a id="5/image-two-sides-of-the-slit-at-i-2-become-distinct-boundary-points-after-squaring-a-disk-automorphism-and-a-square-root"></a>
![](../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-9-slit.png)

**[Figure 1](#5/image-two-sides-of-the-slit-at-i-2-become-distinct-boundary-points-after-squaring-a-disk-automorphism-and-a-square-root). Two sides of the slit at i/2 become distinct boundary points after squaring, a disk automorphism and a square root**.

For the given map $f$, the composition $B=f\circ F^{-1}$ is an [automorphism of the unit disk](../../../../../automorphism-of-the-unit-disk.md). To see its precise [boundary](../../../../../boundary-of-a-set.md) behavior, let $a=B^{-1}(0)$ and compose $B$ with the inverse of $T_a(\zeta)=(\zeta-a)/(1-\overline a\zeta)$. This gives a [disc automorphism](../../../../../automorphism-of-the-unit-disk.md) fixing zero. Applying [Schwarz lemma](../../../../../schwarz-lemma.md) to it and its inverse shows it is a [rotation](../../../../../rotation-mathematics.md). Thus

$$
B(\zeta)=e^{i\theta}\frac{\zeta-a}{1-\overline a\zeta},\qquad |a|<1.
$$

Its denominator never vanishes on the closed disc, and its inverse has the same property; it therefore extends to a continuous [bijection](../../../../../bijection.md) of the unit [circle](../../../../../circle.md). Put **$\alpha=B(\gamma_+)$ and $\beta=B(\gamma_-)$**. These are distinct points of that [circle](../../../../../circle.md), independent of the approaching sequence.

For any sequence approaching $z_0$, every infinite right-side subsequence has image tending to $\alpha$, and every infinite left-side subsequence has image tending to $\beta$. At least one side occurs infinitely often. Conversely, any convergent image subsequence has a further subsequence confined to one side, so its limit must be the corresponding one of these two points. The cluster set is therefore **exactly $\{\alpha\}$, $\{\beta\}$ or $\{\alpha,\beta\}$**, according to which sides occur infinitely often. Both sides really occur in the domain, for example along $i/2\pm\varepsilon_n$ with positive $\varepsilon_n\downarrow0$.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 9](../../paper-9-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
