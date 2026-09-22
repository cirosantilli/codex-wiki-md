<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Insert the two observed spins into the configuration sum for the [transfer matrix for a classical spin chain](../../../../transfer-matrix-for-a-classical-spin-chain.md) [trace](../../../../matrix-trace.md). Since the diagonal matrix $\sigma^z$ has entry $s$ on state $s$, multiplication by it at positions $j$ and $j+r$ produces the factor $\sigma_j\sigma_{j+r}$. The [trace](../../../../matrix-trace.md) representation is consequently

$$
\boxed{g(r)=\frac1{Z_N}\operatorname{Tr}\!\left[T^{j-1}\sigma^zT^r\sigma^zT^{N+1-j-r}\right].}
$$

There are exactly $N$ transfer factors: $(j-1)+r+(N+1-j-r)=N$. The distance between the two insertions is $r$ bonds, not $r-1$. Cyclicity of the [trace](../../../../matrix-trace.md) combines the outside factors and gives the equivalent expression

$$
g(r)=Z_N^{-1}\operatorname{Tr}(\sigma^zT^r\sigma^zT^{N-r}),
$$

which makes independence of the starting site manifest. No assumption that $T$ commutes with $\sigma^z$ is used; in general it does not. For $r=0$ the two insertions multiply to the identity and $g(0)=1$, a useful [normalization](../../../../normalization.md) check.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [4](../../4.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the theoretical physics major option course of the University of Oxford](../../../split.md)
5. [Theoretical physics major option course of the University of Oxford](../../../../theoretical-physics-major-option-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
