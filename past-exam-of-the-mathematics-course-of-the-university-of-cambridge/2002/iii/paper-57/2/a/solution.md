<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Add a fourth level using

$$
\dot X_3=X_3(b_2X_2-d_3-a_3X_4),\qquad
\dot X_4=X_4(b_3X_3-d_4),
$$

with the first two equations unchanged. The positive [equilibrium](../../../../../../equilibrium-point-of-a-dynamical-system.md) must be

$$
\boxed{X_{2*}=\frac r{a_1},\quad X_{3*}=\frac{d_4}{b_3},\quad
X_{1*}=\frac{d_2+a_2d_4/b_3}{b_1},\quad
X_{4*}=\frac{b_2r/a_1-d_3}{a_3}.}
$$

The first three entries are positive automatically. The fourth is positive exactly when $b_2r/a_1>d_3$. Thus the printed coexistence assertion requires adequate herbivore production to support the third and fourth levels; it is not true for every positive parameter set. The top predator supplies the extra mortality that was absent in the unbounded three-level case.

For a chain of $N$ levels, the same equations give $b_{i-1}X_{i-1}-d_i-a_iX_{i+1}=0$ in the interior, with the basal and top equations fixing alternating levels. The interaction [matrix](../../../../../../matrix.md) has zero diagonal and opposite-sign nearest-neighbor entries. Its [determinant](../../../../../../determinant.md) is nonzero for even $N$ and zero for odd $N$: expansion at the end gives $\det A_N=a_{N-1}b_{N-1}\det A_{N-2}$, with $\det A_0=1$, $\det A_1=0$. For even $N$ this gives a unique [equilibrium](../../../../../../equilibrium-point-of-a-dynamical-system.md) candidate, but its entries still need to be positive. For odd $N$ a compatibility condition is necessary, just as for the three-level example. This is [Lotka-Volterra food-chain parity](../../../../../../lotka-volterra-food-chain-parity.md). The parity result is specific to an exponential unregulated resource and nearest-neighbor trophic interactions.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 57](../../../paper-57-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
