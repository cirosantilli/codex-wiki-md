<h1 id="o/o4/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The two totals are independent, with $n\sim\operatorname{Bin}(2N,q)$ and $m\sim\operatorname{Bin}(2M,p)$. Their joint likelihood is

$$
L(p,q)=\binom{2N}nq^n(1-q)^{2N-n}
\binom{2M}mp^m(1-p)^{2M-m}.
$$

Differentiating the separated [log-likelihood](../../../../../../log-likelihood.md) gives

$$
\boxed{\widehat p=\frac m{2M},\qquad\widehat q=\frac n{2N}.}
$$

These formulas include all-zero or all-one totals as boundary maxima. For interior $p,q$, the [Fisher information](../../../../../../fisher-information-matrix.md) in the ordered parameter vector $(p,q)$ is

$$
\mathcal I(p,q)=\begin{pmatrix}
\dfrac{2M}{p(1-p)}&0\\[2mm]
0&\dfrac{2N}{q(1-q)}
\end{pmatrix}.
$$

The off-diagonal entries vanish because the likelihood separates, and the two estimates are independent even at finite sample size. For large $M,N$, their joint distribution is approximately

$$
\boxed{\begin{pmatrix}\widehat p\\\widehat q\end{pmatrix}
\sim N\left(\begin{pmatrix}p\\q\end{pmatrix},
\begin{pmatrix}p(1-p)/(2M)&0\\0&q(1-q)/(2N)\end{pmatrix}\right).}
$$

## ↑ Ancestors (14)

1. [I](../i.md)
2. [B](../../b.md)
3. [O4](../../../o4.md)
4. [O](../../../../o.md)
5. [2010](../../../../../2010-split.md)
6. [Past exam of the options II course of the University of Oxford](../../../../../split.md)
7. [Options II course of the University of Oxford](../../../../../../options-ii-course-of-the-university-of-oxford.md)
8. [Year 2 of the mathematics course of the University of Oxford](../../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
