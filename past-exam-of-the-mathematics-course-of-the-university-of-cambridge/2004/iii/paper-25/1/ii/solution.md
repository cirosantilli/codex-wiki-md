<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Normalize each finite-place [valuation](../../../../../../valuation.md) to have image $\mathbb Z$. For a radical class $[a]$, the residue of $v(a)$ modulo $n$ is well-defined, because replacing $a$ by $ab^n$ adds $nv(b)$. A suitable finite set is

$$
\boxed{S=S_\infty\ \cup\ \{v<\infty:v(n)>0\}
\ \cup\ \{v<\infty:v(a)\not\equiv0\pmod n
\text{ for some }[a]\in\Delta\}.}
$$

One can compute the last union from any finite generating set of $\Delta$. Each representative has only finitely many nonzero [valuations](../../../../../../valuation.md), so this indeed defines a finite set depending only on $n$ and the classes, not on a choice of representatives. Including all infinite places safely allows possible real-to-complex ramification.

Fix $v\notin S$ and work over the completion $K_v$. A representative has $v(a)=nk$, so $a=\pi^{nk}u$ with $u$ a unit. Adjoining an $n$th root of $a$ is the same as adjoining an $n$th root of $u$. Since $n$ is invertible in the [residue field](../../../../../../residue-field.md), $X^n-\bar u$ is separable: its derivative $nX^{n-1}$ has no common zero with it.

Take a finite extension of the finite [residue field](../../../../../../residue-field.md) containing all roots of all these finitely many reduced polynomials. The corresponding finite [unramified extension](../../../../../../unramified-extension.md) of $K_v$ exists by the classification proved in Question 2. [Hensel's lemma](../../../../../../hensel-s-lemma.md) lifts each simple residue root to a root of the original polynomial in that [unramified extension](../../../../../../unramified-extension.md). Thus all the required radicals, and every conjugate root, lie in an unramified local extension. Every completion of the radical field at $v$ is therefore unramified. This proves [finite ramification support for radical extensions](../../../../../../finite-ramification-support-for-radical-extensions.md).

The local argument does not assume $\mu_n\subset K$: adjoining all roots proves the stronger unramified assertion for the [splitting field](../../../../../../splitting-field.md), and hence for any field obtained by choosing the radicals. For $n=1$ the radical extension is trivial; the displayed set is still valid.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 25](../../../paper-25-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
