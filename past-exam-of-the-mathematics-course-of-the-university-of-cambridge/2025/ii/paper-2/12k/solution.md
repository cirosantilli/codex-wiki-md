<h1 id="12k/solution">Solution</h1>

↑ **Parent:** [12K](../12k.md)

The [unicity distance](../../../../../unicity-distance.md) is the ciphertext length at which the key is uniquely determined, or equivalently at which [key equivocation](../../../../../key-equivocation.md) vanishes:

$$
U=\min\{n:H(K\mid C^n)=0\}.
$$

For Shannon's idealized calculation, assume a uniformly chosen key independent of an iid plaintext source, deterministic invertible encryption for each key, and uniformly distributed ciphertext over an alphabet $\Sigma$. Since $M^n$ is determined by $(C^n,K)$,

$$
\begin{aligned}
H(K\mid C^n)
&=H(M^n,K\mid C^n)\\
&=H(M^n,K)-H(C^n)\\
&=\log|K|+nH-n\log|\Sigma|.
\end{aligned}
$$

Setting this to zero gives

$$
\boxed{U=\frac{\log|K|}{\log|\Sigma|-H}.}
$$

Equivalently, each ciphertext symbol supplies the source redundancy $\log|\Sigma|-H$ bits toward identifying the key.

For the stated cipher, the original formula uses $k_{i\bmod3}$, so $|K|=2^3=8$, while $|\Sigma|=3$. Split first according to whether $m=0$. This event and its complement each have probability $1/2$, and conditional on $m\ne0$ the probabilities are $(2p,1-2p)$. Hence

$$
H(m)=1+\frac12H(2p,1-2p).
$$

If $U\geq20$, then

$$
\log_2(3)-H(m)\leq\frac3{20},
$$

so, using $\log_2(3)=1.585$,

$$
1+\frac12H(2p,1-2p)\geq1.435.
$$

Therefore

$$
\boxed{H(2p,1-2p)\geq0.87.}
$$

[Binary entropy](../../../../../binary-entropy.md) is symmetric about probability $1/2$ and increases up to that point. Since equality holds at $2p=0.30$, it also holds at $2p=0.70$. Thus

$$
H(2p,1-2p)\geq0.87
\quad\Longleftrightarrow\quad
0.30\leq2p\leq0.70,
$$

and all requested values are

$$
\boxed{0.15\leq p\leq0.35.}
$$

Finally let $p=0$, so the source is uniform on $\{0,2\}$. Use one uniform key bit $k$ and encrypt each symbol by

$$
c_i=\begin{cases}m_i,&k=0,\\2-m_i,&k=1.
\end{cases}
$$

Thus the second key swaps $0$ and $2$. Every ciphertext has two possible plaintexts, a binary string and its complement, with equal source probability. No amount of ciphertext distinguishes the keys: $H(K\mid C^n)=1$ for every $n$. This cipher has infinite unicity distance.

## ↑ Ancestors (10)

1. [12K](../12k.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
