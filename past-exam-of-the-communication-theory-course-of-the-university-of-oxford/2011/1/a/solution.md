<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the [continuous](../../../../continuous-function.md) convention $0\log_2(0/q)=0$. Let $S=\{r:p_r>0\}$. Applying the allowed [logarithm](../../../../logarithm.md) [inequality](../../../../inequality-mathematics.md) to $q_r/p_r$ for $r\in S$ gives

$$
-d(p,q)=\sum_{r\in S}p_r\log_2\frac{q_r}{p_r}
\leq c\sum_{r\in S}(q_r-p_r)=c\left(\sum_{r\in S}q_r-1\right)\leq0.
$$

Hence $d(p,q)\geq0$. [Equality](../../../../equality-mathematics.md) forces $\sum_{r\in S}q_r=1$. Since every $q_r$ is strictly positive, this makes $S$ the entire [alphabet](../../../../alphabet.md). [Equality](../../../../equality-mathematics.md) in every weighted [logarithm](../../../../logarithm.md) [inequality](../../../../inequality-mathematics.md) then forces $q_r/p_r=1$ for every $r$. Conversely $p=q$ makes every summand zero. Thus

$$
\boxed{d(p,q)\geq0,\qquad d(p,q)=0\iff p=q.}
$$

This is [Gibbs inequality](../../../../gibbs-inequality.md) for [relative entropy](../../../../kullback-leibler-divergence.md), with zero [probabilities](../../../../probability.md) in the first argument handled explicitly.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the communication Theory course of the University of Oxford](../../../split.md)
5. [Communication Theory course of the University of Oxford](../../../../communication-theory-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
