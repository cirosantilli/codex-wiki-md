<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The [EPR criterion of reality](../../../../../epr-criterion-of-reality.md) says that if a physical quantity can be predicted with certainty without disturbing the system, then it represents an element of physical reality. For separated particles, the EPR locality assumption regards choices of measurements on the other particles as nondisturbing. The perfect correlations below therefore imply predetermined local values for both $X=\sigma_x$ and $Y=\sigma_y$, independent of which distant measurements are chosen.

Put $|0\rangle=|\uparrow\rangle$ and $|1\rangle=|\downarrow\rangle$. The [Pauli matrices](../../../../../pauli-matrices.md) satisfy

$$
X|0\rangle=|1\rangle,\quad X|1\rangle=|0\rangle,\quad Y|0\rangle=i|1\rangle,\quad Y|1\rangle=-i|0\rangle.
$$

For three particles, each operator with one $X$ and two $Y$ takes $|000\rangle$ to $-|111\rangle$ and $|111\rangle$ to $-|000\rangle$, whereas $X\otimes X\otimes X$ interchanges the two strings without a minus sign. Thus the [GHZ state](../../../../../greenberger-horne-zeilinger-state.md) in the question has the certain outcomes

$$
\boxed{XYY=YXY=YYX=+1,\qquad XXX=-1.}
$$

Each local $X$ or $Y$ value can be predicted from measurements at the other two sites in one of these contexts. If the [EPR criterion of reality](../../../../../epr-criterion-of-reality.md) and locality assign values $x_j,y_j\in\{\pm1\}$, the first three equalities require

$$
x_1y_2y_3=1,\qquad y_1x_2y_3=1,\qquad y_1y_2x_3=1.
$$

Multiplying these ordinary numbers and using $y_j^2=1$ yields $x_1x_2x_3=1$, contradicting the certain quantum outcome $-1$. This derives the [GHZ theorem](../../../../../ghz-theorem.md) explicitly; the multiplication is of hypothetical local values, not of mutually incompatible local observables.

For general $N$, let $O_j=X_j\bigotimes_{k\ne j}Y_k$, with the tensor factors ordered by their site labels, and let $X_N=X^{\otimes N}$. Directly,

$$
O_j|0\rangle^{\otimes N}=i^{N-1}|1\rangle^{\otimes N},\qquad O_j|1\rangle^{\otimes N}=(-i)^{N-1}|0\rangle^{\otimes N}.
$$

For the difference of the two strings to be an [eigenstate](../../../../../eigenstate.md), these phases must agree, which happens exactly when $N-1$ is even. For odd $N$ the common phase is $(-1)^{(N-1)/2}$, and interchanging the strings negates their difference. Consequently

$$
\boxed{N\text{ odd}:\quad O_j|\psi\rangle_N=(-1)^{(N+1)/2}|\psi\rangle_N\ \text{for every }j,\qquad X_N|\psi\rangle_N=-|\psi\rangle_N.}
$$

For even $N$, $X_N$ still has [eigenvalue](../../../../../eigenvalue.md) $-1$, but every $O_j$ takes the difference state to a phase times the sum state, which is [orthogonal](../../../../../orthogonal-vectors.md) to it. Thus it is not an [eigenstate](../../../../../eigenstate.md) of any $O_j$; those operators each have outcomes $\pm1$ with equal [probabilities](../../../../../probability.md). Among the stated $N\geq4$, simultaneous eigenstates therefore occur precisely at $N=5,7,9,\ldots$.

For odd $N$, certainty of each $O_j$ again permits remote prediction of both local $X$ and $Y$. Writing $\lambda_N=(-1)^{(N+1)/2}$, the [local hidden-variable theory](../../../../../local-hidden-variable-theory.md) would require $x_j\prod_{k\ne j}y_k=\lambda_N$ for all $j$. Their product is

$$
\left(\prod_jx_j\right)\prod_k y_k^{N-1}=\lambda_N^N,
$$

hence $\prod_jx_j=\lambda_N$, since $N-1$ is even and $N$ is odd. Quantum theory requires the same product to be $-1$. The contradiction occurs when $\lambda_N=+1$, giving the infinite family

$$
\boxed{N\equiv3\pmod4;\quad N\geq4\text{ gives }N=7,11,15,\ldots.}
$$

For $N\equiv1\pmod4$, these particular certain product constraints are consistent; for example $x_j=-1$, $y_j=+1$ satisfies them. This distinguishes the [GHZ contradiction for N congruent to 3 modulo 4](../../../../../ghz-contradiction-for-n-congruent-to-3-modulo-4.md) from the larger set of odd $N$ for which simultaneous eigenstates exist.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 53](../../paper-53-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
