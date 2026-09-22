<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

First use the fact that a [small set is absent from a complete nonprincipal ultrafilter](../../../../../../small-set-is-absent-from-a-complete-nonprincipal-ultrafilter.md). Indeed, if $A\subseteq\kappa$ and $|A|<\kappa$, then every $\kappa\setminus\{\alpha\}$, $\alpha\in A$, belongs to $U$ by nonprincipality. [Kappa-completeness](../../../../../../kappa-complete-filter.md) gives $\kappa\setminus A\in U$, so $A\notin U$. In particular every final segment $\{i:i>\alpha\}$ belongs to $U$.

Suppose for contradiction that the [ultrapower](../../../../../../ultrapower.md) has at most $\kappa$ elements. List representatives $f_\alpha:\kappa\to M$ for all its classes, indexed by $\alpha<\kappa$; repetitions are allowed. At coordinate $i<\kappa$, fewer than $\kappa$ values occur among $f_\alpha(i)$ with $\alpha<i$. Since $|M|\geq\kappa$, choose

$$
g(i)\in M\setminus\{f_\alpha(i):\alpha<i\}.
$$

This [diagonal argument for ultrapower cardinality](../../../../../../diagonal-argument-for-ultrapower-cardinality.md) uses the [axiom of choice](../../../../../../axiom-of-choice.md). For each fixed $\alpha$, the functions $g$ and $f_\alpha$ disagree throughout the final segment $i>\alpha$, which belongs to $U$. Their equality set therefore cannot belong to $U$, and $[g]\ne[f_\alpha]$.

This contradicts the assumed enumeration of the [ultrapower](../../../../../../ultrapower.md). Hence

$$
\boxed{|M^\kappa/U|>\kappa.}
$$

The proof uses only that each ordinal $i<\kappa$ has [cardinality](../../../../../../cardinality.md) below $\kappa$; it does not require a separate assumption of regularity.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [1](../../1.md)
3. [Paper 23](../../../paper-23-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
