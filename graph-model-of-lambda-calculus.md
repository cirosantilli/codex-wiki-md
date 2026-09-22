# Graph model of lambda calculus

↑ **Parent:** [Reflexive domain](reflexive-domain.md)

Let $P\omega=\mathcal P(\mathbb N)$ ordered by [subset](subset.md). Encode a finite subset $u$ and output $n$ by a natural number $\langle u,n\rangle$. Define $a\cdot b=\{n:\exists u\subseteq b\text{ finite},\ \langle u,n\rangle\in a\}$ and $e(f)=\{\langle u,n\rangle:n\in f(u)\}$. Every [Scott continuous map](scott-continuous-map.md) satisfies $f(b)=\bigcup_{u\subseteq b\text{ finite}}f(u)$, proving that application is the projection of a retraction. [Lambda abstraction](lambda-abstraction.md) has graph $\{\langle u,n\rangle:n\in\llbracket M\rrbracket_{\rho[x:=u]}\}$.

**Table of contents**

- [Approximation theorem for the graph model](approximation-theorem-for-the-graph-model.md)
- [Indexed lambda term](indexed-lambda-term.md)
  - [Indexed beta reduction](indexed-beta-reduction.md)

## ↑ Ancestors (8)

1. [Reflexive domain](reflexive-domain.md)
2. [Lambda model](lambda-model.md)
3. [Lambda calculus](lambda-calculus.md)
4. [Computability theory](computability-theory.md)
5. [Foundations of mathematics](foundations-of-mathematics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Approximation theorem for the graph model](approximation-theorem-for-the-graph-model.md)
- [Finite Böhm approximant](finite-bohm-approximant.md)
- [Indexed lambda term](indexed-lambda-term.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-76/7/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-76/8/solution.md)
