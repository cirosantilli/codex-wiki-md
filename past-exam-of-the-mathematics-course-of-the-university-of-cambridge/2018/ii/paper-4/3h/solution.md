<h1 id="3h/solution">Solution</h1>

↑ **Parent:** [3H](../3h.md)

A binary [linear-feedback shift register](../../../../../linear-feedback-shift-register.md) of length $L$ stores $L$ bits. At each clock it outputs one bit, shifts the state, and inserts a fixed [linear combination](../../../../../linear-combination.md) over $\mathbb F_2$ of the stored bits. Equivalently, its output obeys a recurrence

$$
s_n=c_1s_{n-1}+\cdots+c_Ls_{n-L}.
$$

The [Berlekamp-Massey algorithm](../../../../../berlekamp-massey-algorithm.md) processes the observed symbols from left to right. It maintains the shortest current connection polynomial $C(D)$, its degree $L$, and a saved polynomial from the most recent degree increase. At step $n$ it computes the discrepancy

$$
d_n=s_n+\sum_{i=1}^{L}c_i s_{n-i}.
$$

If $d_n=0$, the current recurrence already predicts the new symbol. If $d_n\ne0$, a shifted multiple of the saved polynomial is added to $C$ to cancel the discrepancy; when $2L\leq n$, the algorithm also replaces $L$ by $n+1-L$ and saves the old polynomial.

For the observed binary sequence, the nonzero-discrepancy updates are

$$
\begin{array}{c|c|c}
n&L&C(D)\\ \hline
1&2&1+D^2\\
4&3&1+D^2+D^3\\
6&4&1+D^3+D^4.
\end{array}
$$

All discrepancies through $n=11$ then vanish. Thus the shortest recurrence is

$$
\boxed{s_n=s_{n-3}+s_{n-4}\pmod2,}
$$

or, equivalently, $s_{n+4}=s_{n+1}+s_n$. The connection polynomial is $1+D^3+D^4$, and with the reciprocal convention the [feedback polynomial](../../../../../feedback-polynomial.md) is

$$
\boxed{x^4+x+1.}
$$

## ↑ Ancestors (10)

1. [3H](../3h.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
