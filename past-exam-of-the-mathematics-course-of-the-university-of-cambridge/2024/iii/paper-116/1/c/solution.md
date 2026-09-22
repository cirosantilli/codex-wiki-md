<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $F$ be a $\kappa$-complete filter on $\kappa$. Use an $L_{\kappa,\kappa}$ propositional language with a sentence $P_A$ for every $A\subseteq\kappa$. Form a theory containing $P_A$ for $A\in F$, the Boolean identities

$$
P_{\kappa\setminus A}\leftrightarrow\neg P_A,
$$

and, for every $\delta<\kappa$,

$$
P_{\bigcap_{i<\delta}A_i}\leftrightarrow\bigwedge_{i<\delta}P_{A_i}.
$$

Every subtheory of size below $\kappa$ mentions fewer than $\kappa$ required members of $F$. Their intersection is nonempty by $\kappa$-completeness; choosing a point in it and interpreting $P_A$ as membership of that point satisfies the subtheory. The theory is therefore $\kappa$-satisfiable. [Strong compactness](../../../../../../strongly-compact-cardinal.md) supplies a model. Then

$$
U=\{A\subseteq\kappa:P_A\text{ holds in the model}\}
$$

is an ultrafilter, contains $F$, and is $\kappa$-complete by the infinitary intersection axioms.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 116](../../../paper-116-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
