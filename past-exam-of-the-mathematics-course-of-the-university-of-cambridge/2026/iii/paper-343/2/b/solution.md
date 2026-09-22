<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Interpret the sum as one term per unordered pair. With

$$
S_\alpha=\frac12\sum_{i=1}^N\sigma_i^\alpha,
$$

the all-to-all XY Hamiltonian is

$$
H=2(S_x^2+S_y^2)-N
=2[S(S+1)-m^2]-N.
$$

For fixed total spin $S$, choose $|m|=S$, giving $E=2S-N$. The smallest allowed total spin is $S=0$ for even $N$ and $S=1/2$ for odd $N$, so

$$
E_0=
\begin{cases}
-N,&N\ \text{even},\\
1-N,&N\ \text{odd}.
\end{cases}
$$

Dividing by $\binom N2$ gives

$$
\boxed{\lim_{N\to\infty}\frac{E_0}{\binom N2}=0^-}.
$$

For three qubits, $E_0=-2$ and there are three pairs:

$$
\boxed{\frac{E_0}{3}=-\frac23<0}.
$$

The finite system therefore has a smaller pair-energy density; monogamy prevents every pair from independently attaining the two-qubit minimum.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 343](../../../paper-343-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
