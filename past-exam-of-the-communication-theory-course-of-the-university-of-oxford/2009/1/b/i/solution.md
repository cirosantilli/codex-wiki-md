<h1 id="1/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Factoring a joint [probability](../../../../../probability.md) into successive conditional probabilities and taking the expected negative logarithm gives the [chain rule for entropy](../../../../../chain-rule-for-conditional-entropy.md):

$$
H_n=\sum_{r=1}^nH(X_r\mid X_1,\ldots,X_{r-1}).
$$

At $r=1$ this means the unconditional [entropy](../../../../../information-entropy-split.md). Removing conditioning can only increase each term by part (a), so $H_n\leq\sum_rH(X_r)$.

Write $X_{-r}$ for the vector omitting coordinate $r$. Another application of the chain rule gives $H(X_{-r}\mid X_r)=H_n-H(X_r)$. Therefore

$$
\sum_rH(X_{-r}\mid X_r)=nH_n-\sum_rH(X_r)\leq(n-1)H_n.
$$

Divide by $n-1>0$ to obtain the required averaged inequality. The case $n=1$ is excluded precisely because that denominator vanishes.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the communication Theory course of the University of Oxford](../../../../split.md)
6. [Communication Theory course of the University of Oxford](../../../../../communication-theory-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
