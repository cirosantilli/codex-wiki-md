<h1 id="20h/solution">Solution</h1>

↑ **Parent:** [20H](../20h.md)

Write the top row as $(u,v,5-u-v)$. The bottom row is then $(3-u,3-v,u+v-1)$, and nonnegativity becomes

$$
0\le u\le3,\qquad0\le v\le3,\qquad1\le u+v\le5.
$$

The feasible set is a hexagon in this plane. Its six vertices, hence all [basic feasible solutions](../../../../../basic-feasible-solution.md) of this [transportation problem](../../../../../transportation-problem.md), are

$$
\boxed{\begin{gathered}
\begin{pmatrix}0&1&4\\3&2&0\end{pmatrix},\quad
\begin{pmatrix}0&3&2\\3&0&2\end{pmatrix},\quad
\begin{pmatrix}2&3&0\\1&0&4\end{pmatrix},\\
\begin{pmatrix}3&2&0\\0&1&4\end{pmatrix},\quad
\begin{pmatrix}3&0&2\\0&3&2\end{pmatrix},\quad
\begin{pmatrix}1&0&4\\2&3&0\end{pmatrix}.
\end{gathered}}
$$

There are four independent constraints; each displayed support consists of four cells forming a [transportation spanning tree](../../../../../transportation-spanning-tree.md), so each is a nondegenerate basic solution. Conversely, a basic feasible solution is a vertex, so the hexagon enumeration is exhaustive.

For any feasible $x'$, the proposed dual inequalities give

$$
f(x')\ge\sum_{ij}(\lambda_i+\mu_j)x'_{ij}=5(\lambda_1+\lambda_2)+3\mu_1+3\mu_2+4\mu_3.
$$

If equality holds on every cell with $x_{ij}>0$, this last quantity equals $f(x)$. Hence **$f(x)\le f(x')$ for every feasible $x'$**. This is [weak duality](../../../../../weak-duality.md) with [complementary slackness](../../../../../complementary-slackness.md).

The [Northwest corner method](../../../../../northwest-corner-method.md) first allocates three units to $(1,1)$, then two to $(1,2)$, one to $(2,2)$ and four to $(2,3)$:

$$
x^*=\begin{pmatrix}3&2&0\\0&1&4\end{pmatrix},\qquad f(x^*)=3a+12.
$$

Choose $\lambda_1=0$, $\lambda_2=2$, $(\mu_1,\mu_2,\mu_3)=(a,2,-1)$. Equality holds on its four occupied cells. The other inequalities are $-1\le3$ and $a+2\le b$. Thus **$a+2\le b$ implies that $x^*$ minimizes $f$**.

The last printed clause changes from minimization to maximization. To answer that wording, use the [transportation simplex algorithm](../../../../../transportation-simplex-algorithm.md) for maximization, equivalently minimize the negative costs. There are only two possible entering cells at $x^*$:

- Entering $(1,3)$ increases $x_{13}$ and $x_{22}$ by $\theta$, and decreases $x_{12}$ and $x_{23}$ by $\theta$. The maximal feasible step is $\theta=2$, reaching $E=\begin{pmatrix}3&0&2\\0&3&2\end{pmatrix}$ and increasing $f$ by $8$.
- Entering $(2,1)$ increases $x_{21}$ and $x_{12}$, and decreases $x_{11}$ and $x_{22}$. Here $\theta=1$, reaching $C=\begin{pmatrix}2&3&0\\1&0&4\end{pmatrix}$ and changing $f$ by $b-a-2$.

Put $d=b-a$. On the feasible hexagon,

$$
f(u,v)=3b+26-(d+2)u-4v.
$$

If $d\le-2$, this expression is maximized by taking $u=3,v=0$, so $E$ is a global maximizer. If $d>-2$, the feasible vertex $(u,v)=(1,0)$ has objective $2(d+2)$ larger than $E$, so $E$ is not a maximizer. Nor can $C$ ever be one: comparison with $x^*$ requires $d\ge2$, while comparison with the vertex $(0,3)$ requires $d\le-2$. Therefore **one pivot to a maximizer is possible exactly when $a\ge b+2$**, by entering $(1,3)$. Its reduced cost for maximization is $4>0$; the other reduced cost is $d-2\le-4$, so the improving pivot is unambiguous.

If “transportation algorithm” is required to retain the preceding minimization objective, no such step can reach a maximizer: every minimizing step is nonincreasing, whereas the feasible point $E$ always has $f(E)=f(x^*)+8$. If the final word was intended to be “minimizes”, the corresponding genuinely improving one-pivot condition would instead be $a-2\le b<a+2$; at $b=a+2$, $x^*$ is already optimal and a zero-cost pivot is possible. These distinctions preserve the printed maximization request without silently altering it.

## ↑ Ancestors (10)

1. [20H](../20h.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
