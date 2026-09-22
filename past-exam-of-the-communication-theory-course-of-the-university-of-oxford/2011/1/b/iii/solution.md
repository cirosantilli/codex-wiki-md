<h1 id="1/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The given logarithmic moment is

$$
\ell=\frac2{n(n+1)}\sum_{r=1}^nr\log_2r,
$$

where the $r=1$ term is zero. It is attained by the positive distribution

$$
q_r=\frac{2r}{n(n+1)},
$$

whose [probabilities](../../../../../probability.md) [sum](../../../../../sum.md) to one. Write $A=2/[n(n+1)]$, so $\log_2q_r=\log_2A+\log_2r$. For any distribution $p$ with the required logarithmic moment,

$$
d(p,q)=-H(p)-\log_2A-\ell=H(q)-H(p).
$$

Consequently the unique maximizer and its [entropy](../../../../../information-entropy-split.md) are

$$
\boxed{p_Z(r)=\frac{2r}{n(n+1)},\qquad H(Z)_{\max}=\log_2\frac{n(n+1)}2-\ell.}
$$

The increasing weights are consistent with the prescribed moment; they need not be a decreasing [power law](../../../../../power-law.md).

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the communication Theory course of the University of Oxford](../../../../split.md)
6. [Communication Theory course of the University of Oxford](../../../../../communication-theory-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
