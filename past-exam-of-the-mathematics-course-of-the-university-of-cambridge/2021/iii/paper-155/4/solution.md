<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The [Johnson–Lindenstrauss lemma](../../../../../johnson-lindenstrauss-lemma.md) says that for $0<\varepsilon<1$, every set of $N$ points in a Hilbert space admits a linear map into $\ell_2^m$, where $m\leq C\varepsilon^{-2}\log N$, such that every pairwise distance is multiplied by a factor in $[1-\varepsilon,1+\varepsilon]$.

Let $S$ be a maximal $\delta$-separated subset of the unit sphere $S_E$. Maximality makes it a $\delta$-net. The translates $s+(\delta/2)B_E$, $s\in S$, have disjoint interiors and lie in $(1+\delta/2)B_E$. Comparing $n$-dimensional volumes gives

$$
|S|\left(\frac\delta2\right)^n
\leq\left(1+\frac\delta2\right)^n,
$$

so

$$
\boxed{|S|\leq(1+2/\delta)^n\leq(3/\delta)^n}.
$$

Put $M=\|T\|$. For every $x\in S_E$, choose $s\in S$ with $\|x-s\|\leq\delta$. Then

$$
\|Tx\|\leq1+\delta+M\delta,
$$

and taking the supremum gives

$$
M\leq\frac{1+\delta}{1-\delta}.
$$

The reverse triangle inequality gives

$$
\|Tx\|\geq1-\delta-M\delta
\geq\frac{1-3\delta}{1-\delta}>0.
$$

Thus $T$ is injective and the [net estimate for a linear operator](../../../../../net-estimate-for-a-linear-operator.md) yields

$$
\boxed{\|T\|\|T^{-1}\|
\leq\frac{1+\delta}{1-3\delta}}.
$$

For a standard normal $Y$, completing the square gives

$$
\mathbb E e^{u|Y|}
=\frac2{\sqrt{2\pi}}\int_0^\infty e^{uy-y^2/2}\,dy
=2e^{u^2/2}\Phi(u).
$$

With $\beta=\sqrt{2/\pi}$, set

$$
H(u)=\log(2\Phi(u))-\beta u.
$$

Now $H(0)=H'(0)=0$. Its second derivative is bounded above on $[0,1]$, so Taylor's theorem gives $H(u)\leq Cu^2$ there. For $u\geq1$, the elementary bound $\Phi(u)\leq1$ gives

$$
\log\mathbb E e^{u(|Y|-\beta)}
=\frac{u^2}{2}+H(u)\leq Cu^2.
$$

This proves the first [subgaussian concentration of the absolute Gaussian average](../../../../../subgaussian-concentration-of-the-absolute-gaussian-average.md) estimate. The second estimate is supplied in the question.

For fixed $x\ne0$, rotational invariance of a Gaussian vector gives

$$
\sum_{j=1}^nZ_{ij}x_j\overset d=\|x\|_2Y_i,
$$

where the $Y_i$ are independent standard normals. Hence

$$
\frac{\|Tx\|_1}{\|x\|_2}
=\frac1{\beta k}\sum_{i=1}^k|Y_i|.
$$

For the upper tail, the [Chernoff bound](../../../../../chernoff-bound.md) and the preceding moment estimate give

$$
\mathbb P\left(\sum_{i=1}^k(|Y_i|-\beta)\geq\beta\delta k\right)
\leq\exp\bigl(-u\beta\delta k+Cku^2\bigr).
$$

Choosing $u=\beta\delta/(2C)$ gives $e^{-c\delta^2k}$; the supplied negative-moment bound gives the same lower-tail estimate. Therefore

$$
\boxed{\mathbb P\left((1-\delta)\|x\|_2\leq\|Tx\|_1
\leq(1+\delta)\|x\|_2\right)
\geq1-2e^{-c\delta^2k}}.
$$

Fix $\varepsilon>0$ and choose $0<\delta<1/3$ so that

$$
\frac{1+\delta}{1-3\delta}<1+\varepsilon.
$$

Take a $\delta$-net of $S^{n-1}$ with at most $(3/\delta)^n$ points. If $k\geq C_\varepsilon n$, the union bound and the concentration estimate show that with positive probability the random map satisfies the required inequalities simultaneously on the net. The net estimate then proves the [Almost-isometric Gaussian embedding from l2 into l1](../../../../../almost-isometric-gaussian-embedding-from-l2-into-l1.md) with distortion below $1+\varepsilon$.

For the final claim, first apply the [Bourgain embedding theorem](../../../../../bourgain-embedding-theorem.md) to the given $n$-point metric space, obtaining distortion $O(\log n)$ in Euclidean dimension $O((\log n)^2)$. Apply the [Johnson–Lindenstrauss lemma](../../../../../johnson-lindenstrauss-lemma.md) to its $n$ image points, reducing the dimension to $m=O(\log n)$ at constant additional distortion. Finally apply the preceding Gaussian construction with $k=O(m)=O(\log n)$. The composition proves the [Low-dimensional L1 embedding of a finite metric space](../../../../../low-dimensional-l1-embedding-of-a-finite-metric-space.md):

$$
\boxed{k\leq C\log n,
\qquad \operatorname{dist}(F)\leq C\log n}.
$$

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 155](../../paper-155-split.md)
3. [Iii](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
