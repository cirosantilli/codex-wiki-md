<h1 id="5d/solution">Solution</h1>

↑ **Parent:** [5D](../5d.md)

The [Lagrange theorem](../../../../../lagrange-s-theorem.md) states that $|H|$ divides $|G|$ for every [subgroup](../../../../../subgroup.md) $H$ of a finite [group](../../../../../group-split.md) $G$, with $|G|=|G:H||H|$. The left cosets partition $G$, and multiplication by a representative bijects $H$ with each coset, proving the formula.

The intersection $H\cap K$ contains the identity and is closed under $xy^{-1}$, so it is a [subgroup](../../../../../subgroup.md). Its order divides both $|H|$ and $|K|$; if these are coprime, $H\cap K=\{e\}$.

The order $o(x)$ is the least positive $m$ with $x^m=e$. Division $k=qm+r$, $0\leq r<m$, shows that $x^k=e$ exactly when $r=0$, so exactly when $o(x)\mid k$.

If $x,y$ commute and have coprime orders $m,n$, then $(xy)^{mn}=e$. Conversely $(xy)^r=e$ implies $x^r=y^{-r}$ lies in $\langle x\rangle\cap\langle y\rangle=\{e\}$, so $m,n\mid r$ and $mn\mid r$. Hence $o(xy)=mn$.

[Cauchy theorem for groups](../../../../../cauchy-theorem-for-groups.md) says that every prime divisor $p$ of $|G|$ occurs as the order of an element of $G$. For $|G|=26$, the Sylow $13$-subgroup $P\cong C_{13}$ is unique and normal, and Cauchy's theorem supplies a complement $C_2$. Thus $G=C_{13}\rtimes C_2$. The homomorphism $C_2\to\operatorname{Aut}(C_{13})\cong C_{12}$ is either trivial or has the unique image of order two, inversion. These give exactly $C_{26}$ and the dihedral [group](../../../../../group-split.md) of order $26$.

## ↑ Ancestors (10)

1. [5D](../5d.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
