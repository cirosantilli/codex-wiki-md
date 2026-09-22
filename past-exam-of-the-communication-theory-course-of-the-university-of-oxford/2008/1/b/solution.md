<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The conditional output distributions are permutations of the same triple, so both [conditional entropies](../../../../conditional-entropy.md) equal

$$
H_0=H(1/6,1/3,1/2).
$$

With input probability $p$, the three output probabilities are $q_1=(2-p)/6$, $q_2=(1+2p)/6$, and $q_3=(3-p)/6$. Therefore

$$
\boxed{I(p)=-\sum_{j=1}^3q_j\log_2q_j-H_0}.
$$

Differentiating, the constant terms cancel because $\sum q_j'=0$:

$$
I'(p)=\frac16\log_2\frac{(2-p)(3-p)}{(1+2p)^2},\qquad
I''(p)=-\frac1{\log_e2}\sum_j\frac{(q_j')^2}{q_j}<0.
$$

Thus there is a unique maximum. Its stationary equation reduces to $3p^2+9p-5=0$, whose root in $[0,1]$ is

$$
\boxed{p_{\max}=\frac{\sqrt{141}-9}{6}}.
$$

The other root is negative; [strict concavity](../../../../strict-concavity.md) proves this is the global maximum.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the communication Theory course of the University of Oxford](../../../split.md)
5. [Communication Theory course of the University of Oxford](../../../../communication-theory-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
