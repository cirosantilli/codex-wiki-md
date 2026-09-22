<h1 id="3/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Write the final [topological quantum order](../../../../../../../topological-quantum-order.md) constants as $a>0$ and $\varepsilon<1$, to avoid confusing the allowed support diameter with the small time coefficient. For any initial operator $A_X$ of [operator norm](../../../../../../../operator-norm.md) at most one,

$$
\langle\psi_0|A_X|\psi_0\rangle=\langle\psi_1|A_X(-t)|\psi_1\rangle,
$$

and similarly for the partner state. The minus sign follows from $|\psi_0\rangle=e^{itH}|\psi_1\rangle$ and the [Heisenberg picture](../../../../../../../heisenberg-picture.md) convention $A_X(t)=e^{itH}A_Xe^{-itH}$. The [Lieb-Robinson bound](../../../../../../../lieb-robinson-bound.md) and its localization corollary apply to either time direction, using $|t|$.

Choose $\operatorname{diam}(X)\leq aL/4$, $t=\tau L$ with $v\tau\leq a/8$, and localization buffer $l=aL/8$. The enlarged support $X'$ obeys

$$
\operatorname{diam}(X')\leq\operatorname{diam}(X)+2(v|t|+l)\leq3aL/4<aL.
$$

The [Lieb-Robinson localization by Haar twirling](../../../../../../../lieb-robinson-localization-by-haar-twirling.md) corollary supplies an operator $B_{X'}$ approximating $A_X(-t)$ with

$$
\delta_L:=\|A_X(-t)-B_{X'}\|\leq\mu v\tau L|X|e^{-\mu aL/16}.
$$

Do not assume that the approximate operator has norm at most one: it only has $\|B_{X'}\|\leq1+\delta_L$. Apply final-state [local indistinguishability](../../../../../../../local-indistinguishability.md) to $B_{X'}/(1+\delta_L)$. The two approximation errors then give

$$
\left|\langle\psi_0|A_X|\psi_0\rangle-\langle\widetilde\psi_0|A_X|\widetilde\psi_0\rangle\right|\leq\varepsilon(1+\delta_L)+2\delta_L.
$$

If the lattice has polynomially many sites in its diameter, $N(L)=O(L^p)$, the error tends to zero uniformly in these supports. For sufficiently large $L$, take $\delta_L\leq(1-\varepsilon)/[2(\varepsilon+2)]$. The initial pair is then indistinguishable within $\varepsilon'=(1+\varepsilon)/2<1$ on supports of diameter at most $aL/4$. Together with the exact orthogonality from condition (i), this proves **the initial state is topologically ordered for sufficiently small linear-time coefficient**. The constants for initial and final order need not be identical.

The [backward preservation of local indistinguishability](../../../../../../../backward-preservation-of-local-indistinguishability.md) has an explicit finite-system qualification: it holds whenever the displayed $L|X|e^{-\mu aL/16}$ error is small enough. The conventional bounded-density, fixed-dimensional lattice interpretation supplies that condition. The question leaves growth control implicit; for an arbitrary collection of qudits one cannot discard the $|X|$ prefactor merely because $L$ is large. This identifies exactly the assumption needed by the supplied localization proof.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [Paper 63](../../../../paper-63-split.md)
5. [Iii](../../../../split.md)
6. [2014](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
