<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

[Löb's theorem](../../../../lob-s-theorem.md) states that, for a [first-order theory](../../../../first-order-theory.md) with the stated provability and diagonalization properties,

$$
\boxed{S\vdash(BA\to A)\quad\Longrightarrow\quad S\vdash A,}
$$

where $BA=P_S(\ulcorner A\urcorner)$. It does not require an extra consistency assumption.

By the [diagonal lemma](../../../../diagonal-lemma.md), choose $D$ with $S\vdash D\leftrightarrow(BD\to A)$. [necessitation rule](../../../../necessitation-rule.md) and distribution applied to $D\to(BD\to A)$ give

$$
S\vdash BD\to B(BD\to A),\qquad S\vdash BD\to(B(BD)\to BA).
$$

Using [positive introspection](../../../../positive-introspection.md) $BD\to B(BD)$ gives the unconditional theorem $S\vdash BD\to BA$. If $S\vdash BA\to A$, it follows that $S\vdash BD\to A$, and the reverse fixed-point implication gives $S\vdash D$. Necessitating gives $S\vdash BD$, hence $S\vdash BA$ and finally $S\vdash A$.

The same derivation also gives the [Internal form of Löb's theorem](../../../../internal-form-of-lob-s-theorem.md), needed for modal soundness. Put $H=(BA\to A)$. From the unconditional $BD\to BA$, propositional reasoning and the fixed point give $S\vdash H\to D$. [necessitation rule](../../../../necessitation-rule.md) and distribution imply $S\vdash BH\to BD$, and hence

$$
\boxed{S\vdash B(BA\to A)\to BA.}
$$

This internal statement was derived without necessitating a temporary assumption.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the Gödel's incompleteness theorems course of the University of Oxford](../../../split.md)
5. [Gödel's incompleteness theorems course of the University of Oxford](../../../../godel-s-incompleteness-theorems-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
