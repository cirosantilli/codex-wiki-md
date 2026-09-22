<h1 id="a/1/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The two child intervals partition their parent:

$$
B_{n,k}=B_{n+1,2k}\,\dot\cup\,B_{n+1,2k+1}.
$$

Their [preimages](../../../../../../preimage.md) under $g$ satisfy the same identity. Since all $A$ sets lie inside $f(M)$ and $f$ is onto its image, equality of their [preimages](../../../../../../preimage.md) under $f$ implies

$$
A_{n,k}=A_{n+1,2k}\,\dot\cup\,A_{n+1,2k+1}.
$$

On the first child, $h_{n+1}=2k\,2^{-n-1}=k2^{-n}=h_n$; on the second it is $h_n+2^{-n-1}$. Outside the image both functions are zero. Thus

$$
\boxed{0\leq h_{n+1}(t)-h_n(t)\leq2^{-n-1}.}
$$

For $m>n$, summing these bounds gives

$$
|h_m(t)-h_n(t)|\leq\sum_{j=n}^{m-1}2^{-j-1}
\leq2^{-n}.
$$

This tends to zero uniformly in $m>n$, proving that each real sequence $h_n(t)$ is Cauchy and has a finite limit.

## ↑ Ancestors (14)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [A](../../../../a.md)
5. [2007](../../../../../2007-split.md)
6. [Past exam of the martingales and financial mathematics course of the University of Oxford](../../../../../split.md)
7. [Martingales and financial mathematics course of the University of Oxford](../../../../../../martingales-and-financial-mathematics-course-of-the-university-of-oxford.md)
8. [Year 3 of the mathematics course of the University of Oxford](../../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
