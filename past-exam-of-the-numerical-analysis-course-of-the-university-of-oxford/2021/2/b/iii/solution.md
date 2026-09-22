<h1 id="2/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

**No. Distinct [singular values](../../../../../singular-value.md) do not force uniqueness in the [spectral norm](../../../../../matrix-2-norm.md).** For an explicit example take

$$
A=\begin{pmatrix}2&0\\0&1\end{pmatrix},\qquad
B_t=\begin{pmatrix}2+t&0\\0&0\end{pmatrix},\qquad -1\leq t\leq1.
$$

The [singular values](../../../../../singular-value.md) of $A$ are $2>1>0$. Every $B_t$ has [matrix rank](../../../../../matrix-rank.md) one, and its error in the [spectral norm](../../../../../matrix-2-norm.md) is

$$
\boxed{\|A-B_t\|_2=\max\{|t|,1\}=1=\sigma_2(A).}
$$

Thus there are infinitely many best rank-one approximations even with a strict gap between the [singular values](../../../../../singular-value.md).

The same mechanism works for every $1\leq r<n$ under the question's positive [singular values](../../../../../singular-value.md). Starting with $A_r$, define

$$
B_t=A_r+t u_1v_1^T,\qquad |t|\leq\sigma_{r+1}.
$$

When the [singular values](../../../../../singular-value.md) are distinct, $\sigma_1+t\geq\sigma_1-\sigma_{r+1}>0$, so every $B_t$ has [matrix rank](../../../../../matrix-rank.md) $r$, while

$$
\|A-B_t\|_2=\max\{|t|,\sigma_{r+1}\}=\sigma_{r+1}.
$$

The [spectral norm](../../../../../matrix-2-norm.md) measures only the largest remaining [singular value](../../../../../singular-value.md), leaving room to change retained components without increasing that maximum. This is the [nonuniqueness of spectral-norm low-rank approximation](../../../../../nonuniqueness-of-spectral-norm-low-rank-approximation.md). The exceptional case $r=0$ is unique for the elementary reason given above.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the numerical analysis course of the University of Oxford](../../../../split.md)
6. [Numerical analysis course of the University of Oxford](../../../../../numerical-analysis-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
