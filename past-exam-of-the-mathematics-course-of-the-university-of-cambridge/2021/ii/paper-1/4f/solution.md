<h1 id="4f/solution">Solution</h1>

↑ **Parent:** [4F](../4f.md)

For the given effective enumeration of partial computable functions, the [diagonal halting set](../../../../../diagonal-halting-set.md) is

$$
\boxed{K=\{n\in\mathbb N:f_{n,1}(n)\text{ is defined}\}}.
$$

A [many-one reduction](../../../../../many-one-reduction.md) $A\leq_mB$ is a [total computable function](../../../../../total-computable-function.md) $g:\mathbb N\to\mathbb N$ such that

$$
\boxed{x\in A\Longleftrightarrow g(x)\in B}.
$$

The [S-m-n theorem](../../../../../smn-theorem.md) states that for every $m,k\geq1$ there is a total computable function $s_k^m$ satisfying

$$
f_{s_k^m(e,x_1,\ldots,x_m),k}(y_1,\ldots,y_k)
=f_{e,m+k}(x_1,\ldots,x_m,y_1,\ldots,y_k)
$$

whenever either side is defined.

Suppose first that $X$ is [recursively enumerable](../../../../../recursively-enumerable-set.md). Choose a program that halts exactly on inputs in $X$, and let $e$ index a two-variable program that, on $(x,y)$, ignores $y$ and runs that program on $x$. By the S-m-n theorem,

$$
g(x)=s_1^1(e,x)
$$

is total computable and indexes the unary function

$$
f_{g(x),1}(y)=f_{e,2}(x,y).
$$

Therefore

$$
x\in X
\Longleftrightarrow f_{g(x),1}(g(x))\text{ is defined}
\Longleftrightarrow g(x)\in K.
$$

Thus $X\leq_mK$.

Conversely, suppose $X\leq_mK$ through a total computable $g$. On input $x$, compute $g(x)$ and simulate machine $g(x)$ on its own code. This procedure halts exactly when $g(x)\in K$, equivalently exactly when $x\in X$. Hence $X$ is recursively enumerable. We have proved the [many-one completeness of the halting problem](../../../../../many-one-completeness-of-the-halting-problem.md):

$$
\boxed{X\text{ is recursively enumerable}\Longleftrightarrow X\leq_mK}.
$$

Finally, use the stated fact that $0\notin K$ and define

$$
S=\{0\}\cup\{2n+1:n\in K\}.
$$

Then $0\in S\setminus K$, so $S\ne K$. The total computable map $n\mapsto2n+1$ satisfies

$$
n\in K\Longleftrightarrow2n+1\in S,
$$

and therefore $K\leq_mS$. This is a [distinct representative of the halting many-one degree](../../../../../distinct-representative-of-the-halting-many-one-degree.md).

## ↑ Ancestors (10)

1. [4F](../4f.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
