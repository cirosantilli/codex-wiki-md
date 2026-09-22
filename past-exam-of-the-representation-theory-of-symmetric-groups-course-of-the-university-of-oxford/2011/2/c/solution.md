<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Identify $M=M_F^{(n-1,1)}$ with $F^n$, whose [basis vectors](../../../../basis-vector.md) record the singleton row. Put

$$
T=F(1,\ldots,1),\qquad U=\{(a_1,\ldots,a_n):\textstyle\sum_i a_i=0\}=S_F^{(n-1,1)}.
$$

If the [characteristic](../../../../characteristic-of-a-field.md) does not divide $n$, then $M=T\oplus U$, and $U$ is simple. If it divides $n$, then $0<T<U<M$ is the [submodule](../../../../submodule.md) chain, with $T$ and $M/U$ trivial and $U/T$ simple of [dimension](../../../../dimension-vector-space.md) $n-2$. In both cases there are no additional [submodules](../../../../submodule.md): any vector with unequal coordinates yields a nonzero multiple of $e_i-e_j$ by subtracting its [image](../../../../image-of-a-function.md) under $(i,j)$, and the [orbit](../../../../orbit-dynamical-system.md) of such a difference spans $U$. A [submodule](../../../../submodule.md) containing no nonconstant vector is contained in $T$.

Now suppose $p\nmid n$. When $p\neq2$, part (b)'s valid vanishing $\operatorname{Hom}_{S_n}(M,W)=0$ implies $\operatorname{Hom}_{S_n}(U,W)=0$: extend a putative map using the [projection](../../../../projection-linear-algebra.md) $M\to U$.

When $p=2$, the assumption $p\nmid n$ makes $n$ odd. The corrected calculation in part (b) says every map $M\to W$ sends its singleton-row [basis vectors](../../../../basis-vector.md) to the same multiple of the globally [invariant](../../../../invariant-mathematics.md) vector $v$. Hence it kills the augmentation [submodule](../../../../submodule.md) $U$. Extending a map $U\to W$ along the direct-sum [projection](../../../../projection-linear-algebra.md) again makes it zero. Thus, despite the characteristic-two error in the earlier claim, the requested conclusion remains valid:

$$
\boxed{p\nmid n\quad\Longrightarrow\quad\operatorname{Hom}_{FS_n}(S_F^{(n-1,1)},S_F^{(n-2,1,1)})=0.}
$$

The structural input is the [submodule lattice of the standard symmetric-group permutation module](../../../../submodule-lattice-of-the-standard-symmetric-group-permutation-module.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the representation Theory of Symmetric Groups course of the University of Oxford](../../../split.md)
5. [Representation Theory of Symmetric Groups course of the University of Oxford](../../../../representation-theory-of-symmetric-groups-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
