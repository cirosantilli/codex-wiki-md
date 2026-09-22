<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Set $N=|\mathcal X|$, $d_i=|p_i-q_i|$ and $d=\sum_i d_i=\|p-q\|_1$. If $d=0$, the two [probability mass functions](../../../../probability-mass-function.md) agree and the bound is zero. Otherwise every $d_i\leq d\leq1/2$. The half-interval [entropy summand](../../../../entropy-summand.md) bound, with $t=\min(p_i,q_i)$ and $v=d_i$, gives

$$
|f(p_i)-f(q_i)|\leq f(d_i).
$$

By the [triangle inequality](../../../../triangle-inequality.md), followed by [Jensen's inequality](../../../../jensen-s-inequality.md) for the [concave function](../../../../concave-function.md) $f$,

$$
\begin{aligned}
|H(p)-H(q)|
&\leq\sum_{i=1}^N|f(p_i)-f(q_i)|
\leq\sum_{i=1}^Nf(d_i)\\
&\leq Nf\left(\frac1N\sum_{i=1}^Nd_i\right)
=-d\log\frac dN.
\end{aligned}
$$

This proves the requested [finite-alphabet entropy continuity bound](../../../../finite-alphabet-entropy-continuity-bound.md):

$$
\boxed{|H(p)-H(q)|\leq-\|p-q\|_1\log\left(\frac{\|p-q\|_1}{|\mathcal X|}\right).}
$$

## ↑ Ancestors (12)

1. [D](../d.md)
2. [1](../../1.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the information theory course of the University of Oxford](../../../split.md)
5. [Information theory course of the University of Oxford](../../../../information-theory-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
