<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

One useful form of [Hensel lemma](../../../../../../hensel-s-lemma.md) is this: if $R$ is a complete [discrete valuation ring](../../../../../../discrete-valuation-ring.md), $f\in R[X]$, and

$$
f(a_1)\equiv0\pmod\pi,
\qquad
f'(a_1)\not\equiv0\pmod\pi,
$$

then there is a unique $a\in R$ such that $f(a)=0$ and $a\equiv a_1\pmod\pi$. Indeed, after constructing $a_r$ with $f(a_r)\equiv0\pmod{\pi^r}$, choose the unique $t$ modulo $\pi$ for which

$$
f(a_r)+\pi^rtf'(a_r)\equiv0\pmod{\pi^{r+1}}
$$

and put $a_{r+1}=a_r+\pi^rt$. The resulting [Cauchy sequence](../../../../../../cauchy-sequence.md) converges by completeness, and the same first-order congruence proves uniqueness.

Apply this to $X^{p-1}-1$. Every nonzero class in $\mathbb F_p$ is a simple root, so it has a unique [Teichmuller representative](../../../../../../teichmuller-representative.md) in $\mathbb Z_p$. These give all roots of unity of order prime to $p$. For odd $p$, the group $1+p\mathbb Z_p$ has no nontrivial torsion: if $u\ne1$, then the binomial theorem gives $v_p(u^p-1)=v_p(u-1)+1$, which is incompatible with finite $p$-power order. Hence

$$
\mu(\mathbb Q_p)\cong C_{p-1}qquad(p\text{ odd}).
$$

For $p=2$, the subgroup $1+4\mathbb Z_2$ is torsion-free by the same argument, while $-1$ supplies the extra torsion element. Thus $\mu(\mathbb Q_2)=\{\pm1\}\cong C_2$. This describes the [roots of unity in a p-adic field](../../../../../../roots-of-unity-in-a-p-adic-field.md) for $K=\mathbb Q_p$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 136](../../../paper-136-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
