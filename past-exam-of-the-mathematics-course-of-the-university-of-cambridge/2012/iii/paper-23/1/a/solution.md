<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $M\times X$ have the diagonal [right monoid action](../../../../../../right-monoid-action.md) $(g,x)m=(gm,xm)$, and put $E=\operatorname{Hom}_M(M\times X,Y)$. Define the right action on this set of [equivariant maps of monoid sets](../../../../../../equivariant-map-of-monoid-sets.md) by

$$
(ek)(g,x)=e(kg,x).
$$

It really stays in $E$: $(ek)(gm,xm)=e(kgm,xm)=e(kg,x)m$. Also $e1=e$ and $((ek)l)(g,x)=e(klg,x)=(e(kl))(g,x)$, so it satisfies the right-action law. Left multiplication in the first argument is intentional; no commutativity of $M$ has been assumed.

Define the [evaluation map of an exponential object](../../../../../../evaluation-map-of-an-exponential-object.md)

$$
\operatorname{ev}:E\times X\to Y,\qquad \operatorname{ev}(e,x)=e(1,x).
$$

It is equivariant, because

$$
\operatorname{ev}(ek,xk)=e(k,xk)=e((1,x)k)=e(1,x)k.
$$

For any right $M$-set $Z$ and [equivariant map](../../../../../../equivariant-map.md) $h:Z\times X\to Y$, define its [currying](../../../../../../currying.md) by

$$
\widehat h(z)(g,x)=h(zg,x).
$$

For fixed $z$, this is equivariant in the diagonal variables: $h(zgm,xm)=h(zg,x)m$. The map $z\mapsto\widehat h(z)$ is also equivariant, since

$$
\widehat h(zk)(g,x)=h(zkg,x)=(\widehat h(z)k)(g,x).
$$

It satisfies $\operatorname{ev}(\widehat h(z),x)=h(z,x)$.

Conversely, given an equivariant $u:Z\to E$, set $h(z,x)=u(z)(1,x)$. Evaluation makes this equivariant, and currying recovers $u$:

$$
\widehat h(z)(g,x)=u(zg)(1,x)=(u(z)g)(1,x)=u(z)(g,x).
$$

These constructions are inverse and natural in $Z$. Therefore they establish the [exponential object](../../../../../../exponential-object.md) universal property

$$
\boxed{\operatorname{Hom}_M(Z,E)\cong\operatorname{Hom}_M(Z\times X,Y),\qquad
Y^X=E.}
$$

This is the [exponential of right monoid actions](../../../../../../exponential-of-right-monoid-actions.md), not the set of ordinary maps $X\to Y$ with an arbitrarily guessed action.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 23](../../../paper-23-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
