# Concatenation grammar

↑ **Parent:** [Variable-based grammar](variable-based-grammar.md)

For grammars $G=(\Sigma,V,P,S)$ and $G'=(\Sigma,V',P',S')$ with disjoint variable sets, introduce a new variable $S_0$ and set

$$
H=(\Sigma,V\cup V'\cup\{S_0\},
P\cup P'\cup\{S_0\to SS'\},S_0).
$$

If both input grammars are variable based, then $L(H)=L(G)L(G')$.

**Table of contents**

- [Regular concatenation grammar](regular-concatenation-grammar.md)
  - [Failure of the regular concatenation construction for a nonregular grammar](failure-of-the-regular-concatenation-construction-for-a-nonregular-grammar.md)
- [Concatenation grammar need not be regular](concatenation-grammar-need-not-be-regular.md)

## ↑ Ancestors (7)

1. [Variable-based grammar](variable-based-grammar.md)
2. [Formal grammar](formal-grammar.md)
3. [Formal language theory](formal-language-theory.md)
4. [Foundations of mathematics](foundations-of-mathematics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/ii/paper-4/4f/b/i/solution.md)
