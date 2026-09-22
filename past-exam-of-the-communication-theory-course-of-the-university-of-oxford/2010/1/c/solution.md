<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For the nontrivial case $a\geq2$, every $p_r<1$ and

$$
l_r=\lceil-\log_2p_r\rceil\geq1.
$$

The [probability](../../../../probability.md) ordering makes $l_1\leq\cdots\leq l_a$. At a dyadic number, choose the terminating [binary expansion](../../../../binary-expansion.md) followed by zeros. Let $c_r$ be the first $l_r$ bits of $t_r$, and let

$$
J_r=\left[\frac{\lfloor2^{l_r}t_r\rfloor}{2^{l_r}},
\frac{\lfloor2^{l_r}t_r\rfloor+1}{2^{l_r}}\right)
$$

be its binary cylinder interval.

Suppose $r<s$ and $c_r$ were a prefix of $c_s$. Since $l_r\leq l_s$, the numbers $t_r$ and $t_s$ would have the same first $l_r$ bits, so both would lie in $J_r$. In particular $t_s-t_r<2^{-l_r}$. But

$$
t_s-t_r=\sum_{i=r}^{s-1}p_i\geq p_r\geq2^{-l_r},
$$

a contradiction. A later word cannot be a shorter prefix of an earlier word because the lengths are nondecreasing; equal-length coincidences were also excluded. Thus the [cumulative Shannon code](../../../../cumulative-shannon-code.md) is a [prefix code](../../../../prefix-code.md).

The ceiling inequalities give

$$
-\log_2p_r\leq l_r<-\log_2p_r+1.
$$

Multiply by $p_r$ and [sum](../../../../sum.md) to obtain

$$
\boxed{H(X)\leq\mathbb EL<H(X)+1.}
$$

For a one-symbol deterministic source the displayed construction assigns the empty word and gives $H=\mathbb EL=0$. This zero-bit convention is valid when the number of source emissions is supplied separately. It is not an unframed [uniquely decodable code](../../../../decipherable-code.md): concatenating different numbers of empty words gives the same bit string. If positive-length unframed words are required, the shortest deterministic code has length $1$, so the strict upper bound $\mathbb EL<H+1$ requires the nontrivial-source assumption.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [2010](../../../2010-split.md)
4. [Past exam of the communication Theory course of the University of Oxford](../../../split.md)
5. [Communication Theory course of the University of Oxford](../../../../communication-theory-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
