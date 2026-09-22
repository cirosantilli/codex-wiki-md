<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The orbits of $N_\alpha\trianglelefteq G_\alpha$ on $\Omega\setminus\{\alpha\}$ have a common size $r$, because $G_\alpha$ is transitive there. Suppose $N$ has a [block system](../../../../../../block-system.md) of block size $b$, $1<b<n$. Since $r\mid n-1$ and $b\mid n$, $\gcd(r,b)=1$. Let $B$ be the block of $\alpha$ and $C\ne B$ another block. The union $N_\alpha C$ is a union of blocks and of r-element point-orbits, so its size is divisible by $br$; it is at most $br$. Equality means each of the b point-orbits meets $C$ once. Thus $N_{\alpha\beta}$ fixes $C$ pointwise for $\beta\in C$. Interchanging $\alpha,\beta$ also makes it fix $B$. All two-point stabilizers have order $|N_\alpha|/r$. Therefore $N_{\alpha\beta}=N_{\alpha\gamma}$ for every $\gamma\in B\setminus\{\alpha\}$. Varying $\beta$ outside $B$ shows this same [subgroup](../../../../../../subgroup.md) fixes every point, so it is trivial. We have proved [uniform subdegrees force an imprimitive action to be Frobenius](../../../../../../uniform-subdegrees-force-an-imprimitive-action-to-be-frobenius.md): no nonidentity element of $N$ fixes two points.

Write $|N_\alpha|=h$. The distinct [point stabilizers](../../../../../../stabilizer-subgroup.md) meet only at $1$, and $|N|=nh$. Thus the set $D$ of fixed-point-free elements of $N$ has size

$$
|D|=nh-\bigl(1+n(h-1)\bigr)=n-1.
$$

Count triples $(\alpha,\beta,x)$ with $x\in D$ and $x\alpha=\beta$: there are $n(n-1)$, exactly the number of ordered distinct pairs. [Conjugation](../../../../../../conjugation.md) by the [two-transitive](../../../../../../two-transitive-group-action.md) [group](../../../../../../group-split.md) makes every pair occur, hence each pair has a unique such $x$. It follows that $G$ conjugates all elements of $D$ transitively.

Also $h\mid n-1$, since $N_\alpha$ acts freely on the remaining points. For each prime $p\mid n$, [Cauchy's theorem for finite groups](../../../../../../cauchy-theorem-for-groups.md) supplies an order-p element of $N$; it cannot fix a point, since $p\nmid h$. Conjugacy of $D$ forces all these primes to coincide, so $n=p^d$ and every element of $D$ has order $p$. A [Sylow subgroup](../../../../../../sylow-subgroup.md) $P$ of $N$ has order $n$, because $p\nmid h$. Every nonidentity element of $P$ is fixed-point-free, so $P=\{1\}\cup D$. This uniquely described [subgroup](../../../../../../subgroup.md) is normal in $G$. Minimal normality of $N$ gives $P=N$, and $|N|=n$. **Therefore $N$ is regular.** The proof establishes closure through a [Sylow subgroup](../../../../../../sylow-subgroup.md); it does not assume that a set of derangements is automatically a [subgroup](../../../../../../subgroup.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
