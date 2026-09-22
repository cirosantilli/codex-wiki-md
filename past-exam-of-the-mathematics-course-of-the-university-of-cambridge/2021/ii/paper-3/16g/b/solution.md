<h1 id="16g/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The map $a\mapsto\{a\}$ injects $x$ into $\mathcal P(x)$. Cantor's diagonal argument shows that no map $x\to\mathcal P(x)$ is surjective: for $f:x\to\mathcal P(x)$, the set $D=\{a:a\notin f(a)\}$ differs from every $f(a)$. Hence $\kappa<2^\kappa$.

If $f:x\to y$ is surjective, inverse image gives an injection

$$
\mathcal P(y)\to\mathcal P(x),
\qquad A\mapsto f^{-1}(A).
$$

For every infinite initial ordinal $\omega_\alpha$, transfinite recursion constructs a pairing of $\omega_\alpha\times\omega_\alpha$ with $\omega_\alpha$: at each stage fewer than $\aleph_\alpha$ earlier pairs have been used. Thus

$$
\aleph_\alpha\aleph_\alpha=\aleph_\alpha
$$

without invoking choice for arbitrary families.

Every ordinal below $\omega_{\alpha+1}$ has cardinal at most $\aleph_\alpha$ and can be coded by a well-ordering relation on a subset of $\omega_\alpha$. Sending such a relation to its order type, and all non-well-orders to zero, gives a surjection

$$
\mathcal P(\omega_\alpha\times\omega_\alpha)\to\omega_{\alpha+1}.
$$

Using the pairing above to code relations as subsets of $\omega_\alpha$ yields

$$
\boxed{\aleph_{\alpha+1}\leq2^{\aleph_\alpha}}.
$$

Again, strictness beyond this is independent of the usual axioms.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [16G](../../16g.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
