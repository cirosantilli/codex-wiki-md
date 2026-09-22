<h1 id="13f/solution">Solution</h1>

↑ **Parent:** [13F](../13f.md)

The [Fundamental theorem of finitely generated abelian groups](../../../../../fundamental-theorem-of-finitely-generated-abelian-groups.md) states that every such [group](../../../../../group-split.md) is isomorphic to

$$
\mathbb Z^r\oplus\mathbb Z/d_1\mathbb Z\oplus\cdots\oplus\mathbb Z/d_s\mathbb Z,
\qquad 1<d_1\mid d_2\mid\cdots\mid d_s,
$$

with uniquely determined rank and invariant factors, allowing an empty finite part. Modulo $pA$, the free summand contributes $(\mathbb Z/p\mathbb Z)^r$. If $A/pA=0$ for some prime, this forces $r=0$, so $A$ is finite. Conversely, if $A$ is finite, choose a prime $p$ coprime to $|A|$. Bezout's identity gives an integer $b$ with $bp\equiv1\pmod{|A|}$. Since $|A|$ kills every element, multiplication by $p$ is onto, with inverse multiplication by $b$. Hence $pA=A$. This proves **$\boxed{A\text{ finite}\iff A/pA=0\text{ for some prime }p}$** under finite generation.

For the requested nonzero example use the additive [divisible group](../../../../../divisible-group.md) $A=\mathbb Q$. Each rational $q$ equals $p(q/p)$, so $p\mathbb Q=\mathbb Q$ for every prime. It is not finitely generated: a finite list of rational generators has a common denominator $D$, and every integral combination then lies in $D^{-1}\mathbb Z$. The rational $1/(2D)$ does not lie there. This proves non-finite-generation directly and shows why the hypothesis in [finite generation detected by a prime quotient](../../../../../finite-generation-detected-by-a-prime-quotient.md) is essential.

## ↑ Ancestors (10)

1. [13F](../13f.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
