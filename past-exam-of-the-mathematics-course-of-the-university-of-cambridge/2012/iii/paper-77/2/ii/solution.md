<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Set the time derivatives to zero. The scalar equations give

$$
b=\frac{a}{1+a^2},\qquad c=\frac{a^2}{1+a^2},\qquad d=\frac{a\tau}{\tau^2+a^2},\qquad e=\frac{a^2}{\tau^2+a^2}.
$$

For the nonzero convection branch, division of the velocity equation by $a$ gives

$$
\boxed{r(x)=(1+x)+\frac{r_s\tau(1+x)}{\tau^2+x},\qquad x=a^2\ge0.}
$$

Its zero-amplitude limit is $r_e=1+r_s/\tau$. Differentiation yields

$$
r'(x)=1-\frac{r_s\tau(1-\tau^2)}{(\tau^2+x)^2}.
$$

For $0<\tau<1$, the sharp condition for a [subcritical bifurcation](../../../../../../subcritical-bifurcation.md) at the steady onset is $r_s>\tau^3/(1-\tau^2)$. The stronger bound printed in the question is sufficient, since $(1-\tau)^2<1-\tau^2$. Under it the branch initially runs toward smaller $r$, and the unique [saddle-node bifurcation](../../../../../../saddle-node-bifurcation.md) has

$$
\boxed{x_*=a_*^2=-\tau^2+\sqrt{r_s\tau(1-\tau^2)}.}
$$

It is a genuine positive-amplitude minimum: $r''(x)=2r_s\tau(1-\tau^2)/(\tau^2+x)^3>0$. Put $h=\sqrt{r_s\tau}$ and $j=\sqrt{1-\tau^2}$. At the minimum, $1+x_*=j(j+h)$ and $\tau^2+x_*=hj$, so

$$
\boxed{r_{\rm min}=(h+j)^2=\left(\sqrt{r_s\tau}+\sqrt{1-\tau^2}\right)^2.}
$$

These results describe the [steady fold of a thermosolutal Lorenz model](../../../../../../steady-fold-of-a-thermosolutal-lorenz-model.md). They do not by themselves assert stability against every oscillatory disturbance.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Section I](../../section-i.md)
4. [Paper 77](../../../paper-77-split.md)
5. [Iii](../../../split.md)
6. [2012](../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
