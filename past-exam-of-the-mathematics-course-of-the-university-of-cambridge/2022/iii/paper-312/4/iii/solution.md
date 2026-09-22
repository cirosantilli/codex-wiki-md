<h1 id="4/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Put $\mathbf p=\mathbf k-\mathbf q$, $p^2=k^2-2kq\mu+q^2$, and $\mu=\widehat{\mathbf k}\mathbin\cdot\widehat{\mathbf q}$. Direct substitution into $F_2$ gives

$$
F_2(\mathbf q,\mathbf p)
=\frac{k^2[7k\mu+q(3-10\mu^2)]}{14q\,p^2}.
$$

Using $d^3q=2\pi q^2dq\,d\mu$ in part ii therefore yields

$$
\boxed{
P_{22}(k)=\int_0^\infty\frac{dq}{4\pi^2}
\int_{-1}^1d\mu\,
\frac{k^4[7k\mu+q(3-10\mu^2)]^2}
{98(k^2-2kq\mu+q^2)^2}
P(q)P\!\left(\sqrt{k^2-2kq\mu+q^2}\right)}.
$$

For $q\ll k$, $F_2(\mathbf q,\mathbf k-\mathbf q)\sim k\mu/(2q)$. Including the equal soft region $|\mathbf k-\mathbf q|\to0$ and using $\int_{-1}^1\mu^2d\mu=2/3$ gives

$$
\boxed{P_{22,{\rm IR}}(k)\longrightarrow
\frac13k^2P(k)\int\frac{dq}{2\pi^2}P(q)}.
$$

For $q\gg k$, the constant and linear hard-momentum terms cancel, displaying the [ultraviolet softness of the second-order density kernel](../../../../../../ultraviolet-softness-of-the-second-order-density-kernel.md). Since $p\sim q$,

$$
F_2\sim\frac{k^2}{14q^2}(3-10\mu^2).
$$

The angular integral $\int_{-1}^1(3-10\mu^2)^2d\mu=18$ then gives

$$
\boxed{P_{22,{\rm UV}}(k)\longrightarrow
\frac9{98}k^4\int\frac{dq}{2\pi^2}\frac{P(q)^2}{q^2}}.
$$

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [4](../../4.md)
3. [Paper 312](../../../paper-312-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
