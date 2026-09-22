<h1 id="4g/solution">Solution</h1>

↑ **Parent:** [4G](../4g.md)

A binary [linear-feedback shift register](../../../../../linear-feedback-shift-register.md) of length $L$ keeps $L$ bits and produces a sequence satisfying a recurrence

$$
s_n+c_1s_{n-1}+\cdots+c_Ls_{n-L}=0\quad\text{in }\mathbb F_2.
$$

After each output it shifts its stored bits and inserts the feedback bit. Its connection polynomial is $C(z)=1+c_1z+\cdots+c_Lz^L$. This convention reverses the usual [characteristic polynomial](../../../../../characteristic-polynomial.md) $z^L+c_1z^{L-1}+\cdots+c_L$.

The [Berlekamp-Massey algorithm](../../../../../berlekamp-massey-algorithm.md) recovers the shortest recurrence compatible with observed bits. Maintain the current $C$, length $L$, an earlier polynomial $B$ that last caused a length increase, and the offset $m$ since that increase. Initially $C=B=1,L=0,m=1$. At position $n$ calculate the discrepancy $d=s_n+\sum_{j=1}^Lc_js_{n-j}$. If $d=0$, advance $m$. If $d=1$, save $T=C$ and replace $C$ by $C+z^mB$. If also $2L\leq n$, replace $L$ by $n+1-L$, $B$ by $T$ and $m$ by one; otherwise increase $m$. Over a general field the correction is $(d/b)z^mB$, where $b$ is the saved nonzero discrepancy. The correction cancels the failed equation while retaining the previous successful ones; when it forces a length increase the smallest possible new length is $n+1-L$.

Here, indexing the first bit by zero, the nonzero discrepancies occur at positions $1,4,6$. The corresponding updates are

$$
(C,L)=(1+z^2,2),\quad(1+z^2+z^3,3),\quad(1+z^3+z^4,4).
$$

Every subsequent supplied discrepancy is zero. Thus

$$
\boxed{C(z)=1+z^3+z^4,\qquad s_n=s_{n-3}+s_{n-4}.}
$$

Equivalently the characteristic [feedback polynomial](../../../../../feedback-polynomial.md) is $z^4+z+1$. No length-three recurrence works: positions $3,4,5$ force $c_2=1,c_1=0,c_3=1$, but position six then has nonzero discrepancy. The recovered length is therefore minimal. Observing at least twice the true linear complexity ordinarily identifies the recurrence, after which a known consecutive block determines all future key bits. This is why a bare register is unsuitable as a cryptographic keystream generator; a finite prefix alone does not exclude a longer generator that later diverges.

## ↑ Ancestors (10)

1. [4G](../4g.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
