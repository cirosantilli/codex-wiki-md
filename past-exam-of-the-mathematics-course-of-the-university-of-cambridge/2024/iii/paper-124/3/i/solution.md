<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $V(x,w)$ be a polynomial-time verifier for $f\in\mathbf{NP}$, with witnesses of length $p(|x|)$. Consider the prefix language

$$
B=\{(x,u):\text{there exists }v\text{ such that }V(x,uv)=1\}.
$$

This language lies in NP, so the assumption $\mathbf{NP}\subseteq\mathbf P/\mathrm{poly}$ supplies a [polynomial-size circuit family](../../../../../../polynomial-size-circuit-family.md) deciding $B$.

Apply the usual [search-to-decision reduction](../../../../../../search-to-decision-reduction.md). Starting with the empty prefix, append zero if the circuit says that some accepting witness has that extended prefix; otherwise append one. Repeat for $p(n)$ positions. Composing the polynomially many copies of the decision circuit produces a polynomial-size circuit $C_n$. Whenever $f(x)=1$, at least one accepting extension exists at every step, so the final string $C_n(x)$ satisfies

$$
\boxed{V(x,C_n(x))=1.}
$$

On negative inputs the output may be arbitrary, as required.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 124](../../../paper-124-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
