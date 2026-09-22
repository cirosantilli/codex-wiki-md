<h1 id="1/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Let $P=b(T)q(T)$ and $Q=a(T)p(T)$. By part (ii), these are complementary [projection operators](../../../../../projection-linear-algebra.md) with images $U=\ker(T-\lambda I)^\alpha$ and $W=\ker(T-\mu I)^\beta$. Thus $D=\lambda P+\mu Q$ acts as $\lambda I$ on $U$ and $\mu I$ on $W$.

The [linear operator](../../../../../linear-operator.md) $T$ preserves both summands because it commutes with its own polynomials. Therefore $N=T-D$ preserves them too, and its restrictions satisfy

$$
N|_U=(T-\lambda I)|_U,\quad (N|_U)^\alpha=0,\qquad
N|_W=(T-\mu I)|_W,\quad (N|_W)^\beta=0.
$$

Put $k=\max(\alpha,\beta)$. Both restrictions of $N^k$ vanish, so the [direct sum](../../../../../direct-sum.md) gives

$$
\boxed{(T-D)^k=0.}
$$

Hence **$T-D$ is a [nilpotent linear map](../../../../../nilpotent-linear-map.md)**. The operator $D$ is [diagonalizable](../../../../../diagonalizable-matrix.md), since its two summands are its [eigenspaces](../../../../../eigenspace.md), and it commutes with $T$. This illustrates the [Jordan–Chevalley decomposition](../../../../../jordan-chevalley-decomposition.md) in the case of two distinct eigenvalues.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [2014](../../../../2014-split.md)
5. [Past exam of the algebra 1 and differential equations 1 course of the University of Oxford](../../../../split.md)
6. [Algebra 1 and differential equations 1 course of the University of Oxford](../../../../../algebra-1-and-differential-equations-1-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
