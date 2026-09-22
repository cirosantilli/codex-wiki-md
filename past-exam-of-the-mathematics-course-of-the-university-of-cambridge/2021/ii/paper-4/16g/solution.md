<h1 id="16g/solution">Solution</h1>

↑ **Parent:** [16G](../16g.md)

[Axiom of foundation](../../../../../axiom-of-regularity.md) says every nonempty set $A$ contains $a$ with $a\cap A=\emptyset$. Define $T_0=x$, $T_{n+1}=\bigcup T_n$, and $\operatorname{TC}(x)=\bigcup_{n<ω}T_n$ (including $x$ if that convention is desired). Replacement and union form this set, and it is transitive; induction shows every transitive set containing $x$ contains it.

The principle of membership induction says that if $(\forall y\in x\ P(y))\Rightarrow P(x)$ for every $x$, then $P$ holds for every set. Otherwise Foundation applied to the set of counterexamples in a suitable transitive closure gives a minimal counterexample.

Apply induction to $P(x):F(x)=x$. If it holds for all $y\in x$, then extensionality and preservation plus surjectivity give $z\in F(x)$ iff $z=F(y)$ for some $y\in x$, iff $z\in x$. Hence $F(x)=x$.

## ↑ Ancestors (10)

1. [16G](../16g.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
