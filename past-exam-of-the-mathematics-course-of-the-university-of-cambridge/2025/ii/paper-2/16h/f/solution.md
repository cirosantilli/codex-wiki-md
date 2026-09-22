<h1 id="16h/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

We describe a collection of finite multiplication patterns. For finite sets

$$
E\subseteq\{1,\ldots,n\}^3,
\qquad
D\subseteq\{1,\ldots,n\}^2,
$$

write

$$
P_{E,D}(x_1,\ldots,x_n)=
\bigwedge_{(i,j,k)\in E}x_ix_j=x_k
\ \wedge\!
\bigwedge_{(i,j)\in D}x_i\ne x_j.
$$

Call $(E,D)$ $T$-forbidden if the following theory, in $L$ expanded by unary symbols $f_1,\ldots,f_n$, is inconsistent:

- $T$, together with the assertion that every $f_i$ is an automorphism;
- $\forall z\,f_i(f_j(z))=f_k(z)$ for every $(i,j,k)\in E$;
- $\exists z\,f_i(z)\ne f_j(z)$ for every $(i,j)\in D$.

Let $T^*$ contain the group axioms and, for every $T$-forbidden finite pattern, the sentence

$$
\forall x_1\cdots\forall x_n\,\neg P_{E,D}(x_1,\ldots,x_n).
$$

This is a first-order theory in the language of groups.

Suppose $G$ is $T$-good. Choose $M\models T$ and an embedding $\rho:G\hookrightarrow\operatorname{Aut}(M)$. If a tuple $(g_1,\ldots,g_n)$ in $G$ realized a forbidden pattern, interpreting $f_i$ as $\rho(g_i)$ would give a model of its supposedly inconsistent automorphism theory. Thus no such tuple exists, and $G\models T^*$.

Conversely, suppose $G$ is $T$-bad. By part (e), there is a finite set $X=\{g_1,\ldots,g_n\}\subseteq G$ for which $T_G\cap L_X$ is inconsistent. Let

$$
E=\{(i,j,k):g_ig_j=g_k\},
\qquad
D=\{(i,j):g_i\ne g_j\}.
$$

The associated automorphism theory is precisely $T_G\cap L_X$, up to renaming its function symbols, so $(E,D)$ is $T$-forbidden. But $(g_1,\ldots,g_n)$ realizes $P_{E,D}$ in $G$, and therefore $G$ violates the corresponding forbidding axiom. Hence $G\not\models T^*$.

We have proved

$$
\boxed{G\models T^*\quad\Longleftrightarrow\quad G\text{ is }T\text{-good}.}
$$

## ↑ Ancestors (11)

1. [F](../f.md)
2. [16H](../../16h.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
