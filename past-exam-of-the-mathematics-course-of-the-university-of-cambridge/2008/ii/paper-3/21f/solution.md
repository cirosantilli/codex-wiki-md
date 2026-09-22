<h1 id="21f/solution">Solution</h1>

↑ **Parent:** [21F](../21f.md)

The real [Stone-Weierstrass theorem](../../../../../stone-weierstrass-theorem.md) states that a subalgebra $A\subseteq C(K,\mathbb R)$ on a compact Hausdorff space $K$, containing constants and separating points, is dense in the [uniform norm](../../../../../supremum-norm.md). Let $B$ be its uniform closure. Polynomial approximation to $|t|$ on a bounded interval shows that $f\in B$ implies $|f|\in B$. Therefore $B$ is closed under pointwise maximum and minimum, since $\max(f,g)=(f+g+|f-g|)/2$ and $\min(f,g)=(f+g-|f-g|)/2$.

Fix $h\in C(K)$ and $\epsilon>0$. Point separation and constants supply, for each pair $x,y$, a function $f_{xy}\in A$ agreeing with $h$ at both points. For fixed $x$, finitely many open sets where $f_{xy}>h-\epsilon$ cover $K$; their corresponding maximum $g_x\in B$ satisfies $g_x>h-\epsilon$ everywhere and $g_x(x)=h(x)$. The open sets where $g_x<h+\epsilon$, as $x$ varies, cover $K$. Choose finitely many and take their minimum $g\in B$. Then $h-\epsilon<g<h+\epsilon$ throughout $K$. Approximating $g$ by members of $A$ proves the theorem.

Now let $F$ be the [uniform closure](../../../../../uniform-closure-of-a-function-algebra.md) of integer-coefficient polynomials on $[a,b]$. It is a closed ring. Since $q=\max_{[a,b]}|1-2x|<1$, the integer-coefficient polynomials $\sum_{j=0}^Nx(1-2x)^j$ converge uniformly to $1/2$, with error at most $bq^{N+1}/(1-q)$. Thus $1/2\in F$. Ring operations give every dyadic rational constant, and closure gives every real constant. Since $x\in F$, all real polynomials lie in $F$. The [Stone-Weierstrass theorem](../../../../../stone-weierstrass-theorem.md) now yields $\boxed{F=C([a,b])}$, as in [integer polynomial approximation away from zero and one](../../../../../integer-polynomial-approximation-away-from-zero-and-one.md).

On $[0,b]$ the answer is **no**. The constant function $1/2$ cannot be uniformly approximated by integer-coefficient polynomials: at zero every such polynomial has an integer value and therefore error at least $1/2$.

## ↑ Ancestors (10)

1. [21F](../21f.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
