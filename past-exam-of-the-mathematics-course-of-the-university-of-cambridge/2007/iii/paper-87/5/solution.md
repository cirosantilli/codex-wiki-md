<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Write products of [endomorphisms](../../../../../endomorphism.md) as composition, with the rightmost map applied first. Because $1$ is terminal, the only hom-sets that can contain multiple arrows are $\operatorname{Hom}(1,D)$ and $\operatorname{End}(D)$. If the latter contained only the identity, any point $p:1\to D$ would have $p!=\operatorname{id}_D$, where $!:D\to1$. Then any other point $q$ would satisfy $q=p!q=p$. Thus the category would be a [preorder](../../../../../preorder.md). The hypothesis therefore implies $|\operatorname{End}(D)|>1$.

If the product object $D\times D$ were $1$, its universal property applied to arrows from $D$ would give $\operatorname{End}(D)^2\cong\operatorname{Hom}(D,1)$, a singleton, which is impossible. Since there are only two objects, $D\times D=D$. Similarly, if $D^D=1$, the exponential adjunction at $1$ would give

$$
\operatorname{Hom}(1,1)\cong\operatorname{Hom}(1\times D,D)\cong\operatorname{End}(D),
$$

again impossible. Hence **$D\times D=D^D=D$** as chosen objects.

Let $M=\operatorname{End}(D)$, let $\pi,\pi'$ be the product projections, and let $\varepsilon:D^D\times D\to D$ be evaluation, all now [endomorphisms](../../../../../endomorphism.md). Pairing is $\langle-,-\rangle$, and for $x:D\times D\to D$ write $x^*$ for its [currying](../../../../../currying.md). The product identities and the two inverse exponential identities give

$$
\pi\langle x,y\rangle=x,\quad\pi'\langle x,y\rangle=y,\quad\langle\pi z,\pi'z\rangle=z,
$$



$$
\varepsilon\langle x^*\pi,\pi'\rangle=x,\qquad(\varepsilon\langle y\pi,\pi'\rangle)^*=y.
$$

This is the structure of a [cartesian closed monoid](../../../../../cartesian-closed-monoid.md).

For the converse, start only from the [monoid](../../../../../monoid.md) and these identities. The first three make pairing a bijection from $M^2$ to $M$, inverse to $z\mapsto(\pi z,\pi'z)$. In particular

$$
\langle x,y\rangle z=\langle xz,yz\rangle,\qquad\langle\pi,\pi'\rangle=1_M,
$$

as follows by applying both projections and using uniqueness. Define $U(y)=\varepsilon\langle y\pi,\pi'\rangle$. The last two identities say that $U$ and $(-)^*$ are inverse bijections. These facts also derive, rather than assume, the naturality law

$$
\boxed{(x\langle z\pi,\pi'\rangle)^*=x^*z.}
$$

Indeed $U(x^*z)=\varepsilon\langle x^*z\pi,\pi'\rangle=U(x^*)\langle z\pi,\pi'\rangle=x\langle z\pi,\pi'\rangle$; applying the inverse bijection proves the law.

Put $e=(\pi')^*$. The law applied to $x=\pi'$ gives, for every $z\in M$,

$$
ez=(\pi'\langle z\pi,\pi'\rangle)^*=(\pi')^*=e.
$$

Taking $z=e$ proves **$e^2=e$**. This stronger absorption identity is what makes the split object terminal.

Assume first that $M$ is nontrivial; the degenerate case is handled below. Construct the required category using the two idempotents $d=1_M$ and $e$, as a two-object part of the [Karoubi envelope](../../../../../karoubi-envelope.md). Call their objects $D$ and $1$. A morphism from the object with idempotent $a$ to the object with idempotent $b$ is an element $f\in M$ satisfying $bfa=f$. Composition is [monoid](../../../../../monoid.md) multiplication, and the identity on each object is its idempotent. These laws are well-defined and associative. Its hom-sets are concretely

$$
\operatorname{Hom}(D,D)=M,\quad\operatorname{Hom}(D,1)=\{e\},\quad\operatorname{Hom}(1,1)=\{e\},\quad\operatorname{Hom}(1,D)=\{f:fe=f\}.
$$

For example, $ef=e$ for every $f$, so the condition for $D\to1$ forces $f=e$. Thus $1$ is terminal, and the original [monoid](../../../../../monoid.md) appears unchanged at $D$.

Set $D\times D=D$ with projections $\pi,\pi'$ and the given pairing. The product property works for arrows from either object: for global arrows $x,y$ satisfying $xe=x$, $ye=y$, pairing also satisfies $\langle x,y\rangle e=\langle x,y\rangle$. The original projection identities give existence and uniqueness. Products with $1$ are the other object, with its identity and the unique terminal arrow as projections; $1\times1=1$.

For the exponential set $D^D=D$ with evaluation $\varepsilon$. For a parameter object $D$, the given $(-)^*$ and $U$ already establish the universal property. We must additionally verify it for parameter object $1$. An arrow $f:1\times D=D\to D$ is an arbitrary element of $M$. Define its transpose by

$$
\kappa(f)=(f\pi')^*.
$$

Naturality gives $\kappa(f)z=\kappa(f)$ for every $z$, because $f\pi'\langle z\pi,\pi'\rangle=f\pi'$. In particular $\kappa(f)e=\kappa(f)$, so it really is an arrow $1\to D$.

Its uncurrying is $\varepsilon\langle\kappa(f),1_M\rangle=f$. To see this, start from $U(\kappa(f))=f\pi'$ and compose with $\langle e,1_M\rangle$. Pairing naturality, $\pi'\langle e,1_M\rangle=1_M$, and the absorption property of $\kappa(f)$ give precisely the claimed equality. Conversely, if $g:1\to D$ satisfies $ge=g$, then $gz=gez=ge=g$ for every $z$. Therefore

$$
\kappa(\varepsilon\langle g,1_M\rangle)=(\varepsilon\langle g\pi',\pi'\rangle)^*=(\varepsilon\langle g\pi,\pi'\rangle)^*=g.
$$

Thus transpose and uncurrying are inverse for the terminal parameter object too. This verifies the full exponential property, rather than only its [endomorphism](../../../../../endomorphism.md) instance.

The remaining exponentials are $D^1=D$, $1^D=1$, and $1^1=1$, by the unit product law and terminality. Hence **the constructed two-object category is cartesian closed and $\operatorname{End}(D)=M$**.

For nontrivial $M$, the constructed $D$ is nonterminal because it has more than one [endomorphism](../../../../../endomorphism.md), and $e\ne1_M$ by the absorption identity. This is the case corresponding to the forward non-preorder hypothesis.

If $M$ has one element, all the algebraic identities still hold, but splitting $e=1_M$ alone would make the original object terminal. To satisfy the literal converse's requirement of a nonterminal object, handle this case separately: take the two-object poset category $D<1$. Products are meets, $D^D=1$, $1^D=1$, $D^1=D$, and $1^1=1$, which verify the exponential adjunction on this two-element order. It is cartesian closed, $D$ is nonterminal, and its one-element [endomorphism](../../../../../endomorphism.md) [monoid](../../../../../monoid.md) is $M$. It is a preorder, so it does not recover the forward non-preorder setting or the self-exponential equality. Thus the converse's stated [endomorphism](../../../../../endomorphism.md) realization works also in the degenerate case, while the stronger non-preorder reconstruction uses nontrivial $M$.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 87](../../paper-87-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
