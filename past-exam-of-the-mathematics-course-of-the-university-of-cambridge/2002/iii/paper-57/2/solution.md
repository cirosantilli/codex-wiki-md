<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Use a basal resource $X_1$, herbivore $X_2$ and predator $X_3$, with positive encounter, conversion and mortality parameters:

$$
\dot X_1=X_1(r-a_1X_2),\qquad
\dot X_2=X_2(b_1X_1-d_2-a_2X_3),\qquad
\dot X_3=X_3(b_2X_2-d_3).
$$

Only the resource has intrinsic positive growth; the consumers die without food. There is no resource carrying capacity, immigration or feeding on nonadjacent levels. These assumptions define the simplest [food chain](../../../../../food-chain.md) with [Lotka-Volterra equations](../../../../../lotka-volterra-equations.md).

A positive [equilibrium](../../../../../equilibrium-point-of-a-dynamical-system.md) would require both $X_2=r/a_1$ and $X_2=d_3/b_2$. Hence three-level coexistence is possible only on the special balance $\kappa=b_2r/a_1-d_3=0$. The exact identity

$$
\boxed{X_1^{b_2}X_3^{a_1}=C\exp[(b_2r-a_1d_3)t]}
$$

follows by combining $b_2\,d\log X_1/dt$ and $a_1\,d\log X_3/dt$. It gives a useful classification rather than incorrectly postulating a generic coexistence fixed point.

If $\kappa<0$, the top predator cannot invade the underlying resource-herbivore cycle: its average per-capita growth there is $\kappa$. This extinction statement can be strengthened. The boundary [equilibrium](../../../../../equilibrium-point-of-a-dynamical-system.md) has $X_{1*}=d_2/b_1$, $X_{2*}=r/a_1$, $X_{3*}=0$. With weights $w_1=1$, $w_2=a_1/b_1$, $w_3=a_1a_2/(b_1b_2)$, define

$$
V=\sum_{i=1}^2w_i\bigl[X_i-X_{i*}-X_{i*}\log(X_i/X_{i*})\bigr]+w_3X_3.
$$

Direct cancellation of paired trophic terms gives $\dot V=w_3\kappa X_3<0$. Its level sets bound the first two species above and away from zero and bound $X_3$. Integration and uniform continuity imply $X_3\to0$; the limiting dynamics are the usual resource-herbivore closed orbits, not generally an attracting [equilibrium](../../../../../equilibrium-point-of-a-dynamical-system.md).

If $\kappa=0$, there is a line of positive [equilibria](../../../../../equilibrium-point-of-a-dynamical-system.md): $X_2=r/a_1$, $b_1X_1-a_2X_3=d_2$. Choosing any positive point on that line gives a conserved coercive version of $V$ with all three relative-entropy terms. Together with the product integral, it confines generic trajectories to closed curves, with neutral oscillations around the [equilibrium](../../../../../equilibrium-point-of-a-dynamical-system.md) line. All three can persist, but only under this finely balanced parameter condition.

If $\kappa>0$, the product identity grows without bound, so at least one of $X_1,X_3$ must become unbounded in the unregulated model. There is no bounded persistent three-species attractor. Finite-time blow-up is excluded by a weighted total-abundance bound whose encounter terms cancel and whose derivative is at most a constant times that abundance. The unbounded long-term behavior signals the missing biological resource regulation. **The simplest odd chain does not generically permit bounded full coexistence; adding resource self-limitation changes this conclusion.**

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 57](../../paper-57-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
