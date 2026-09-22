<h1 id="15f/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

By the [Bromwich inversion formula](../../../../../../bromwich-inversion-formula.md), for $t>0$ and $\gamma>0$,

$$
f(t)=\frac1{2\pi i}\int_{\gamma-i\infty}^{\gamma+i\infty}\frac{e^{st}}{s^2(s+1)^2}\,ds.
$$

Close the upward vertical segment by a left semicircle of radius $R$ centred at $\gamma$. On that arc $\operatorname{Re}s\le\gamma$, so $|e^{st}|\le e^{\gamma t}$, while $|s^2(s+1)^2|$ is bounded below by a constant times $R^4$ for large $R$. Its length is $\pi R$, hence the arc [integral](../../../../../../integral.md) tends to zero as $O(R^{-3})$. The [contour](../../../../../../complex-integration-contour.md) is positively oriented and encloses the [double poles](../../../../../../double-pole.md) at $0$ and $-1$.

Their [residues](../../../../../../residue.md) are

$$
\operatorname{Res}_{s=0}\frac{e^{st}}{s^2(s+1)^2}=\left.\frac d{ds}\frac{e^{st}}{(s+1)^2}\right|_{s=0}=t-2,
$$

and

$$
\operatorname{Res}_{s=-1}\frac{e^{st}}{s^2(s+1)^2}=\left.\frac d{ds}\frac{e^{st}}{s^2}\right|_{s=-1}=(t+2)e^{-t}.
$$

The [residue theorem](../../../../../../residue-theorem.md) therefore yields

$$
\boxed{f(t)=t-2+(t+2)e^{-t}\qquad(t\ge0).}
$$

The value at zero follows by [continuity](../../../../../../continuous-function.md) and is $f(0)=0$.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [15F](../../15f.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
