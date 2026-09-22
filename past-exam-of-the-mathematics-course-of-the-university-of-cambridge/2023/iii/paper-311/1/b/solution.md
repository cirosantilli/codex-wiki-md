<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Define [Ingoing BTZ coordinates](../../../../../../ingoing-btz-coordinates.md) by

$$
dv=dt+\frac{dr}{f(r)},
\qquad
d\chi=d\phi+\frac{\Omega(r)}{f(r)}\,dr.
$$

Thus $dt=dv-dr/f$ and $d\phi=d\chi-\Omega\,dr/f$, so the potentially singular terms cancel:

$$
d\phi-\Omega dt=d\chi-\Omega dv,
$$

and

$$
-f\left(dv-\frac{dr}{f}\right)^2+\frac{dr^2}{f}
=-f\,dv^2+2\,dv\,dr.
$$

The metric becomes

$$
\boxed{ds^2=-f(r)dv^2+2\,dv\,dr
+r^2[d\chi-\Omega(r)dv]^2}.
$$

For $r_+>r_-$, antiderivatives may be chosen as

$$
v=t+\frac{L^2}{2(r_+^2-r_-^2)}
\left[r_+\log\left|\frac{r-r_+}{r+r_+}\right|
-r_-\log\left|\frac{r-r_-}{r+r_-}\right|\right]
$$

and

$$
\chi=\phi+\frac{L}{2(r_+^2-r_-^2)}
\left[r_-\log\left|\frac{r-r_+}{r+r_+}\right|
-r_+\log\left|\frac{r-r_-}{r+r_-}\right|\right],
$$

with the extremal case obtained by taking the limit. The transformed metric contains neither $1/f$ nor any other singular coefficient at $r=r_+$; since $f$, $\Omega$, and $r^2$ are analytic there, it gives an analytic extension across the outer horizon.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 311](../../../paper-311-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
