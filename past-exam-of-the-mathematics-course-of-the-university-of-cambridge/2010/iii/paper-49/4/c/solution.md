<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The eigenvalue on $|0\rangle$ of every power is one, and its eigenvalue on $|1\rangle$ is $e^{2\pi iak/N}$. Thus

$$
R_a^k=R_a^l\quad\Longleftrightarrow\quad e^{2\pi ia(k-l)/N}=1
\quad\Longleftrightarrow\quad N\mid a(k-l).
$$

If $a$ is odd, its [greatest common divisor](../../../../../../greatest-common-divisor.md) with $N=2^n$ is one. Divisibility can therefore be cancelled, giving

$$
\boxed{R_a^k=R_a^l\iff k\equiv l\pmod{2^n}.}
$$

In particular, the $N$ powers with $0\leq k<N$ are distinct. Each is the phase gate $R_m$ with $m\equiv ak\pmod N$, and multiplication by $a$ is a permutation of these residue classes. Equivalently, for any desired $m$, choose $k\equiv a^{-1}m\pmod N$, where $a^{-1}$ is the [modular inverse](../../../../../../modular-multiplicative-inverse.md). Then $R_a^k=R_m$, using the representative $0\leq k<N$ and repeated forward applications only. Thus the powers generate the entire set. Once the preceding identification procedure has found $a$, these powers can also be labelled and selected classically.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 49](../../../paper-49-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
