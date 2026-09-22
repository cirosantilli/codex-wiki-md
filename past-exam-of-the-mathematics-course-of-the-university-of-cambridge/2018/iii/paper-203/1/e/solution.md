<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

The scaling rule for the [Chordal Loewner equation](../../../../../../chordal-loewner-equation.md) shows that $A_t=\sqrt t\,A_1$, because $r^{-1}U_{r^2t}=a\sqrt t$. To identify the shape, rather than infer it from scaling alone, construct the inverse map explicitly. Put

$$
d=\sqrt{a^2+16},\qquad r_\pm=\frac{a\pm d}{2},\qquad
\alpha=-\frac{r_-}{d}\in(0,1).
$$

Then $r_-<0<r_+$, $r_-r_+=-4$, and $\alpha r_++(1-\alpha)r_-=0$. Define

$$
f_t(w)=(w-r_+\sqrt t)^\alpha(w-r_-\sqrt t)^{1-\alpha},
$$

using logarithms whose arguments lie in $(0,\pi)$ on $\mathbb H$. Its [Laurent series](../../../../../../laurent-series.md) is $f_t(w)=w-2t/w+O(w^{-2})$, so it has the inverse [hydrodynamic normalization at infinity](../../../../../../hydrodynamic-normalization-at-infinity.md).

On the real interval $(r_-\sqrt t,r_+\sqrt t)$, the first factor has argument $\pi\alpha$ and the second has argument zero. The image therefore lies on one straight ray. Its modulus increases from zero to a maximum at $w=a\sqrt t$, and then decreases to zero. The complementary real intervals map to the negative and positive real axes. The [argument principle](../../../../../../argument-principle.md), or the usual conformal slit-map construction, shows that $f_t$ maps $\mathbb H$ conformally onto the half-plane minus that segment; the interval traverses its two sides.

The boundary walk has winding number one around every point of the half-plane off the segment: the two traversals of the slit cancel, leaving the real boundary and a large semicircle. The [argument principle](../../../../../../argument-principle.md) therefore gives exactly one preimage of each such point.

It remains to check that this is the correct [Loewner chain](../../../../../../loewner-chain.md). For $f=f_1$,

$$
\frac{f'(w)}{f(w)}=\frac{w-a}{(w-r_+)(w-r_-)}
=\frac{w-a}{w^2-aw-4}.
$$

Together with $f_t(w)=\sqrt t\,f(w/\sqrt t)$, this gives

$$
\partial_tf_t(w)=-\frac{2f_t'(w)}{w-a\sqrt t},
$$

the inverse form of the [Chordal Loewner equation](../../../../../../chordal-loewner-equation.md). Uniqueness therefore identifies its slit with $A_t$. Its endpoint is $\sqrt t\,f_1(a)$, where $f_1(a)\ne0$ lies in $\mathbb H$. This proves that the [square-root Loewner driving function generates a straight slit](../../../../../../square-root-loewner-driving-function-generates-a-straight-slit.md) and that

$$
\boxed{\bigcup_{t\geq0}A_t=\{s f_1(a):s>0\},}
$$

a straight ray from the boundary point $0$ to infinity.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [1](../../1.md)
3. [Paper 203](../../../paper-203-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
