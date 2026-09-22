<h1 id="16g/solution">Solution</h1>

↑ **Parent:** [16G](../16g.md)

The [Knaster–Tarski fixed-point theorem](../../../../../knaster-tarski-fixed-point-theorem.md) states that if $L$ is a [complete lattice](../../../../../complete-lattice.md) and $f:L\to L$ is [order-preserving](../../../../../order-preserving-function.md), then the fixed points of $f$ form a complete lattice; in particular, $f$ has least and greatest fixed points.

Let

$$
P=\{x\in L:f(x)\leq x\},
\qquad a=\bigwedge P.
$$

For every $x\in P$, monotonicity gives $f(a)\leq f(x)\leq x$, so $f(a)\leq a$. Applying $f$ once more shows $f(f(a))\leq f(a)$, hence $f(a)\in P$. Therefore $a\leq f(a)$ by the definition of $a$, and $f(a)=a$. Every fixed point belongs to $P$, so $a$ is the least fixed point. Dually, $\bigvee\{x:x\leq f(x)\}$ is the greatest fixed point. For any family $S$ of fixed points, apply the same argument inside the upper interval above $\bigvee S$ to obtain the least fixed point above every member of $S$; this is their join in the fixed-point set. The dual construction supplies meets, proving the full statement.

To deduce the [Cantor-Schröder-Bernstein theorem](../../../../../cantor-schroder-bernstein-theorem.md), let $i:A\to B$ and $j:B\to A$ be injections. On the complete lattice $\mathcal P(A)$ define

$$
F(X)=A\setminus j(B\setminus i(X)).
$$

This map is order-preserving, so it has a fixed point $X$. The relation

$$
A\setminus X=j(B\setminus i(X))
$$

shows that

$$
h(a)=\begin{cases}
i(a),&a\in X,\\
j^{-1}(a),&a\notin X
\end{cases}
$$

is a bijection: its two pieces map bijectively onto the disjoint sets $i(X)$ and $B\setminus i(X)$. Thus injections both ways imply a bijection.

Let $P$ be the poset of countable subsets of $\mathbb R$. The family of all singletons $\{\{r\}:r\in\mathbb R\}$ has no upper bound in $P$, since any upper bound would contain every real number and would be uncountable. Therefore

$$
\boxed{P\text{ is not complete}.}
$$

Finally, use the [well-ordering theorem](../../../../../well-ordering-theorem.md) to fix a well-order $\prec$ of $\mathbb R$. Every countable $A$ omits some real number; let $m(A)$ be its $\prec$-least omitted element and define

$$
f(A)=A\cup\{m(A)\}.
$$

If $A\subseteq B$, then either $m(A)\in B$, or every point preceding $m(A)$ lies in $A\subseteq B$ and $m(A)=m(B)$. In either case $f(A)\subseteq f(B)$, so $f$ is order-preserving. Yet $m(A)\notin A$, and hence

$$
\boxed{f(A)\ne A\text{ for every }A\in P.}
$$

This does not contradict Knaster–Tarski because $P$ is not a complete lattice.

## ↑ Ancestors (10)

1. [16G](../16g.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
