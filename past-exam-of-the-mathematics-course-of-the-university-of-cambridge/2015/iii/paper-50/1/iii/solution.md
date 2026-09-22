<h1 id="1/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For the all-[kink](../../../../../../scalar-field-kink.md) sector, keep $\alpha_{ij}=\tanh^2[(\theta_i-\theta_j)/2]$ and $E_i=e^{X_i}$. Enumerating the even and odd binary configurations gives the [Hirota tau functions](../../../../../../hirota-tau-function.md)

$$
\begin{aligned}
f&=1-\alpha_{12}E_1E_2-\alpha_{13}E_1E_3-\alpha_{23}E_2E_3,\\
g&=E_1+E_2+E_3-\alpha_{12}\alpha_{13}\alpha_{23}E_1E_2E_3.
\end{aligned}
$$

The last minus sign is the product of three negative pair coefficients. As in the two-body limit, **the three velocities are $v_i=\beta_i/\kappa_i=\tanh\theta_i$**.

To follow the first [kink](../../../../../../scalar-field-kink.md), keep $X_1$ bounded and take $t\to\pm\infty$. Let $J_\pm$ be the set of spectators whose exponential diverges in that limit:

$$
J_+=\{j\in\{2,3\}:v_1>v_j\},\qquad J_-=\{j\in\{2,3\}:v_1<v_j\}.
$$

For no large spectators, $g/f\to E_1$. For one large spectator $j$, $g/f\to-1/(\alpha_{1j}E_1)$. For two large spectators, the dominant terms give $g/f\to\alpha_{12}\alpha_{13}E_1$. On a continuous [branch of a multivalued function](../../../../../../branch-of-a-multivalued-function.md), each case has local profile $4\arctan\exp(X_1+c_\pm)$ plus the appropriate vacuum offset, where

$$
c_\pm=\sum_{j\in J_\pm}\log\alpha_{1j}.
$$

Consequently the incoming and outgoing intercepts are $-(\gamma_1+c_-)/\kappa_1$ and $-(\gamma_1+c_+)/\kappa_1$. This proves

$$
\boxed{\Delta^{(3)}t[v_1;v_2,v_3]=\frac1{\beta_1}\sum_{j=2}^{3}\operatorname{sgn}(v_1-v_j)\log\alpha_{1j}=\Delta^{(2)}t[v_1;v_2]+\Delta^{(2)}t[v_1;v_3].}
$$

Again the time expression requires $v_1\ne0$ and distinct velocities; the corresponding spatial-shift identity holds also when $v_1=0$. With mixed orientations, use the general pair shift established above and determine growing spectators by the sign of $\kappa_j(v_1-v_j)$; the same multiplication of pair coefficients proves additivity.

**There is no independent three-body contribution to the asymptotic shift.** The [pairwise additivity of soliton shifts](../../../../../../pairwise-additivity-of-soliton-shifts.md) is a classical manifestation of [factorized scattering](../../../../../../factorized-scattering.md) in an [integrable partial differential equation](../../../../../../integrable-partial-differential-equation.md). The collision preserves the individual asymptotic [rapidities](../../../../../../rapidity.md) and profiles, and the net shift is independent of the sequence of separated pair collisions. In the quantum theory, consistency of the corresponding species-changing [S-matrices](../../../../../../s-matrix.md) becomes the [Yang-Baxter equation](../../../../../../yang-baxter-equation.md); the classical scalar shift identity is its physical precursor, rather than a derivation of all quantum matrix identities.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [1](../../1.md)
3. [Paper 50](../../../paper-50-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
