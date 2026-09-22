<h1 id="20/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Take positive dimensions measured in metres. The [volume](../../../../../volume.md) is $V=lwh$ and the external [surface area](../../../../../surface-area.md) constraint is $S=lw+2lh+2wh=12$. There is one base and four walls, with no lid. The [Lagrange multiplier](../../../../../lagrange-multiplier.md) equations for $V-\lambda(S-12)$ are

$$
wh=\lambda(w+2h),\qquad lh=\lambda(l+2h),\qquad lw=2\lambda(l+w).
$$

The first equation implies $\lambda>0$. Multiply the first by $l$ and the second by $w$ and subtract; this gives $2\lambda h(l-w)=0$, hence $l=w=s$. The last equation gives $\lambda=s/4$. Substituting into the first yields $sh=(s/4)(s+2h)$ and therefore $s=2h$.

The constraint now reads $s^2+4sh=3s^2=12$. Thus

$$
\boxed{l=w=2\ \mathrm m,\qquad h=1\ \mathrm m,\qquad V_{\max}=4\ \mathrm{m^3}.}
$$

For a global check, apply the [arithmetic-geometric mean inequality](../../../../../arithmetic-geometric-mean-inequality.md) to $lw$, $2lh$ and $2wh$, whose sum is $12$. Their product is $4V^2\leq4^3=64$, so no feasible box has $V>4$. Equality holds exactly at the dimensions found above. This is the [maximum-volume open rectangular box at fixed surface area](../../../../../maximum-volume-open-rectangular-box-at-fixed-surface-area.md).

## ↑ Ancestors (13)

1. [A](../a.md)
2. [20](../../20.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
