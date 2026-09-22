<h1 id="1/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Normalize the candidate distribution by setting

$$
q_r=c2^{-r},\qquad c=\frac1{1-2^{-n}}=\frac{2^n}{2^n-1}.
$$

The supplied [finite sum](../../../../../finite-sum.md) gives its [mean](../../../../../expected-value-split.md)

$$
\sum_{r=1}^nrq_r=c\left(2-(n+2)2^{-n}\right)=\frac{2^{n+1}-(n+2)}{2^n-1}=m.
$$

Thus it meets the [constraint](../../../../../constraint-mechanics.md). Since $\log_2q_r=\log_2c-r$, every other distribution $p$ with [mean](../../../../../expected-value-split.md) $m$ satisfies

$$
d(p,q)=-H(p)-\log_2c+m=H(q)-H(p).
$$

Nonnegativity and the [equality](../../../../../equality-mathematics.md) case in part (a) prove

$$
\boxed{p_Y(r)=\frac{2^n}{2^n-1}\,2^{-r},\qquad H(Y)_{\max}=m-\log_2\frac{2^n}{2^n-1}.}
$$

The [maximum](../../../../../maximum-of-a-subset-of-a-total-order.md) is unique; the [entropy](../../../../../information-entropy-split.md) comparison uses the fixed [mean](../../../../../expected-value-split.md) rather than an unconstrained optimization.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
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
