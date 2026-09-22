<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Give $\mathfrak g$ its [Adjoint representation](../../../../../adjoint-representation-of-a-lie-algebra.md) and use the [tensor product of Lie algebra representations](../../../../../tensor-product-of-lie-algebra-representations.md). Define the [action map of a Lie algebra representation](../../../../../action-map-of-a-lie-algebra-representation.md)

$$
\boxed{a:\mathfrak g\otimes V\longrightarrow V,\qquad a(x\otimes v)=xv.}
$$

For $y\in\mathfrak g$, the action on the source is $y(x\otimes v)=[y,x]\otimes v+x\otimes yv$. The defining representation identity then gives

$$
a(y(x\otimes v))=[y,x]v+x(yv)=y(xv)=y\,a(x\otimes v).
$$

Thus $a$ is a [Lie algebra representation homomorphism](../../../../../lie-algebra-representation-homomorphism.md).

If $V$ is nontrivial and simple, the action is not identically zero, so the image of $a$ is a nonzero submodule. Simplicity forces $a$ to be surjective. For a finite-dimensional $V$ and a [semisimple Lie algebra](../../../../../semisimple-lie-algebra-split.md), the [Weyl complete reducibility theorem](../../../../../weyl-complete-reducibility-theorem.md) provides an invariant complement $U$ to $\ker a$ in $\mathfrak g\otimes V$. The restriction $a|_U$ is then an isomorphism onto $V$, giving

$$
\boxed{\mathfrak g\otimes V\cong\ker a\oplus V.}
$$

This proves the requested summand assertion in the finite-dimensional setting.

If finite dimensionality is not implicit, the final assertion needs that hypothesis: the [action summand can fail for an infinite-dimensional simple module](../../../../../action-summand-can-fail-for-an-infinite-dimensional-simple-module.md). Here is an explicit counterexample. Take $\mathfrak g=\mathfrak{sl}_2$ with $[h,e]=2e$, $[h,f]=-2f$, $[e,f]=h$, and the [Verma module](../../../../../verma-module.md) of [highest weight](../../../../../highest-weight-of-a-representation.md) $-2$:

$$
V=\bigoplus_{m\ge0}\mathbb Cv_m,\qquad
fv_m=v_{m+1},\quad hv_m=(-2-2m)v_m,\quad ev_m=-m(m+1)v_{m-1}.
$$

The lowering coefficient never vanishes for $m>0$, so an [invariant subspace](../../../../../invariant-subspace.md), using the distinct $h$-weights to isolate a basis vector and then raising, contains $v_0$ and hence all of $V$. Thus $V$ is simple.

In $\mathfrak{sl}_2\otimes V$, a vector of [weight](../../../../../weight-representation-theory.md) $-2$ is $A e\otimes v_1+B h\otimes v_0$. Applying $e$ gives $-2(A+B)e\otimes v_0$, so its highest vectors are precisely the multiples of $w=e\otimes v_1-h\otimes v_0$. But $w=f(e\otimes v_0)$, and $e\otimes v_0$ has [weight](../../../../../weight-representation-theory.md) zero, absent from $V$. Every homomorphism $r:\mathfrak g\otimes V\to V$ therefore kills this vector and then kills $w$. Any embedded copy of $V$ would send its highest vector to a nonzero multiple of $w$, so it cannot admit a projection back to $V$. This rules out a direct summand, not merely a splitting of the particular action map.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 4](../../paper-4-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
