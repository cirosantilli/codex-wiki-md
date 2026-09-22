# Jordan decomposition of a function of bounded variation

↑ **Parent:** [Total variation of a function](total-variation-of-a-function.md)

Every real [function](function-split.md) on $[a,b]$ has [bounded variation](total-variation-of-a-function.md) if and only if it is a difference of two [nondecreasing functions](nondecreasing-function.md). For a normalized version, let $v(t)=V_a^t(f)$ and $v(a)=0$. Its accumulated positive and negative variations are

$$
P(t)=\frac{v(t)+f(t)-f(a)}2,\qquad
N(t)=\frac{v(t)-f(t)+f(a)}2.
$$

Both are [nondecreasing functions](nondecreasing-function.md), $P(a)=N(a)=0$, and

$$
f(t)=f(a)+P(t)-N(t),\qquad v(t)=P(t)+N(t).
$$

This is the [Jordan decomposition of a function of bounded variation](jordan-decomposition-of-a-function-of-bounded-variation.md).[§3.5.2, Definition 9, Lemma 12, Exercise 13 and Theorem 14, printed pp. 3–5: positive and negative variation and Jordan decomposition](real-analysis-lecture-notes-3-5-functions-of-bounded-variation-by-christopher-e-heil.md) Equivalently one may write $f=f_+-f_-$ with $f_+=(v+f)/2$ and $f_-=(v-f)/2$; those functions need not vanish at $a$.

For the [piecewise linear function](piecewise-linear-function.md) in [partition example of total variation](partition-example-of-total-variation.md), the successive values of $P$ are $0,2,2,6,6$, while those of $N$ are $0,0,3,3,5$. At $t=4$, the total rise is $6$ and the total fall is $5$: their difference gives the net change $1$, and their sum gives the total variation $11$. A declining segment increases $N$ while $P$ stays constant; an ascending segment does the opposite.

For a short proof outline, total variation is additive over adjacent [intervals](interval-mathematics.md), because any two [partitions of an interval](partition-of-an-interval.md) have a common [partition refinement](partition-refinement.md). Thus $v(t)-v(s)=V_s^t(f)\geq|f(t)-f(s)|$ for $s<t$. Substituting this inequality into the formulas for $P$ and $N$ shows their increments are nonnegative. Conversely, if $f=g-h$ for two [nondecreasing functions](nondecreasing-function.md), the [triangle inequality](triangle-inequality.md) bounds each partition sum by $g(b)-g(a)+h(b)-h(a)$. This proves finite total variation without restricting the number of changes of direction.

## ↑ Ancestors (7)

1. [Total variation of a function](total-variation-of-a-function.md)
2. [Riemann integration](riemann-integration.md)
3. [Real analysis](real-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (5)

- [History of total variation of a function](history-of-total-variation-of-a-function.md)
- [Jordan decomposition of a function of bounded variation](jordan-decomposition-of-a-function-of-bounded-variation.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-202/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-202/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-202/1/c/solution.md)
