# Indexed beta reduction

↑ **Parent:** [Indexed lambda term](indexed-lambda-term.md)

Use the binary finite-set encoding $e_k$ and Cantor code $\langle k,t\rangle$. Contracting $(\lambda x.P^n)^{m+1}Q^p$ gives the substituted body with its root index lowered by taking the minimum with $\min(m,n)$, replacing each occurrence $x^r$ by a copy of $Q$ with root index $\min(m,p,r)$. A zero-indexed abstraction instead substitutes $\bot$ and gives the body root index zero. Indices strictly budget the argument information that can be used by application. Finite-witness inequalities for the pairing code prove that indexed reduction increases the interpretation, although it can decrease the underlying [Böhm tree](bohm-tree.md).

## ↑ Ancestors (10)

1. [Indexed lambda term](indexed-lambda-term.md)
2. [Graph model of lambda calculus](graph-model-of-lambda-calculus.md)
3. [Reflexive domain](reflexive-domain.md)
4. [Lambda model](lambda-model.md)
5. [Lambda calculus](lambda-calculus.md)
6. [Computability theory](computability-theory.md)
7. [Foundations of mathematics](foundations-of-mathematics-split.md)
8. [Area of mathematics](area-of-mathematics.md)
9. [Mathematics](mathematics-split.md)
10. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-76/8/solution.md)
