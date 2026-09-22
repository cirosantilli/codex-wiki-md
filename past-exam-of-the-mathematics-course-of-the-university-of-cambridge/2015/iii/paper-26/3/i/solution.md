<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

**The [valuation ring](../../../../../../valuation-ring.md) and local compactness.** The opening, unlettered requests use

$$
\boxed{\mathcal O_K=\{x:|x|\leq1\},\quad
\mathfrak m=\{x:|x|<1\},\quad k=\mathcal O_K/\mathfrak m.}
$$

The ultrametric inequality makes $\mathcal O_K$ a [valuation ring](../../../../../../valuation-ring.md); its elements outside $\mathfrak m$ are exactly the units, so $\mathfrak m$ is its unique [maximal ideal](../../../../../../maximal-ideal.md), and $k$ is the [residue field](../../../../../../residue-field.md).

Here the customary nontrivial-[valuation](../../../../../../valuation.md) hypothesis for a [local field](../../../../../../local-field.md) is necessary. With the trivial absolute value, any infinite field is discrete and locally compact, but its [residue field](../../../../../../residue-field.md) is infinite and there is no nonzero [uniformizer](../../../../../../uniformizer.md). We use the nontrivial [valuation](../../../../../../valuation.md) in the conclusions below.

Local compactness first gives a compact neighborhood of zero. Choose a sufficiently small nonzero $t$ so that the closed set $t\mathcal O_K$ is contained in that compact neighborhood. Then $t\mathcal O_K$, and hence $\mathcal O_K$, is compact. Since $\mathfrak m$ is open, its cosets give a discrete compact quotient $k$, which must be finite. Write $|k|=q$. The subgroup $\mathfrak m$ now has finite index and is closed in $\mathcal O_K$, hence compact. The continuous function $|\cdot|$ attains on $\mathfrak m$ a maximum $c$ with $0<c<1$. Choose $\pi$ with $|\pi|=c$. Every $x\in\mathfrak m$ has $|x/\pi|\leq1$, so

$$
\boxed{\mathfrak m=\pi\mathcal O_K,\qquad |k|=q<\infty.}
$$

Successive division by $\pi$ shows that every nonzero element of $\mathcal O_K$ is a unit times a power of $\pi$: division must terminate because $|\pi|^j\to0$. Thus the value group is discrete. A Cauchy sequence eventually lies in a translate of the compact ring $\mathcal O_K$, has a convergent subsequence, and consequently converges itself. These arguments prove the [discrete valuation from nontrivial local compactness](../../../../../../discrete-valuation-from-nontrivial-local-compactness.md) and the [completeness of locally compact nontrivially valued fields](../../../../../../completeness-of-locally-compact-nontrivially-valued-fields.md).

**The iterated-power limit.** Normalize the [discrete valuation](../../../../../../discrete-valuation.md) by $v(\pi)=1$, and write $q=\ell^f$, where $\ell$ is the [residue characteristic](../../../../../../residue-characteristic.md). For $u\in1+\pi^s\mathcal O_K$ with $s\geq1$, the binomial theorem gives

$$
v(u^q-1)\geq s+1.
$$

The linear term gains a factor $q\in\mathfrak m$ (or is zero in positive characteristic), while all terms of degree at least two have [valuation](../../../../../../valuation.md) at least $2s\geq s+1$.

For $a\in\mathcal O_K^\times$, reduction gives $a^{q-1}\in1+\mathfrak m$, because $k^\times$ has order $q-1$. Iterating the inequality yields

$$
v\bigl(a^{(q-1)q^j}-1\bigr)\geq j+1,\qquad
v\bigl(a^{q^{j+1}}-a^{q^j}\bigr)\geq j+1.
$$

The sequence is Cauchy and converges to a unit $\omega(a)$. Since the reduction of $a^{q^j}$ is always $\bar a$, its limit has the same residue. Taking limits after shifting the sequence gives $\omega(a)^q=\omega(a)$, whence

$$
\boxed{a^{q^j}\longrightarrow\omega(a),\qquad
\omega(a)^{q-1}=1,\qquad\omega(a)\equiv a\pmod\pi.}
$$

This is the [Teichmuller representative](../../../../../../teichmuller-representative.md). The [Hensel lemma](../../../../../../hensel-s-lemma.md) applied to $T^{q-1}-1$, whose derivative is a unit at every nonzero residue, shows uniqueness for each residue. Consequently the prime-to-$\ell$ roots give a canonical splitting

$$
\mathcal O_K^\times=\mu_{q-1}\times(1+\mathfrak m).
$$

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 26](../../../paper-26-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
