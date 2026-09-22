<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The structural facts used about a non-Archimedean [local field](../../../../../../local-field.md) are that it is complete for a normalized [discrete valuation](../../../../../../discrete-valuation.md) $v:K^\times\to\mathbb Z$, its [valuation ring](../../../../../../valuation-ring.md) $\mathcal O_K=\{x:v(x)\ge0\}$ is a [discrete valuation ring](../../../../../../discrete-valuation-ring.md), its maximal ideal is $\mathfrak m_K=\pi\mathcal O_K$ for a [uniformizer](../../../../../../uniformizer.md) $\pi$, and its [residue field](../../../../../../residue-field.md) is a finite field $k=\mathbb F_q$. Polynomial operations are continuous for this valuation topology.

A simple-root version of [Hensel lemma](../../../../../../hensel-s-lemma.md) is: if $f\in\mathcal O_K[X]$, $a_1\in\mathcal O_K$, $f(a_1)\in\mathfrak m_K$, and $f'(a_1)\notin\mathfrak m_K$, then there is a unique $a\in\mathcal O_K$ with $f(a)=0$ and $a\equiv a_1\pmod{\mathfrak m_K}$.

Construct $a_n$ with $f(a_n)\in\pi^n\mathcal O_K$. Given $a_n$, put $a_{n+1}=a_n+\pi^nb_n$. Taylor expansion over the valuation ring gives

$$
f(a_n+\pi^nb_n)\equiv f(a_n)+\pi^nb_nf'(a_n)\pmod{\pi^{n+1}}.
$$

The omitted terms contain $\pi^{2n}$, and $2n\ge n+1$ for $n\ge1$. The residue of $f'(a_n)$ remains the nonzero residue of $f'(a_1)$, so choose $b_n$ with

$$
\overline{b_n}=-\overline{f(a_n)/\pi^n}\,\overline{f'(a_n)}^{-1}.
$$

This makes $f(a_{n+1})\in\pi^{n+1}\mathcal O_K$. The congruences $a_{n+1}\equiv a_n\pmod{\pi^n}$ make $(a_n)$ a [Cauchy sequence](../../../../../../cauchy-sequence.md); completeness gives its limit $a\in\mathcal O_K$. Continuity and $v(f(a_n))\ge n$ give $f(a)=0$, and the first congruence gives its specified residue class.

For uniqueness, if $a,b$ are two roots in that class, polynomial division of their difference gives

$$
0=f(a)-f(b)=(a-b)\bigl(f'(b)+(a-b)c\bigr),\qquad c\in\mathcal O_K.
$$

The second factor is a unit, since $f'(b)$ is a unit and $a-b\in\mathfrak m_K$. Thus $a=b$. This proves both existence and uniqueness in the stated [Hensel lemma](../../../../../../hensel-s-lemma.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 29](../../../paper-29-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
