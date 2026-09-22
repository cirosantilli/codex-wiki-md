# Hilbert-Serre theorem

↑ **Parent:** [Hilbert series](hilbert-series.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hilbert-Serre_theorem)

Let $S=k[x_1,\ldots,x_r]$ be graded with positive degrees $d_i=\deg x_i$, and let $M$ be a finitely generated graded $S$-module with finite-dimensional graded pieces. Then

$$
H_M(t)=\frac{P(t)}{\prod_{i=1}^r(1-t^{d_i})}
$$

for a Laurent polynomial $P(t)\in\mathbb Z[t,t^{-1}]$. For a standard grading, $\dim_kM_n$ consequently agrees with a polynomial for all sufficiently large $n$.

The proof is by induction on $r$. For $x=x_r$ of degree $d$, the exact sequence of graded modules

$$
0\longrightarrow(0:_Mx)(-d)\longrightarrow M(-d)
\xrightarrow{x}M\longrightarrow M/xM\longrightarrow0
$$

gives

$$
(1-t^d)H_M(t)=H_{M/xM}(t)-t^dH_{(0:_Mx)}(t).
$$

Both modules on the right are finitely generated over $k[x_1,\ldots,x_{r-1}]$, so induction supplies the asserted denominator.

**Table of contents**

- [Hilbert-Serre theorem for an additive coefficient function](hilbert-serre-theorem-for-an-additive-coefficient-function.md)
- [Hilbert series multiplication exact sequence](hilbert-series-multiplication-exact-sequence.md)
- [Growth of a finitely generated commutative algebra](growth-of-a-finitely-generated-commutative-algebra.md)
  - [Growth of the two-variable Laurent polynomial algebra](growth-of-the-two-variable-laurent-polynomial-algebra.md)

## ↑ Ancestors (9)

1. [Hilbert series](hilbert-series.md)
2. [Hilbert series and Hilbert polynomial](hilbert-series-and-hilbert-polynomial.md)
3. [Graded ring](graded-ring.md)
4. [Ring](ring.md)
5. [Commutative algebra](commutative-algebra-split.md)
6. [Algebra](algebra-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (16)

- [Dimension of a filtered module](dimension-of-a-filtered-module.md)
- [Growth of a finitely generated commutative algebra](growth-of-a-finitely-generated-commutative-algebra.md)
- [Hilbert series multiplication exact sequence](hilbert-series-multiplication-exact-sequence.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-2/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-2/3/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-2/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-2/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-1/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-1/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-1/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-101/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-128/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-148/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-101/5/a/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-101/5/c/iv/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-101/5/ii/solution.md)
