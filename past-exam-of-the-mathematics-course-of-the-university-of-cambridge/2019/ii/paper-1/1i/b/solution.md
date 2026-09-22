<h1 id="1i/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

An odd [composite number](../../../../../../composite-number.md) $N$ with $\gcd(b,N)=1$ is a [Fermat pseudoprime](../../../../../../fermat-pseudoprime.md) to base $b$ when

$$
b^{N-1}\equiv1\pmod N.
$$

For $N=35$, the [Chinese remainder theorem for unit groups](../../../../../../chinese-remainder-theorem-for-unit-groups.md) reduces this condition to congruences modulo $5$ and $7$. Modulo $5$, [Fermat's little theorem](../../../../../../fermat-little-theorem.md) gives

$$
b^{34}=b^{2}\pmod5,
$$

so $b^{34}\equiv1\pmod5$ exactly when $b\equiv\pm1\pmod5$. Modulo $7$, the unit group has order $6$, so

$$
b^{34}=b^4\pmod7.
$$

The equation $b^4=1$ in the cyclic group $(\mathbb Z/7\mathbb Z)^\times$ has $\gcd(4,6)=2$ solutions, namely $b\equiv\pm1\pmod7$.

Combining the two independent sign choices by the Chinese remainder theorem gives

$$
\begin{array}{c|c|c}
b\pmod5&b\pmod7&b\pmod{35}\\ \hline
1&1&1\\
1&-1&6\\
-1&1&29\\
-1&-1&34
\end{array}
$$

and hence

$$
\boxed{35\text{ is a Fermat pseudoprime to base }b
\iff b\equiv1,6,29,34\pmod{35}}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1I](../../1i.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
