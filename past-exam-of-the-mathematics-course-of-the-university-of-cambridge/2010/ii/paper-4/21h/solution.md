<h1 id="21h/solution">Solution</h1>

↑ **Parent:** [21H](../21h.md)

The [Snake lemma](../../../../../snake-lemma.md) applies to a commutative diagram of modules with exact rows $0\to A'\xrightarrow{i'}B'\xrightarrow{j'}C'\to0$ and $0\to A\xrightarrow{i}B\xrightarrow{j}C\to0$, and vertical maps $f,g,h$. It supplies the exact sequence

$$
0\to\ker f\to\ker g\to\ker h
\xrightarrow{\delta}\operatorname{coker}f
\to\operatorname{coker}g\to\operatorname{coker}h\to0.
$$

For $c'\in\ker h$, choose $b'$ with $j'b'=c'$. Commutativity gives $jgb'=0$, so $gb'=i(a)$ for a unique $a\in A$. Define $\delta(c')=[a]$ modulo $f(A')$. Changing $b'$ by $i'(a')$ changes $a$ by $f(a')$, proving well-definedness. This construction is additive. Exactness follows by the same lift-and-chase: $\delta(c')=0$ exactly when the lift can be adjusted into $\ker g$; a class in $\operatorname{coker}f$ maps to zero in $\operatorname{coker}g$ exactly when it is obtained from such a lift. The remaining kernel and cokernel positions follow directly from row exactness.

For an open cover $X=U\cup V$, use the [short exact sequence](../../../../../short-exact-sequence.md) of singular chain complexes

$$
0\to C_*(U\cap V)\xrightarrow{a\mapsto(a,-a)}
C_*(U)\oplus C_*(V)\xrightarrow{(a,b)\mapsto a+b}
C_*^{\{U,V\}}(X)\to0,
$$

where the last complex consists of chains whose simplices lie in one member of the cover. This is exact because a simplex present in both summands lies in their intersection. Barycentric subdivision and its chain homotopy to the identity show that this small-chain inclusion induces an isomorphism on [homology](../../../../../homology-split.md): [compactness](../../../../../compact-space.md) of each simplex and a Lebesgue-number argument place sufficiently subdivided simplices inside the cover.

Applying the [Snake lemma](../../../../../snake-lemma.md) to a [short exact sequence](../../../../../short-exact-sequence.md) of chain complexes gives the connecting homomorphism $[c]\mapsto[da]$: lift a quotient cycle $c$ to the middle complex, take its differential, and identify that differential with an element of the subcomplex. Its independence of the lift and representative follows by the same chase. Repeating this degree by degree, or chasing the cycles and boundaries directly, gives

$$
\boxed{\cdots\to H_n(U\cap V)\to H_n(U)\oplus H_n(V)
\to H_n(X)\xrightarrow{\delta}H_{n-1}(U\cap V)\to\cdots.}
$$

This is the [Mayer–Vietoris sequence](../../../../../mayer-vietoris-sequence.md). Specifically, split a small cycle as $a+b$; then $da=-db$ lies in the intersection, and $\delta[a+b]=[da]$ with the sign convention above.

For the final truncation, use homological grading $d:C_j\to C_{j-1}$. The span $B$ in degrees below $n$ is a subcomplex. The span called $A$ in degrees at least $n$ need not be a subcomplex with the inherited differential: $dC_n$ may lie in $C_{n-1}$. Give $A$ the quotient differential, with $d:A_n\to A_{n-1}=0$ zero and all higher differentials inherited. Then

$$
\boxed{0\to B\to C\to A\to0}
$$

is a [short exact sequence](../../../../../short-exact-sequence.md) of chain complexes. Its only potentially nonzero connecting map is

$$
\boxed{\delta:H_n(A)\to H_{n-1}(B),\qquad [a]\mapsto[da].}
$$

Indeed $H_n(A)=C_n/dC_{n+1}$; $da$ is a cycle in $B$, and changing $a$ by $db$ changes $da$ by zero. In other degrees either the source or the relevant target of the connecting map vanishes.

## ↑ Ancestors (10)

1. [21H](../21h.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
