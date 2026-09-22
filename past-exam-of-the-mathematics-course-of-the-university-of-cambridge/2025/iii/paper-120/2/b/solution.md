<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [Weak normalization theorem for simply typed lambda calculus](../../../../../../weak-normalization-theorem-for-simply-typed-lambda-calculus.md) says that every term typable in the implicational [simply typed lambda calculus](../../../../../../simply-typed-lambda-calculus.md) has a beta-normal form. Define reducibility by induction on types: a term of atomic type is reducible when it is weakly normalizing, and $M:A\to B$ is reducible when $MN$ is reducible at $B$ for every reducible $N:A$. Induction on types shows that every reducible term is weakly normalizing and that variables are reducible.

The fundamental substitution lemma is proved by induction on a typing derivation: if $\Gamma\vdash M:A$ and each variable in $\Gamma$ is replaced by a reducible term of its declared type, then the resulting term is reducible at $A$. The application case is the definition at arrow type; in the abstraction case, applying the abstraction to any reducible argument makes one beta step to the substituted body, which is reducible by induction. Substituting each free variable by itself makes every well-typed term reducible, hence weakly normalizing.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 120](../../../paper-120-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
