<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Assume independent physical-qubit errors with common [probability](../../../../../../probability.md) $p$, ideal encoding and recovery, and the specified rule that every block with two or more errors fails. The number of physical errors has a [binomial distribution](../../../../../../binomial-distribution.md) with parameters $5,p$. Correct recovery occurs for zero or one error, so

$$
\boxed{P_{\mathrm{correct}}=(1-p)^5+5p(1-p)^4=(1-p)^4(1+4p).}
$$

The corresponding logical failure [probability](../../../../../../probability.md) is

$$
f(p)=1-P_{\mathrm{correct}}=10p^2-20p^3+15p^4-4p^5.
$$

An unencoded [qubit](../../../../../../qubit.md) succeeds with [probability](../../../../../../probability.md) $1-p$. Thus encoding improves this [probability](../../../../../../probability.md) precisely when $f(p)<p$. Factoring gives

$$
f(p)-p=p(1-p)(4p^3-11p^2+9p-1).
$$

On $0<p<1$, the sign is the sign of $g(p)=4p^3-11p^2+9p-1$. Its derivative is $12p^2-22p+9$: it is positive until $(11-\sqrt{13})/12$ and negative afterwards on $[0,1]$. Since $g(0)=-1$, $g(1)=1$ and its interior maximum is positive, there is exactly one zero in $(0,1)$. The [five-qubit concatenation threshold](../../../../../../five-qubit-concatenation-threshold.md) is therefore

$$
\boxed{4p_*^3-11p_*^2+9p_*-1=0,\qquad p_*\simeq0.1311231479,\qquad 0<p<p_*\ \text{improves recovery}.}
$$

At $p=p_*$ the two success [probabilities](../../../../../../probability.md) agree; above it this decoder makes the error rate worse. At $p=0$ both schemes succeed perfectly, and at $p=1$ both fail under the stated error model. The small-$p$ behavior $f(p)=10p^2+O(p^3)$ exhibits cancellation of every single-qubit-error contribution.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 58](../../../paper-58-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
