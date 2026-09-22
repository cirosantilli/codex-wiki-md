<h1 id="m/m1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The preceding marginal calculation makes each $V_i$ [uniformly distributed](../../../../../continuous-uniform-distribution.md) on $(0,1)$, with [expectation](../../../../../expected-value-split.md) $1/2$ and [variance](../../../../../variance-split.md) $1/12$. By [independence](../../../../../independent-random-variables.md),

$$
\mathbb E(S_n/n)=\frac12,\qquad
\operatorname{Var}(S_n/n)=\frac1{12n}.
$$

Apply part (a) to the centred [random variable](../../../../../random-variable-split.md) $Z=S_n/n-1/2$ to obtain

$$
\boxed{\mathbb P\left(\left|S_n/n-1/2\right|\geq a\right)\leq\frac1{12na^2}}.
$$

This is [Chebyshev's inequality](../../../../../chebyshev-s-inequality.md) in this setting.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [M1](../../m1.md)
3. [M](../../../m.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the options I course of the University of Oxford](../../../../split.md)
6. [Options I course of the University of Oxford](../../../../../options-i-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
