<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Enumerate the [vertices](../../../../../vertex-graph-theory.md) as $V=\{1,\ldots,n\}$ and introduce a [Boolean variable](../../../../../boolean-variable.md) $X_{u,v}$ for each ordered pair of [vertices](../../../../../vertex-graph-theory.md). Its intended meaning is that a proposed [graph automorphism](../../../../../graph-automorphism.md) sends $u$ to $v$. Build four groups of [Boolean clauses](../../../../../clause-of-a-boolean-formula.md).

First require exactly one image for each [vertex](../../../../../vertex-graph-theory.md):

$$
A=\bigwedge_{u\in V}\left[
\left(\bigvee_{v\in V}X_{u,v}\right)
\land\bigwedge_{v<w}(\neg X_{u,v}\lor\neg X_{u,w})\right].
$$

Next require that distinct [vertices](../../../../../vertex-graph-theory.md) have distinct images:

$$
B=\bigwedge_{v\in V}\bigwedge_{u<w}(\neg X_{u,v}\lor\neg X_{w,v}).
$$

Together $A$ and $B$ specify an injective [function](../../../../../function-split.md) $f:V\to V$. Since $V$ is finite, this [function](../../../../../function-split.md) is a [bijection](../../../../../bijection.md); a separate surjectivity condition is unnecessary.

Write $e(u,w)=1$ when $(u,w)\in E$ and $e(u,w)=0$ otherwise. Prohibit every pair of images that would change adjacency:

$$
C=\bigwedge_{\substack{u,w,v,z\in V\\ e(u,w)\ne e(v,z)}}
(\neg X_{u,v}\lor\neg X_{w,z}).
$$

Checking both possible mismatches preserves both edges and nonedges. Finally require a moved [vertex](../../../../../vertex-graph-theory.md):

$$
D=\bigvee_{u\in V}\neg X_{u,u}.
$$

The desired [propositional formula](../../../../../propositional-formula.md) is

$$
\boxed{\varphi_G=A\land B\land C\land D.}
$$

If a [Boolean valuation](../../../../../boolean-valuation.md) satisfies $\varphi_G$, $A$ selects a unique image for every [vertex](../../../../../vertex-graph-theory.md), $B$ makes the resulting [function](../../../../../function-split.md) a [bijection](../../../../../bijection.md), $C$ preserves adjacency in both directions, and $D$ makes this [graph automorphism](../../../../../graph-automorphism.md) different from the [identity function](../../../../../identity-function.md). Conversely, given such a [graph automorphism](../../../../../graph-automorphism.md) $f$, set $X_{u,v}$ true exactly when $v=f(u)$. Each of $A,B,C,D$ is then satisfied.

There are $n^2$ [Boolean variables](../../../../../boolean-variable.md), $O(n^3)$ image and injectivity [Boolean clauses](../../../../../clause-of-a-boolean-formula.md), and at most $n^4$ adjacency [Boolean clauses](../../../../../clause-of-a-boolean-formula.md). With the [graph](../../../../../graph-split.md) stored by its [adjacency matrix](../../../../../adjacency-matrix.md), testing a mismatch takes constant time. Thus the construction has [polynomial time](../../../../../polynomial-time.md) and output length $O(n^4\log(n+1))$ with binary-indexed variable names. For $n=0$, interpret the empty [logical disjunction](../../../../../logical-disjunction.md) $D$ as false; for $n=1$, $A$ and $D$ conflict. These cases correctly have no nonidentity [graph automorphism](../../../../../graph-automorphism.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Logic and proof](../../../logic-and-proof-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
