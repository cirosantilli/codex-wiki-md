<h1 id="18i/solution">Solution</h1>

↑ **Parent:** [18I](../18i.md)

Let $G$ be the [Galois group of a polynomial](../../../../../galois-group-of-a-polynomial.md) of the irreducible quartic. Irreducibility makes $G$ a transitive subgroup of $S_4$. The three roots of the given [cubic resolvent of a quartic](../../../../../cubic-resolvent-of-a-quartic.md) correspond to the three partitions of the four quartic roots into two unordered pairs, and the kernel of the $S_4$-action on these partitions is the [Klein four-group](../../../../../klein-four-group.md) $V_4$. If the resolvent has Galois group $S_3$, the image of $G$ in this action is all of $S_3$. Among the [transitive subgroups of the symmetric group on four points](../../../../../transitive-subgroups-of-the-symmetric-group-on-four-points.md), only $S_4$ has this image. Hence

$$
\boxed{\ \operatorname{Gal}(f/\mathbb Q)\cong S_4.\ }
$$

Now put $f_p(t)=t^4+pt+p$. The [Eisenstein criterion](../../../../../eisenstein-criterion.md) at $p$ proves that $f_p$ is an [irreducible polynomial](../../../../../irreducible-polynomial.md), and its cubic resolvent is

$$
g_p(t)=t^3-4pt-p^2.
$$

Its [discriminant of a depressed cubic](../../../../../discriminant-of-a-depressed-cubic.md) is

$$
\Delta_p=256p^3-27p^4=p^3(256-27p).
$$

For odd $p$, the $p$-adic valuation of $\Delta_p$ is three because $p\nmid256$; for $p=2$, $\Delta_2=2^4\cdot101$. Thus $\Delta_p$ is never a square in $\mathbb Q$.

By the [rational root theorem](../../../../../rational-root-theorem.md), a reducible $g_p$ has an integer root among $\pm1,\pm p,\pm p^2$. Reduction modulo $p$ shows that the root is divisible by $p$; writing it as $pk$, with $k\in\{\pm1,\pm p\}$, gives

$$
pk^3-4k-1=0.
$$

The only possibilities are $k=-1,p=3$ and $k=1,p=5$, corresponding to roots $-3$ and $5$. For every other prime, $g_p$ is irreducible with nonsquare discriminant, so its Galois group is $S_3$ and the criterion above gives the quartic group $S_4$. For $p=3$ or $5$, the reducible resolvent makes the quartic group a proper subgroup. Therefore

$$
\boxed{\ p=3\ \text{or}\ p=5.\ }
$$

## ↑ Ancestors (10)

1. [18I](../18i.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
