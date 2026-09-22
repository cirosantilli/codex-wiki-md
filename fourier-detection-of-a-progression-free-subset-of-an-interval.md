# Fourier detection of a progression-free subset of an interval

↑ **Parent:** [Roth density-increment step](roth-density-increment-step.md)

Let $I=[n]$ for odd $n\geq3$, embed it in the [cyclic group](cyclic-group.md) $G=\mathbb Z/(2n+1)\mathbb Z$, and let $A\subseteq I$ have [density of a finite subset](density-of-a-finite-subset.md) $\alpha$. If $A$ has no nonconstant three-term [arithmetic progression](arithmetic-progression.md) and $n\geq4\alpha^{-2}$, its balanced [indicator function](indicator-function.md) $f=1_A-\alpha1_I$ satisfies

$$
\max_{r\ne0}|\widehat f(r)|\geq\alpha^2/36,
\qquad \widehat f(r)=\mathbb E_{x\in G}f(x)e^{-2\pi irx/|G|}.
$$

Indeed, the normalized trilinear [arithmetic progression](arithmetic-progression.md) count has the [Fourier analysis on a finite abelian group](normalized-fourier-analysis-on-a-finite-abelian-group.md) formula $\Lambda(h_1,h_2,h_3)=\sum_r\widehat h_1(r)\widehat h_2(-2r)\widehat h_3(r)$. Its values on $1_A$ and $\alpha1_I$ are $\alpha n/|G|^2$ and $\alpha^3(n^2+1)/(2|G|^2)$. Telescoping their difference into three terms containing $f$, the [Parseval identity](parseval-identity.md) and [Cauchy-Schwarz inequality](cauchy-schwarz-inequality.md) bound its magnitude by $3\max|\widehat f|\alpha n/|G|$. The difference is at least $\alpha^3n^2/(4|G|^2)$, giving the claim. The zero [Fourier coefficient](fourier-coefficient.md) vanishes by the definition of $\alpha$.

## ↑ Ancestors (7)

1. [Roth density-increment step](roth-density-increment-step.md)
2. [Density increment](density-increment.md)
3. [Additive combinatorics](additive-combinatorics-split.md)
4. [Combinatorics](combinatorics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-79/1/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-129/1/solution.md)
