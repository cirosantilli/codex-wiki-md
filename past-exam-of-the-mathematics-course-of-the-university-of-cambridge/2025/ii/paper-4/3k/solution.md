<h1 id="3k/solution">Solution</h1>

↑ **Parent:** [3K](../3k.md)

A binary [linear-feedback shift register](../../../../../linear-feedback-shift-register.md) of degree $d$ has a state  
$(s_n,\ldots,s_{n+d-1})\in\mathbb F_2^d$ and recurrence

$$
s_{n+d}=a_{d-1}s_{n+d-1}+\cdots+a_0s_n.
$$

Its feedback polynomial is

$$
f(X)=X^d+a_{d-1}X^{d-1}+\cdots+a_0.
$$

There are $2^d$ states, and the zero state is fixed. A nonzero periodic orbit therefore visits at most the other $2^d-1$ states, proving the [period bound for a linear-feedback shift register](../../../../../period-bound-for-a-linear-feedback-shift-register.md).

For a maximal orbit with $d>1$, the all-one state cannot itself be fixed. From that state the incoming bit is $a_0+\cdots+a_{d-1}$ in $\mathbb F_2$. If an odd number of the $a_i$ were one, the incoming bit would be one and the all-one state would be fixed. Hence an even number of the $a_i$ are one; including the leading coefficient, the feedback polynomial has an odd number of nonzero coefficients. This is the [feedback-polynomial parity condition for maximal period](../../../../../feedback-polynomial-parity-condition-for-maximal-period.md).

The given prefix has seven consecutive zeros followed by a one. Any register of degree at most seven would therefore enter the all-zero state before producing the final one, which is impossible. Degree eight is attained by

$$
s_{n+8}=s_n,
$$

with initial state $10000000$. It produces the next bit $1$ and has feedback polynomial

$$
\boxed{f(X)=X^8+1}.
$$

**Thus this is the [minimal linear-feedback shift register for the prefix 100000001](../../../../../minimal-linear-feedback-shift-register-for-the-prefix-100000001.md).**

## ↑ Ancestors (10)

1. [3K](../3k.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
