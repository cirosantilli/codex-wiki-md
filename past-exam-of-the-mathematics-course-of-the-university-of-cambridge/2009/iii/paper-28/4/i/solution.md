<h1 id="4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $\pi\in K$ be a [uniformizer](../../../../../../uniformizer.md). Because $L/K$ is [unramified](../../../../../../unramified-extension.md), the same $\pi$ is a [uniformizer](../../../../../../uniformizer.md) of $L$, and $v_L|_K=v_K$. The conjugates of $z\in L^\times$ all have the same [valuation](../../../../../../valuation.md), so

$$
v_K(N_{L/K}z)=n\,v_L(z).
$$

This proves that every [field norm](../../../../../../field-norm.md) has valuation divisible by $n$. Conversely $N_{L/K}(\pi^r)=\pi^{nr}$ for every integer $r$, so it remains to prove [surjectivity of unit norms in unramified extensions](../../../../../../surjectivity-of-unit-norms-in-unramified-extensions.md).

Write $|k_K|=Q$, so $|k_L|=Q^n$. Reduction of the [field norm](../../../../../../field-norm.md) on units is the finite-field norm

$$
k_L^\times\longrightarrow k_K^\times,\qquad a\longmapsto a^{1+Q+\cdots+Q^{n-1}}.
$$

The [multiplicative group of a finite field is cyclic](../../../../../../multiplicative-group-of-a-finite-field-is-cyclic.md). The displayed power map on a group of order $Q^n-1$ has image of order $Q-1$, and is therefore onto $k_K^\times$. Given a unit $u\in\mathcal O_K^\times$, first choose $b_1\in\mathcal O_L^\times$ with $N(b_1)\equiv u\pmod\pi$.

We can correct the norm at each subsequent power of $\pi$. For $r\geq1$ and $a\in\mathcal O_L$, expanding the product over the cyclic [Galois group](../../../../../../galois-group.md) gives

$$
N(1+\pi^r a)\equiv1+\pi^r\operatorname{Tr}_{k_L/k_K}(\bar a)\pmod{\pi^{r+1}}.
$$

All products involving at least two correction terms are divisible by $\pi^{2r}$, hence by $\pi^{r+1}$. The residue [field trace](../../../../../../field-trace.md) is onto even if the residue characteristic divides $n$. Indeed its [polynomial](../../../../../../polynomial-split.md) $T(X)=X+X^Q+\cdots+X^{Q^{n-1}}$ is nonzero of degree $Q^{n-1}<Q^n$; it cannot vanish at every element of $k_L$. Its values lie in $k_K$, since raising $T(a)$ to $Q$ cyclically permutes the summands. Thus it is a nonzero $k_K$-linear map to the one-dimensional space $k_K$, and is surjective.

Suppose $N(b_r)\equiv u\pmod{\pi^r}$. Choose $\bar a_r$ whose trace is the coefficient of $\pi^r$ in $u/N(b_r)-1$, and put $b_{r+1}=b_r(1+\pi^r a_r)$. Then $N(b_{r+1})\equiv u\pmod{\pi^{r+1}}$, and $b_{r+1}\equiv b_r\pmod{\pi^r}$. By [completeness](../../../../../../completeness.md) the units $b_r$ converge to a unit $b$. The [field norm](../../../../../../field-norm.md) is [continuous](../../../../../../continuous-function.md), being a polynomial in coordinates of multiplication, so $N(b)=u$. Multiplying such a unit by a power of $\pi$ proves

$$
\boxed{N_{L/K}(L^\times)=\{x\in K^\times:v_K(x)\equiv0\pmod n\}.}
$$

The proof uses no local class field theory, and works in either characteristic.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [4](../../4.md)
3. [Paper 28](../../../paper-28-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
