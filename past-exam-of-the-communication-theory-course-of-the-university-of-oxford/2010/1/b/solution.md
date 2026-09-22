<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $S=\sum_{k=1}^a2^{-l_k}$ and let $l_{\max}$ be the largest length. Expanding $S^n$ sums $2^{-L}$ over all strings of $n$ source symbols, where $L$ is the total code length. By unique decodability, the concatenations of length $r$ in this [sum](../../../../sum.md) are all distinct, so there are at most $2^r$ of them. Since $n\leq r\leq nl_{\max}$,

$$
S^n\leq\sum_{r=n}^{nl_{\max}}2^r2^{-r}\leq nl_{\max}.
$$

Taking $n$th roots and sending $n$ to infinity proves the [Kraft–McMillan inequality](../../../../kraft-mcmillan-inequality.md)

$$
\boxed{\sum_{k=1}^a2^{-l_k}\leq1.}
$$

Now $q_k=2^{-l_k}/S$ is a [probability distribution](../../../../probability-distribution-split.md). With base-two logarithms, [Gibbs inequality](../../../../gibbs-inequality.md) gives

$$
0\leq D(p\Vert q)=\sum_kp_k\log_2\frac{p_k}{q_k}
=-H(X)+\mathbb EL+\log_2 S.
$$

Terms with $p_k=0$ contribute zero. Therefore

$$
\boxed{\mathbb EL-H(X)=D(p\Vert q)-\log_2S\geq0.}
$$

The normalization by $S$ is important: the raw numbers $2^{-l_k}$ need not [sum](../../../../sum.md) to one.

## ↑ Ancestors (12)

1. [B](../b.md)
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
