<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

If $|G|=p^am$ with $p\nmid m$, a [Sylow subgroup](../../../../sylow-subgroup.md) for $p$ has order $p^a$. Let $P,Q$ be two such [subgroups](../../../../subgroup.md). The action of $P$ by left translation on $G/Q$ has [orbits](../../../../orbit-dynamical-system.md) of powers of $p$, while $|G/Q|=m$ is prime to $p$. There is a fixed coset $gQ$, giving $g^{-1}Pg\leq Q$; equality follows from their orders. Thus **all Sylow $p$-[subgroups](../../../../subgroup.md) are conjugate**.

Let $P$ now act by conjugation on their set. If it fixes $Q$, then $P\leq N_G(Q)$, so $PQ$ is a [subgroup](../../../../subgroup.md) of $p$-power order and must equal $Q$; hence $P=Q$. The unique fixed point is $P$ itself and all other [orbits](../../../../orbit-dynamical-system.md) have size divisible by $p$. Consequently $\boxed{n_p\equiv1\pmod p}$.

For the strengthened conclusion, the [stabilizer](../../../../stabilizer-subgroup.md) of $Q\ne P$ is $H=P\cap N_G(Q)$. The product $HQ$ is a [subgroup](../../../../subgroup.md) of $p$-power order, so $H\leq Q$. If distinct [Sylow subgroups](../../../../sylow-subgroup.md) meet trivially, then $H\leq P\cap Q=1$. Every other [orbit](../../../../orbit-dynamical-system.md) therefore has the full size $|P|$, giving

$$
\boxed{n_p\equiv1\pmod{|P|}.}
$$

Conjugacy also gives $n_p=[G:N_G(P)]$, a divisor of $[G:P]$.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [4](../../4.md)
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
