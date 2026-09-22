<h1 id="2/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

A **[reflexive Banach space](../../../../reflexive-banach-space.md)** is one for which $J_X:X\to X^{**}$ is onto. If $X$ is reflexive, every $\theta\in X^{**}$ has the form $\theta(f)=f(x)$ for some $x\in X$. Thus the functionals defining $\sigma(X^*,X^{**})$ and $\sigma(X^*,X)$ are precisely the same, proving equality of the topologies.

Conversely, assume those topologies coincide. For any $\theta\in X^{**}$, the [linear functional](../../../../linear-functional.md) $f\mapsto\theta(f)$ on $X^*$ is then weak-star continuous. Its [continuity](../../../../continuous-function.md) at zero gives finitely many $x_1,\ldots,x_m\in X$ and $\epsilon>0$ such that

$$
|f(x_j)|<\epsilon\ \text{for all }j\quad\Longrightarrow\quad|\theta(f)|<1.
$$

If all these evaluations are zero, arbitrary [scalar](../../../../scalar.md) multiples of $f$ still satisfy the inequalities, forcing $\theta(f)=0$. Hence $\theta$ factors through the finite-dimensional evaluation map $f\mapsto(f(x_1),\ldots,f(x_m))$. A [linear functional](../../../../linear-functional.md) on its image extends to $\mathbb R^m$, so for suitable [scalars](../../../../scalar.md) $a_j$,

$$
\theta(f)=\sum_{j=1}^ma_jf(x_j)=f\left(\sum_{j=1}^ma_jx_j\right).
$$

Thus $\theta$ lies in $J_X(X)$. Since it was arbitrary, $X$ is reflexive. We have proved

$$
\boxed{X\text{ reflexive}\quad\Longleftrightarrow\quad\sigma(X^*,X)=\sigma(X^*,X^{**}).}
$$

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [2](../../2.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the functional analysis course of the University of Oxford](../../../split.md)
5. [Functional analysis course of the University of Oxford](../../../../functional-analysis-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
