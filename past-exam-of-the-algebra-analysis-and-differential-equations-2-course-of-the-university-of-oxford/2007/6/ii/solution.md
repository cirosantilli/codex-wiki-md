<h1 id="6/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Choose the branch $\operatorname{Log}z=\log|z|+i\arg z$ with $-\pi/2<\arg z<3\pi/2$. It is [holomorphic](../../../../holomorphic-function-split.md) off the downward imaginary ray and takes values $\log x$ on the positive real axis and $\log x+i\pi$ at $-x$ for $x>0$.

Take $R>2$ and $0<\varepsilon<2$. The positively oriented [contour](../../../../complex-integration-contour.md) consists of the real segments $[-R,-\varepsilon]$ and $[\varepsilon,R]$, the small upper semicircle from $-\varepsilon$ to $\varepsilon$ traversed clockwise, and the large upper semicircle from $R$ to $-R$ traversed counterclockwise. For $F(z)=\operatorname{Log}z/(4+z^2)$, the only enclosed [pole](../../../../pole.md) is $2i$, with

$$
\operatorname{Res}_{z=2i}F=\frac{\log2+i\pi/2}{4i}.
$$

The integral over the large arc is $O(\log R/R)$, since its length is $\pi R$ and $|4+z^2|\ge R^2-4$. The small arc contributes $O(\varepsilon|\log\varepsilon|)$, since its length is $\pi\varepsilon$ and $|4+z^2|\ge4-\varepsilon^2$. Both tend to zero.

Let $J=\int_0^\infty\log x/(4+x^2)\,dx$; it converges because $|\log x|$ is integrable near zero and $\log x/x^2$ is integrable at infinity. The two real segments, after substituting $z=-x$ on the negative one, tend to

$$
2J+i\pi\int_0^\infty\frac{dx}{4+x^2}=2J+\frac{i\pi^2}{4}.
$$

The [residue theorem](../../../../residue-theorem.md) therefore gives

$$
2J+\frac{i\pi^2}{4}
=2\pi i\frac{\log2+i\pi/2}{4i}
=\frac\pi2\log2+\frac{i\pi^2}{4}.
$$

Taking real parts yields

$$
\boxed{J=\frac\pi4\log2.}
$$

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [6](../../6.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the algebra, analysis and differential equations II course of the University of Oxford](../../../split.md)
5. [Algebra, analysis and differential equations II course of the University of Oxford](../../../../algebra-analysis-and-differential-equations-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
