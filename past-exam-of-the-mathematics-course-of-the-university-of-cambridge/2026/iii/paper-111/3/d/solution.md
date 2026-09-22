<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

There is a missing hypothesis in the printed claim: it is false when every irreducible component of $W$ has type $A_1$. The intended statement holds as soon as $W$ has an [irreducible component](../../../../../../irreducible-coxeter-system.md) of rank at least two, which we now assume.

Since $q=p$, every [Hecke parameter of a BN-pair](../../../../../../hecke-parameter-of-a-bn-pair.md) vanishes in $k$, and $H$ is the [0-Hecke algebra](../../../../../../0-hecke-algebra.md) with

$$
T_i^2=-T_i.
$$

Let $w_0$ be the [longest element of a finite Coxeter group](../../../../../../longest-element-of-a-coxeter-group.md). Choose a simple generator $s$ in a component of rank at least two, put

$$
r=w_0sw_0,qquad v=w_0s,qquad X=T_v+T_{w_0}.
$$

The element $r$ is again a simple generator. The identities $rv=w_0$ and $\ell(w_0)=\ell(v)+1$ give

$$
T_rX=T_{w_0}-T_{w_0}=0.
$$

If $t\ne r$ is simple, then $t$ is a left descent of both $v$ and $w_0$: using $\ell(w_0u)=\ell(w_0)-\ell(u)$, one gets $\ell(tv)=\ell(v)-1$. Hence

$$
T_tX=-T_v-T_{w_0}=-X.
$$

The one-dimensional subspace $kX$ is therefore a [left ideal](../../../../../../left-ideal.md). It is nonzero because $T_v$ and $T_{w_0}$ are distinct basis elements.

Every [reduced expression in a Coxeter group](../../../../../../reduced-expression-in-a-coxeter-group.md) for $v=w_0s$ contains $r$: in an irreducible finite component of rank at least two, deleting one final generator from $w_0$ does not remove any vertex from its support. A reduced expression for $w_0$ contains $r$ as well. Since $T_rX=0$, associativity now gives

$$
T_vX=T_{w_0}X=0,
\qquad
X^2=(T_v+T_{w_0})X=0.
$$

If $H$ were a [semisimple algebra](../../../../../../semisimple-algebra.md), the left ideal $kX$ would be a direct summand of the regular module. The corresponding projection would produce a nonzero idempotent in $kX$, impossible because $(kX)^2=0$. Thus $H$ is not semisimple.

For completeness, if $W\cong(A_1)^m$, then

$$
H\cong k[T_1,\ldots,T_m]/(T_i(T_i+1))
\cong(k\times k)^{\otimes m},
$$

which is semisimple. This is the counterexample showing why the omitted rank condition is necessary.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 111](../../../paper-111-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
