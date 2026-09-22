<h1 id="4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The intended construction is to solve the [Lenard-Magri recursion](../../../../../../lenard-magri-recursion.md) one step at a time. With $H_0$ a [Casimir function](../../../../../../casimir-function-of-a-poisson-manifold.md) of the first [Poisson structure](../../../../../../poisson-structure.md), seek $H_n$ satisfying

$$
\boxed{X^{(1)}_{H_n}=-X^{(2)}_{H_{n-1}},\quad\text{equivalently}\quad
\Pi_1dH_n=-\Pi_2dH_{n-1}.}
$$

Here $X_H^{(a)}f=\{f,H\}_a$, consistently with part 1(i). If every step can be solved by a globally defined [smooth function](../../../../../../smooth-function.md), the formal series $\sum_{n\geq0}H_n\lambda^n$ is a [Casimir function](../../../../../../casimir-function-of-a-poisson-manifold.md) for the [Poisson pencil](../../../../../../poisson-pencil.md), and part (i) proves that all the $H_n$ are [Poisson-commuting functions](../../../../../../poisson-commuting-functions.md) for every parameter value after complexification.

The recursive step is a concrete potential problem. Put $Y=-X^{(2)}_{H_{n-1}}$. It must first be tangent to the [symplectic leaves](../../../../../../symplectic-leaf.md) of $\Pi_1$. On a regular leaf use [canonical coordinates](../../../../../../canonical-variables.md) $(q_i,p_i)$. The required equations are

$$
\frac{\partial H_n}{\partial p_i}=Y^{q_i},\qquad
\frac{\partial H_n}{\partial q_i}=-Y^{p_i}.
$$

Thus the leaf one-form

$$
\alpha_Y=\sum_i\left(-Y^{p_i}\,dq_i+Y^{q_i}\,dp_i\right)
$$

must be exact. Where it is closed on a contractible coordinate domain, define $H_n$ by integrating $\alpha_Y$ from a base point; path independence follows from closedness. A [function](../../../../../../function-split.md) of the leaf labels can be added, corresponding to a [Casimir function](../../../../../../casimir-function-of-a-poisson-manifold.md) of the first [Poisson structure](../../../../../../poisson-structure.md). Global solvability also requires vanishing periods and smooth matching between leaves. This describes how to perform each solvable step without pretending that a degenerate [Poisson structure](../../../../../../poisson-structure.md) can simply be inverted.

Compatibility alone does not ensure these solvability conditions. There is an immediate [obstruction to a Lenard-Magri recursion](../../../../../../obstruction-to-a-lenard-magri-recursion.md) even in two dimensions. On $M=\mathbb R^2$ take

$$
\{f,g\}_1=0,\qquad
\{f,g\}_2=f_xg_y-f_yg_x,\qquad H_0=x.
$$

Both are [Poisson structures](../../../../../../poisson-structure.md), and their linear combination is a scalar multiple of the canonical [Poisson bracket](../../../../../../poisson-bracket.md), so they are compatible. Every [function](../../../../../../function-split.md), including $H_0$, is a [Casimir function](../../../../../../casimir-function-of-a-poisson-manifold.md) for the first bracket. But the first recursion, evaluated at $f=y$, would require

$$
0=\{H_1,y\}_1=-\{x,y\}_2=-1,
$$

a contradiction. **An arbitrary initial Casimir need not extend even to $H_1$.** Consequently the unconditional existence assertion requires an additional hypothesis: the indicated [vector field](../../../../../../vector-field.md) must be [Hamiltonian](../../../../../../hamiltonian.md) for $\Pi_1$ at every step. Under that hypothesis the recursive construction and involution proof above complete the intended result; without it the counterexample rules out the requested infinite extension.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [4](../../4.md)
3. [Paper 8](../../../paper-8-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
