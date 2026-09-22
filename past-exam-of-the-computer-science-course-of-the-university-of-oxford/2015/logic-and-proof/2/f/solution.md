<h1 id="2/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

Use the [back-and-forth method](../../../../../back-and-forth-method.md). Enumerate the two domains without repetitions as $a_0,a_1,\ldots$ and $b_0,b_1,\ldots$. We construct a sequence of finite maps, each a [partial isomorphism of structures](../../../../../partial-embedding.md),

$$
f_0\subseteq f_1\subseteq f_2\subseteq\cdots,
$$

starting with the empty [function](../../../../../function-split.md). Each $f_s$ is a [bijection](../../../../../bijection.md) between finite subsets of the domains and preserves both adjacency and nonadjacency on its domain.

At a **forth** step, choose the first $a_i$ outside the current domain. List the finitely many domain [vertices](../../../../../vertex-graph-theory.md) as $u_1,\ldots,u_r$. In $\mathcal B$, prescribe that the new image $b$ be adjacent to $f_s(u_j)$ exactly when $a_i$ is adjacent to $u_j$ in $\mathcal A$. Since the image [vertices](../../../../../vertex-graph-theory.md) are distinct, an extension axiom in $\mathcal B$ supplies such a $b$ outside the entire current range. Extend $f_s$ by $a_i\mapsto b$. This preserves injectivity, adjacency and nonadjacency, including the absence of loops.

At a **back** step, choose the first $b_i$ outside the current range. Apply the same argument to the inverse [partial isomorphism of structures](../../../../../partial-embedding.md) in $\mathcal A$, finding a fresh preimage with the required adjacency pattern to the current domain. Extend $f_s$ by this new pair. Alternate forth and back steps indefinitely.

Define

$$
\boxed{f=\bigcup_{s\ge0}f_s.}
$$

Because each finite [function](../../../../../function-split.md) extends the preceding one, this is a well-defined injective [function](../../../../../function-split.md). The forth steps eventually include every $a_i$ in its domain, and the back steps eventually include every $b_i$ in its range, so $f$ is a [bijection](../../../../../bijection.md). Given any $u,v$, both lie in the domain of some finite $f_s$, where the edge equivalence already holds. It therefore also holds for $f$:

$$
\boxed{(u,v)\in E_{\mathcal A}\quad\Longleftrightarrow\quad
(f(u),f(v))\in E_{\mathcal B}.}
$$

Thus the two [first-order structures](../../../../../first-order-structure.md) are isomorphic. Alternating the steps is essential for surjectivity: repeatedly extending only the domain would merely construct an embedding into $\mathcal B$.

## ↑ Ancestors (11)

1. [F](../f.md)
2. [2](../../2.md)
3. [Logic and proof](../../../logic-and-proof-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
