<h1 id="14h/solution">Solution</h1>

↑ **Parent:** [14H](../14h.md)

Let $p$ first be an arbitrary degree-$n$ [polynomial](../../../../../polynomial-split.md) with leading coefficient $a_n\ne0$. Choose $R$ so large that on $|z|=R$,

$$
|p(z)-a_nz^n|<|a_n|R^n.
$$

The homotopy $a_nz^n+s[p(z)-a_nz^n]$, $0\le s\le1$, never meets zero on that [circle](../../../../../circle.md). Hence the image curve $p(Re^{i\theta})$ has [winding number](../../../../../winding-number.md) $n$, the same as $a_nR^ne^{in\theta}$. The [argument principle](../../../../../argument-principle.md) counts precisely $n$ zeros inside, with multiplicity, since there are no poles. Choose $R$ large enough that the same leading-term domination holds for every $|z|\ge R$; the lower-term ratios decrease with radius, so this also excludes all exterior zeros. This proves the [fundamental theorem of algebra](../../../../../fundamental-theorem-of-algebra.md) with its multiplicity count. A degree-zero nonzero [polynomial](../../../../../polynomial-split.md) has no zeros.

Now use the specified bound for the monic quartic. Compare $\Gamma$ with the closed curve

$$
\gamma_0(t)=\begin{cases}R^4e^{4\pi it},&0\le t\le1/2,\\R^4,&1/2\le t\le1.\end{cases}
$$

Its first piece travels once counterclockwise around a [circle](../../../../../circle.md), and its second stays at the endpoint, so its [winding number](../../../../../winding-number.md) is one. On the first piece, $|\Gamma-\gamma_0|<R^4$. On the second, both $p(R)$ and $p(iR)$ differ from $R^4$ by less than $R^4$; every convex combination of those errors also has modulus less than $R^4$. Thus the quoted [winding number](../../../../../winding-number.md) stability result gives

$$
\boxed{n(\Gamma,0)=1.}
$$

For real coefficients define $q(y)=y^4-by^2+d$. It has no real zeros and positive leading coefficient, so $q(y)>0$ for every real $y$, including $d=q(0)>0$. Therefore

$$
p(iy)=q(y)+i(cy-ay^3)
$$

lies strictly in the right half-plane for every real $y$. Also $p(x)>0$ for $x\ge0$: there are no zeros there, and the [polynomial](../../../../../polynomial-split.md) is positive for sufficiently large positive $x$. These facts exclude roots on the positive real and imaginary axes.

Consider the positively oriented quarter-disk boundary: first the arc from $R$ to $iR$, then the imaginary axis to zero, then the real axis back to $R$. Under $p$, its last two pieces form a path from $p(iR)$ to $p(R)$ entirely within the right half-plane. The chord closing $\Gamma$ also lies there. Since this half-plane is convex and excludes zero, deforming one closing path into the other changes no [winding number](../../../../../winding-number.md). Thus the full image of the quarter-disk boundary has [winding number](../../../../../winding-number.md) one. By the [argument principle](../../../../../argument-principle.md) there is exactly one root inside that quarter-disk, counted with multiplicity.

Finally, all [polynomial](../../../../../polynomial-split.md) roots lie in $|z|<R$ under the given strict coefficient bound: for $|z|\ge R$, the sum of lower terms divided by $|z|^4$ is smaller than one. Hence

$$
\boxed{\text{exactly one zero lies in the open first quadrant}.}
$$

Its multiplicity is one. This is the [quarter-sector winding test for a real quartic](../../../../../quarter-sector-winding-test-for-a-real-quartic.md); it accounts for the axis exclusions and does not replace the sector boundary by a chord without justifying the deformation.

## ↑ Ancestors (10)

1. [14H](../14h.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
