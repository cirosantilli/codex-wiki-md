<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

[Independence](../../../../independent-random-variables.md) gives $P(X=Y)=\sum_rp_rq_r=\mathbb E_p[2^{\log_2q_X}]$. The given exponential convexity inequality therefore yields

$$
P(X=Y)\ge2^{\sum_rp_r\log_2q_r}=2^{-H(X)-D(p,q)}.
$$

Taking complementary probabilities proves

$$
\boxed{P(X\ne Y)\le1-2^{-H(X)-D(p,q)}}.
$$

The strict positivity of the entries of $q$ makes all logarithms appearing in this finite expectation well defined.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the communication Theory course of the University of Oxford](../../../split.md)
5. [Communication Theory course of the University of Oxford](../../../../communication-theory-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
