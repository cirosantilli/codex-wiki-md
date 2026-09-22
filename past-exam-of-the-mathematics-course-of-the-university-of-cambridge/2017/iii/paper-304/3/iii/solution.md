<h1 id="3/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Put $I_r=\int_{\Lambda<|q|<\Lambda_0}d^6q\,(2\pi)^{-6}(q^2+m^2)^{-r}$, the [scalar shell integral in six dimensions](../../../../../../scalar-shell-integral-in-six-dimensions.md). Each of the three boxes is $g^4I_4$ as a connected insertion. To fix the effective-action sign and avoid a factorial ambiguity, use the [one-loop scalar effective action](../../../../../../one-loop-scalar-effective-action.md):

$$
\frac12\operatorname{Tr}\log(D+g\phi)=\frac12\operatorname{Tr}\log D+\frac12\sum_{r\ge1}\frac{(-1)^{r+1}g^r}{r}\operatorname{Tr}(D^{-1}\phi)^r,\qquad D=-\partial^2+m^2.
$$

For a constant background the fourth-order density is $-g^4I_4\phi^4/8$. Thus the [cubic scalar box contribution to a quartic coupling](../../../../../../cubic-scalar-box-contribution-to-a-quartic-coupling.md) is $\delta g_4=-3g^4I_4$, whose vertex insertion is $-\delta g_4=+3g^4I_4$.

Using the supplied area of the unit five-sphere,

$$
I_4=\frac1{64\pi^3}\int_\Lambda^{\Lambda_0}\frac{q^5\,dq}{(q^2+m^2)^4}=\frac1{128\pi^3}\left[G(\Lambda^2+m^2)-G(\Lambda_0^2+m^2)\right],
$$

where $G(u)=u^{-1}-m^2u^{-2}+m^4/(3u^3)$. This follows by substituting $u=q^2+m^2$ and integrating $(u-m^2)^2/(2u^4)$. Hence

$$
\boxed{\delta g_4=-\frac{3g^4}{128\pi^3}\left[G(\Lambda^2+m^2)-G(\Lambda_0^2+m^2)\right].}
$$

As a check, the massless limit at positive $\Lambda$ is $-3g^4(\Lambda^{-2}-\Lambda_0^{-2})/(128\pi^3)$. Both versions have [mass dimension](../../../../../../mass-dimension.md) minus two, as a six-dimensional local quartic coupling must.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [3](../../3.md)
3. [Paper 304](../../../paper-304-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
