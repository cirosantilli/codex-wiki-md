<h1 id="5/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

[Periodicity](../../../../periodicity.md) reduces all the indicated vertical segments to the [compact](../../../../compact-space.md) segment $1/2+i[-1,1]$, which misses every pole. [Continuity](../../../../continuous-function.md) therefore gives the first uniform bound. In fact an explicit identity gives a stronger estimate for every real $y$:

$$
g(m+1/2+iy)=-i\pi\tanh(\pi y),\qquad |g(m+1/2+iy)|\leq\pi.
$$

Thus we can take $D_1=\pi$.

Write $L=m+1/2$. On the vertical sides of the square the same bound holds, since both real coordinates are half-integers. On either horizontal side $|\operatorname{Im}z|=L\geq1/2$. For $\operatorname{Im}z=y>0$, put $w=e^{2\pi iz}$, so $|w|=e^{-2\pi y}$. Using

$$
\cot(\pi z)=i\frac{w+1}{w-1}
$$

gives $|g(z)|\leq\pi(1+e^{-2\pi y})/(1-e^{-2\pi y})\leq\pi\coth(\pi/2)$. [Conjugation](../../../../conjugation.md) gives the same estimate below the real axis. Hence an explicit bound valid on every square is

$$
\boxed{D_2=\pi\coth(\pi/2).}
$$

For $L>|b|$, the [contour](../../../../complex-integration-contour.md) has length $8L$ and every point on it has $|z|\geq L$. The [reverse triangle inequality](../../../../reverse-triangle-inequality.md) yields $|z^2-b^2|\geq L^2-b^2$, so the [ML inequality](../../../../estimation-lemma.md) gives

$$
\left|\int_{\gamma_m}\frac{g(z)}{z^2-b^2}\,dz\right|
\leq\frac{8LD_2}{L^2-b^2}\longrightarrow0.
$$

Orient the square positively. Its enclosed poles at the integers $-m,\ldots,m$ have [residues](../../../../residue.md) $1/(n^2-b^2)$. Since $b$ is nonintegral, the additional poles $b$ and $-b$ are distinct from those integers and from one another. Their [residues](../../../../residue.md) are $g(b)/(2b)$ and $g(-b)/(-2b)$, both equal to $g(b)/(2b)$ because $g$ is odd. Their combined contribution is therefore $\pi\cot(\pi b)/b$.

The [residue theorem](../../../../residue-theorem.md) gives

$$
\frac1{2\pi i}\int_{\gamma_m}\frac{g(z)}{z^2-b^2}\,dz
=-\frac1{b^2}+2\sum_{n=1}^m\frac1{n^2-b^2}+\frac{\pi\cot(\pi b)}b.
$$

The series is [absolutely convergent](../../../../absolute-convergence.md), since its terms are $O(n^{-2})$. Taking the limit, then including the $n=0$ term, yields

$$
\boxed{\sum_{n=0}^{\infty}\frac1{n^2-b^2}=-\frac1{2b^2}-\frac{\pi\cot(\pi b)}{2b},\qquad b\in\mathbb R\setminus\mathbb Z.}
$$

This is [cotangent contour summation](../../../../cotangent-contour-summation.md). Keeping the $n=0$ term separate until the last step determines the sign of the $1/(2b^2)$ contribution.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [5](../../5.md)
3. [2013](../../../2013-split.md)
4. [Past exam of the algebra and analysis II for mathematics and philosophy course of the University of Oxford](../../../split.md)
5. [Algebra and analysis II for mathematics and philosophy course of the University of Oxford](../../../../algebra-and-analysis-ii-for-mathematics-and-philosophy-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics and philosophy course of the University of Oxford](../../../../year-2-of-the-mathematics-and-philosophy-course-of-the-university-of-oxford.md)
7. [Mathematics and philosophy course of the University of Oxford](../../../../mathematics-and-philosophy-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
