<h1 id="s7/3/5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

For the standard meaning of a [canonical transformation](../../../../../canonical-transformation.md), the new coordinates must retain Hamiltonian form for every Hamiltonian, with the same physical function expressed in the new coordinates. Let $z=(q,p)$, $Z=F(z)=(Q,P)$, $S=DF$ and $J=\begin{pmatrix}0&I\\-I&0\end{pmatrix}$. With $K(Z)=H(F^{-1}(Z))$, the [chain rule](../../../../../chain-rule.md) gives

$$
\dot Z=S J S^T\nabla_ZK.
$$

Agreement with $\dot Z=J\nabla_ZK$ for arbitrary $K$ forces $SJS^T=J$. Its matrix entries are precisely the [Poisson brackets](../../../../../poisson-bracket.md) of the new coordinates, so

$$
\boxed{\{Q_i,Q_j\}=0,\qquad\{P_i,P_j\}=0,\qquad\{Q_i,P_j\}=\delta_{ij}.}
$$

The qualification for every Hamiltonian matters. [Preserving one Hamiltonian flow does not imply canonicality](../../../../../preserving-one-hamiltonian-flow-does-not-imply-canonicality.md). For example, with two coordinate pairs and $H=(q_1^2+p_1^2)/2$, the invertible change $Q_1=q_1$, $P_1=p_1$, $Q_2=2q_2$, $P_2=p_2$ preserves the equations and the same physical Hamiltonian, but $\{Q_2,P_2\}=2$. Thus a definition requiring only one chosen Hamiltonian flow is too weak to prove the claimed bracket identities. The universal definition supplies the missing condition.

## ↑ Ancestors (12)

1. [5](../5.md)
2. [3](../../3.md)
3. [S7](../../../s7.md)
4. [2015](../../../../2015-split.md)
5. [Past exam of the short options paper shared by Prelims and Parts A and B of the physics course of the University of Oxford](../../../../split.md)
6. [Short options paper shared by Prelims and Parts A and B of the physics course of the University of Oxford](../../../../../short-options-paper-shared-by-prelims-and-parts-a-and-b-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
