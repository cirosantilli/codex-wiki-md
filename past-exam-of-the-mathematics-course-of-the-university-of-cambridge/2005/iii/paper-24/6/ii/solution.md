<h1 id="6/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [homotopy fibre](../../../../../../homotopy-fiber.md) is the [homotopy pullback](../../../../../../homotopy-pullback.md) of the [path fibration](../../../../../../path-space-fibration.md) over the target sphere along $f$. The [Sullivan fibre-model theorem](../../../../../../sullivan-fibre-model-theorem.md) computes it by taking a relative acyclic model of that [path fibration](../../../../../../path-space-fibration.md) and tensoring it over the target model with the source model. Here the construction can be written out and checked directly.

Adjoin $a$ of degree $2n-1$ and $b$ of degree $4n-2$ to the sphere model, with

$$
Da=u,\qquad Db=v-au,\qquad Du=0,\quad Dv=u^2.
$$

This is a differential, because $D(v-au)=u^2-u^2=0$. It is an acyclic [relative Sullivan algebra](../../../../../../relative-sullivan-algebra.md): putting $v'=v-au$ makes its two pairs $Da=u$ and $Db=v'$. The first is a polynomial generator killed by an odd generator; the second is an odd generator killed by an even polynomial generator. Each pair has [cohomology](../../../../../../cohomology-split.md) only $\mathbb Q$, the second by the ordinary polynomial antiderivative calculation in [characteristic zero](../../../../../../characteristic-zero.md). Hence this models the contractible path space, and its augmentation models the chosen basepoint.

Tensoring with the projective-space model via the map in part (i) gives

$$
B=(\Lambda(x,y,a,b),D),\qquad
Dx=0,\quad Dy=x^{n+1},\quad Da=x^n,
\quad Db=x^{n-1}y-a x^n.
$$

The last differential is necessary: using only $Db=f^*v$ would give $D^2b=x^{2n}\ne0$. Make the invertible generator change $z=y-xa$, of degree $2n+1$. Since $x$ is even,

$$
Dz=x^{n+1}-x x^n=0,
\qquad Db=x^{n-1}(z+xa)-a x^n=x^{n-1}z.
$$

For $n\ge2$, all nonzero differentials are decomposable and the generator ordering $x,a,z,b$ is Sullivan. Thus no further minimization is needed:

$$
\boxed{M(F)=(\Lambda(x_2,a_{2n-1},z_{2n+1},b_{4n-2}),D),
\quad Dx=Dz=0,\quad Da=x^n,\quad Db=x^{n-1}z.}
$$

For example at $n=2$ this is $(\Lambda(x_2,a_3,z_5,b_6),Da=x^2,Db=xz)$.

The indecomposable generators of a [simply connected](../../../../../../simply-connected-space.md) finite-type [minimal model](../../../../../../sullivan-minimal-model.md) are dual to its [rational homotopy groups](../../../../../../rational-homotopy-group.md). Therefore, for $n\ge2$,

$$
\boxed{\pi_k(F)\otimes\mathbb Q\cong
\begin{cases}\mathbb Q,&k=2,\ 2n-1,\ 2n+1,\ 4n-2,\\0,&\text{otherwise}.\end{cases}}
$$

These four degrees are distinct. The exact [homotopy](../../../../../../homotopy.md) sequence provides an independent check: $\mathbb{CP}^n$ has rational [homotopy](../../../../../../homotopy.md) only in degrees $2,2n+1$, while $S^{2n}$ has it in degrees $2n,4n-1$. For $n\ge2$ these source and target degrees do not overlap, so the source classes survive in the fibre and the target classes contribute their one-degree-lower connecting classes, giving the same four groups.

At $n=1$, the displayed relative fibre algebra is not minimal: $Da=x$ and $Db=z$ are linear pairs. Cancelling both acyclic pairs leaves $\mathbb Q$. Accordingly

$$
\boxed{M(F)=\mathbb Q,\qquad \pi_k(F)\otimes\mathbb Q=0\quad(n=1).}
$$

This agrees with $\mathbb{CP}^1\cong S^2$ and the degree-one map being a [homotopy](../../../../../../homotopy.md) equivalence. The case distinction is required before reading [homotopy groups](../../../../../../homotopy-group.md) from the generators.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [6](../../6.md)
3. [Paper 24](../../../paper-24-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
