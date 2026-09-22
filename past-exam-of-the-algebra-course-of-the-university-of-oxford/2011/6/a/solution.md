<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The identity column gives the [group order](../../../../order-of-a-finite-group.md) as the sum of squared [irreducible character degrees](../../../../irreducible-character-degree.md):

$$
\boxed{|G|=1+4\cdot7^2+8^2+3\cdot9^2=504.}
$$

By [column orthogonality](../../../../column-orthogonality.md), the squared norm of a column is the corresponding [centralizer](../../../../centralizer.md) order. In source order these orders and the resulting [conjugacy class](../../../../conjugacy-class.md) sizes are

$$
\boxed{|C_G(g)|=(504,8,9,9,9,9,7,7,7),}
$$



$$
|g^G|=(1,63,56,56,56,56,72,72,72).
$$

For example the fourth column has squared norm $1+1+(|\alpha|^2+|\beta|^2+|\gamma|^2)+1=9$, while the seventh has squared norm $1+1+(|\xi|^2+|\eta|^2+|\phi|^2)=7$.

An element's order divides its [centralizer](../../../../centralizer.md) order. [Cauchy's theorem for finite groups](../../../../cauchy-theorem-for-groups.md) provides an [involution](../../../../involution.md), and only $C_2$ has an even [centralizer](../../../../centralizer.md) order. Hence that entire class consists of [involutions](../../../../involution.md). The last three classes consist of elements of order seven. In $C_3,C_4,C_5,C_6$ the possibilities are three and nine. The three real numbers $\alpha,\beta,\gamma$ are roots of $t^3-3t+1$, which has no rational root and is irreducible over $\mathbb Q$. A real [character](../../../../character-of-a-representation.md) value at an element of order three belongs to $\mathbb Q(e^{2\pi i/3})\cap\mathbb R=\mathbb Q$. Therefore the irrational real entries in $C_4,C_5,C_6$ rule out order three there. Cubing any of these order-nine elements produces an element of order three, which must belong to the sole remaining class $C_3$. Thus

$$
\boxed{\operatorname{ord}(C_1),\ldots,\operatorname{ord}(C_9)
=(1,2,3,9,9,9,7,7,7).}
$$

The three deductions below give nine [Sylow subgroups](../../../../sylow-subgroup.md) for $2$ with pairwise trivial intersections. Their conjugation action is transitive. Fix one, $S$. If $T\ne S$, put $H=S\cap N_G(T)$. The product $HT$ is a $2$-[subgroup](../../../../subgroup.md), so maximality of $T$ gives $H\leq T$. Trivial intersection then gives $H=1$. Thus the [orbit](../../../../orbit-dynamical-system.md) of $T$ under $S$ has size eight, exhausting the other eight points. The point [stabilizer](../../../../stabilizer-subgroup.md) $N_G(S)$ is therefore transitive on the remaining points: **the action is doubly transitive**.

For a doubly transitive action, its [permutation character](../../../../permutation-character.md) has the form $1+\theta$ with $\theta$ irreducible. Here $\theta(1)=8$, and the unique degree-eight row is $\chi_6$. Therefore the numbers of fixed points are the entries of

$$
\boxed{\pi=\chi_1+\chi_6=(9,1,0,0,0,0,2,2,2).}
$$

Every nonidentity element consequently fixes at most two points. This also shows that the action is faithful.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [6](../../6.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the algebra course of the University of Oxford](../../../split.md)
5. [Algebra course of the University of Oxford](../../../../algebra-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
