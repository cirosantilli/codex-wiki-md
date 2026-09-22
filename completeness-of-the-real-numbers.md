# Completeness of the real numbers

↑ **Parent:** [Cauchy sequence](cauchy-sequence.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Completeness_of_the_real_numbers)

Every [Cauchy sequence](cauchy-sequence.md) of [real numbers](real-number.md) converges to a [real number](real-number.md). Explicitly, the condition

$$
\forall\varepsilon>0\;\exists N\in\mathbb N_{>0}\;\forall m,n\geq N:\quad |x_m-x_n|<\varepsilon
$$

implies the existence of $L\in\mathbb R$ with $x_n\to L$. The hypothesis compares approximations with one another, without requiring a candidate answer. This makes [completeness of the real numbers](completeness-of-the-real-numbers.md) an existence principle: sufficiently consistent approximations cannot approach a missing destination. [MIT 18.100A, Lecture 10, theorem 7](https://ocw.mit.edu/courses/18-100a-real-analysis-fall-2020/mit18_100af20_lec102.pdf).

The equivalent [least-upper-bound property](least-upper-bound-property.md) says that every nonempty [set](set-split.md) $A\subseteq\mathbb R$ bounded above has a [supremum](supremum.md) $s\in\mathbb R$. Precisely, every $x\in A$ satisfies $x\leq s$, and for every $\varepsilon>0$ some $x\in A$ satisfies $s-\varepsilon<x$. The second condition excludes any smaller [upper bound](upper-bound-in-a-partially-ordered-set.md). No largest element of $A$ is required.

The [rational numbers](rational-number.md) lack this property. The [set](set-split.md) $A=\{q\in\mathbb Q:q\geq0,\ q^2<2\}$ contains one and has [upper bound](upper-bound-in-a-partially-ordered-set.md) two, but has no [supremum](supremum.md) in $\mathbb Q$. A proposed rational [supremum](supremum.md) $s$ would have to satisfy $s^2=2$: if $s^2<2$, a sufficiently small rational increase still lies in $A$; if $s^2>2$, a sufficiently small rational decrease remains an [upper bound](upper-bound-in-a-partially-ordered-set.md). The [irrationality of the square root of two](irrationality-of-the-square-root-of-two.md) excludes equality. In $\mathbb R$, its [supremum](supremum.md) is $\sqrt2$. [MIT 18.100A, Lecture 3, theorems 14–15](https://ocw.mit.edu/courses/18-100a-real-analysis-fall-2020/mit18_100af20_lec32.pdf).

Construct this [square root](square-root.md) by the [bisection method](bisection-method.md), starting with rational bounds $[l_0,u_0]=[1,2]$. At each step square the midpoint and retain the half whose endpoints bracket two after squaring. The first four resulting [intervals](interval-mathematics.md) are $[1,3/2]$, $[5/4,3/2]$, $[11/8,3/2]$, and $[11/8,23/16]$. After $k$ steps, $u_k-l_k=2^{-k}$ and $l_k^2<2<u_k^2$. Both endpoint [sequences](sequence.md) are [Cauchy sequences](cauchy-sequence.md) because every later endpoint remains in the current [interval](interval-mathematics.md). [Completeness of the real numbers](completeness-of-the-real-numbers.md) gives a common [limit of a sequence](limit-of-a-sequence.md) $L$; [continuity](continuous-function.md) of squaring gives $L^2=2$. The midpoint approximates $L$ with error at most $2^{-(k+1)}$. Thus exact rational arithmetic produces certified accuracy while [completeness of the real numbers](completeness-of-the-real-numbers.md) supplies the exact answer.

[Richard Dedekind](richard-dedekind.md) approached [completeness of the real numbers](completeness-of-the-real-numbers.md) by filling gaps in the [rational numbers](rational-number.md) with [Dedekind cuts](dedekind-cut.md). In the preface to his 1872 Continuity and Irrational Numbers, he traced the problem to teaching [differential calculus](differential-calculus.md) in 1858 and wanting arithmetic foundations for [limits](limit-of-a-function.md). His construction makes a missing boundary, such as $\sqrt2$, into a [number](number.md) defined by the separation it produces among [rational numbers](rational-number.md). [Dedekind, Continuity and Irrational Numbers, preface and §§III–IV; Beman's 1901 translation](https://www.gutenberg.org/files/21016/21016-pdf.pdf).

**Table of contents**

- [Dedekind cut](dedekind-cut.md)
- [Least-upper-bound property](least-upper-bound-property.md)

## ↑ Ancestors (7)

1. [Cauchy sequence](cauchy-sequence.md)
2. [Sequence and series](sequence-and-series.md)
3. [Real analysis](real-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (18)

- [Assumptions of the bounded monotone sequence theorem](assumptions-of-the-bounded-monotone-sequence-theorem.md)
- [Bounded monotone sequence theorem](bounded-monotone-sequence-theorem.md)
- [Cauchy sequence](cauchy-sequence.md)
- [Completeness of the real numbers](completeness-of-the-real-numbers.md)
- [Convergence from arbitrary variable-lag increments](convergence-from-arbitrary-variable-lag-increments.md)
- [Infimum and supremum](infimum-and-supremum.md)
- [Least-upper-bound property](least-upper-bound-property.md)
- [Nested-bracket proof of the intermediate value theorem](nested-bracket-proof-of-the-intermediate-value-theorem.md)
- [Nested interval theorem](nested-interval-theorem.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ia/paper-1/10c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ia/paper-1/9c/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ia/paper-1/9c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ia/paper-1/9e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ia/paper-1/10e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/ia/paper-1/10d/iv/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ib/paper-3/12g/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ia/paper-1/9d/c/solution.md)
- [Real analysis](real-analysis-split.md)
