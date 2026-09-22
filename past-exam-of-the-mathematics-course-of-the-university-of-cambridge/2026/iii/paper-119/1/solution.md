<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

A category is [well-powered](../../../../../well-powered-category.md) when the isomorphism classes of monomorphisms into each object form a set. For $P\in[\mathcal C,\mathbf{Set}]$, every subobject is represented by a subfunctor $S$ with $S(A)\subseteq P(A)$. Since $\mathcal C$ is small, all choices lie in the set $\prod_A\mathcal P(P(A))$, and naturality merely cuts out a subset. Thus the [functor category](../../../../../functor-category.md) is well-powered. Quotients are similarly represented by compatible equivalence relations on the sets $P(A)$, so they form a subset of $\prod_A\mathcal P(P(A)^2)$; hence it is well-copowered.

A cocone under the identity diagram consists of maps $c_A:A\to L$ satisfying $c_Bf=c_A$ for every $f:A\to B$. A [terminal object](../../../../../terminal-object.md) supplies the unique such cocone and has the required universal property. Conversely, if $(L,c_A)$ is a [colimit](../../../../../colimit.md) of the identity, both $1_L$ and $c_L$ mediate its cocone to itself, so uniqueness gives $c_L=1_L$. For any $f:A\to L$, cocone compatibility gives $f=c_Lf=c_A$; thus there is exactly one arrow $A\to L$, and $L$ is terminal.

For $A\in\mathcal C$, let $\Omega(A)$ be the set of isomorphism classes of quotients of the representable $\mathcal C(A,-)$. This is a set by well-copoweredness. A map $u:A\to B$ sends a quotient of $\mathcal C(A,-)$ to the image quotient of the composite $\mathcal C(B,-)\to\mathcal C(A,-)$, making $\Omega$ a functor. For any functor $P$ and $x\in P(A)$, Yoneda gives $\mathcal C(A,-)\to P$; factor it as an epimorphism followed by a monomorphism and send $x$ to the resulting quotient class. These maps $P\to\Omega$ agree along every monomorphism. Conversely, a cone with apex $Q$ assigns to a quotient $q:\mathcal C(A,-)\twoheadrightarrow R$ the element obtained by applying its leg at $R$ to $q_A(1_A)$. Yoneda and epi-mono factorization show that this is well-defined and is the unique map $\Omega\to Q$. Therefore $\Omega$ is a [local state classifier](../../../../../local-state-classifier.md).

An object of $[\mathbb Z,\mathbf{Set}_f]$ is a finite set with a permutation. For each $n>0$, let $A_n=\mathbb Z/n$ with trivial action and map a finite $\mathbb Z$-set $P$ to $A_n$ by sending every point to the length of its orbit modulo $n$. Equivariant injections preserve orbit lengths, so these maps form a cocone under the monomorphism subcategory; varying cyclic orbits shows that its legs are collectively surjective. If a local state classifier $L$ existed, its universal map onto every $A_n$ would be surjective because the universal legs are jointly epic. This would force the finite set $L$ to have at least $n$ elements for every $n$, a contradiction.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 119](../../paper-119-split.md)
3. [Iii](../../split.md)
4. [2026](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
