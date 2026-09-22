<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

First suppose $c_i\ne0$ and put $F=\widehat w/(U-c)$. The wall condition gives $F(\pm L)=0$. Substitution into the [Rayleigh equation for inviscid shear flow](../../../../../../rayleigh-equation-for-inviscid-shear-flow.md) gives

$$
[(U-c)^2F']'-k^2(U-c)^2F=0.
$$

Multiply by $\overline F$ and use [integration by parts](../../../../../../integration-by-parts.md). The resulting [weighted identity for Howard's semicircle theorem](../../../../../../weighted-identity-for-howard-s-semicircle-theorem.md) is

$$
\int_{-L}^L(U-c)^2Q\,dz=0,\qquad Q=|F'|^2+k^2|F|^2,\qquad I=\int Q\,dz>0.
$$

Its imaginary part gives $\int UQ=c_rI$, and its real part then gives $\int U^2Q=(c_r^2+c_i^2)I$. Set $a=U_{\min}$ and $b=U_{\max}$. Since $(U-a)(b-U)\ge0$,

$$
0\le\int(U-a)(b-U)Q\,dz
=\bigl[(a+b)c_r-ab-c_r^2-c_i^2\bigr]I.
$$

Completing the square proves [Howard's semicircle theorem](../../../../../../howard-s-semicircle-theorem.md):

$$
\boxed{\left(c_r-\frac{U_{\max}+U_{\min}}2\right)^2+c_i^2\le\left(\frac{U_{\max}-U_{\min}}2\right)^2.}
$$

In particular every growing [normal mode](../../../../../../normal-mode.md) lies in the upper semicircle for $k>0$. If $c$ is real and outside $[a,b]$, $F$ is again regular, but the same identity has a strictly positive integrand unless the mode vanishes. Such a neutral mode is impossible. Consequently neutral regular modes also satisfy the bound; no division by $c_i$ is needed for this last conclusion. The nonreal proof avoids critical-level singularities altogether.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 331](../../../paper-331-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
