<h1 id="16g/solution">Solution</h1>

↑ **Parent:** [16G](../16g.md)

A deduction from premises $\Gamma$ in [propositional logic](../../../../../propositional-logic.md) is a finite sequence of formulas, each an allowed logical axiom instance, a member of $\Gamma$, or obtained from earlier formulas by an inference rule, such as modus ponens. For example a Hilbert system can use the schemas $p\to(q\to p)$, $[p\to(q\to r)]\to[(p\to q)\to(p\to r)]$, and $(\neg q\to\neg p)\to(p\to q)$, with modus ponens as its rule. Its last formula is the conclusion. A finite deduction uses only finitely many premises. The [completeness theorem for propositional logic](../../../../../completeness-theorem-for-propositional-logic.md) says $\Gamma\models v$ implies $\Gamma\vdash v$; together with soundness, syntactic consistency is equivalent to existence of a satisfying [valuation](../../../../../valuation.md).

For [compactness](../../../../../compact-space.md), if $\Gamma$ had no model, completeness would give a deduction of a contradiction. That deduction uses a finite subset of $\Gamma$, which therefore also has no model. Contrapositively, **if every finite subset has a model, so does $\Gamma$**.

Fix the given [valuation](../../../../../valuation.md) on $Q$ and let $L_v$ be its collection of true literals. Suppose $\{s\}\cup L_v$ were inconsistent. A finite subset of its literals, with conjunction $\ell\in L(Q)$, would satisfy $s\vdash\neg\ell$ by the deduction theorem and classical logic. But $\neg\ell\in U$ whereas the given [valuation](../../../../../valuation.md) makes $\ell$ true, contradicting that it satisfies all of $U$. Hence **$\{s\}\cup L_v$ is consistent**.

If $U\cup\{\neg t\}$ had a model, restrict that [valuation](../../../../../valuation.md) to $Q$ and apply the preceding consistency result. Completeness supplies an extension to $P\cup Q$ making $s$ true and preserving those $Q$ values. Combine its $P$ values with the original model's $Q\cup R$ values. Disjointness of $P,Q,R$ makes this a well-defined [valuation](../../../../../valuation.md) satisfying $s$ and $\neg t$, contradicting soundness of $s\vdash t$. Thus $U\cup\{\neg t\}$ is inconsistent.

[Compactness](../../../../../compact-space.md) now supplies $u_1,\ldots,u_k\in U$ with $u_1,\ldots,u_k\vdash t$. Put $u=\bigwedge_j u_j$. Then

$$
\boxed{s\vdash u,\qquad u\vdash t,\qquad u\in L(Q).}
$$

This proves [propositional interpolation](../../../../../propositional-interpolation.md). The empty conjunction is the truth constant; if the language omits truth and falsehood symbols, use an equivalent tautology when $Q$ is nonempty, or adjoin those constants for the empty-common-language case.

## ↑ Ancestors (10)

1. [16G](../16g.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
