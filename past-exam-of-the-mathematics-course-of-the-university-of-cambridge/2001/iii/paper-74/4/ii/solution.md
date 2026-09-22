<h1 id="4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Set $L=K_{\mathfrak P}$ and $F=k_{\mathfrak p}$, with valuation rings $S,R$. Let $e$ be the [ramification index](../../../../../../ramification-index.md), $f$ the [residue-field degree](../../../../../../residue-field-degree.md), and $p$ the [residue characteristic](../../../../../../residue-characteristic.md). A base [uniformizer](../../../../../../uniformizer.md) $\pi$ generates $\mathfrak P^e$ in $S$, up to a unit. The free $R$-module $S$ has rank $ef$. For an integral $a\in S$, its [field trace](../../../../../../field-trace.md) is the [matrix trace](../../../../../../matrix-trace.md) of multiplication by $a$ on this module. Reduction modulo $\pi$ preserves the matrix trace.

The quotient $S/\pi S$ has a filtration

$$
S/\mathfrak P^e\supset\mathfrak P/\mathfrak P^e\supset\cdots\supset\mathfrak P^{e-1}/\mathfrak P^e\supset0.
$$

Each of the $e$ successive quotients is a one-dimensional vector space over $\kappa_L=S/\mathfrak P$. On each, multiplication by $a$ acts as multiplication by its residue $\bar a$, whose trace over $\kappa_F=R/\pi R$ is $\operatorname{Tr}_{\kappa_L/\kappa_F}(\bar a)$. A basis adapted to the filtration makes the multiplication matrix block triangular, so its trace is the sum of these quotient traces. This proves [trace reduction in a ramified local extension](../../../../../../trace-reduction-in-a-ramified-local-extension.md):

$$
\overline{\operatorname{Tr}_{L/F}(a)}=e\operatorname{Tr}_{\kappa_L/\kappa_F}(\bar a).
$$

Since the hypothesis says $p\mid e$, the right side is zero in $\kappa_F$. Thus

$$
\boxed{\operatorname{Tr}_{K_{\mathfrak P}/k_{\mathfrak p}}(a)\in\mathfrak p\mathcal O_{k_{\mathfrak p}}.}
$$

No normality hypothesis is needed. The original PDF only requires divisibility of $e$, not divisibility exactly once; the converted TeX has corrupted that condition and several local subscripts.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [4](../../4.md)
3. [Paper 74](../../../paper-74-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
