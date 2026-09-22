<h1 id="b/6/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

There are two ways for a [set](../../../../../set-split.md) to fail to be the [power set](../../../../../power-set.md) of $y$: it may contain an object which is not a [subset](../../../../../subset.md) of $y$, or omit a [subset](../../../../../subset.md) of $y$. A single existential [logical formula](../../../../../logical-formula.md) expressing these alternatives is

$$
\boxed{\phi(x,y)\equiv\exists z\Bigl[
\bigl(z\in x\wedge(\exists u\in z)\,u\notin y\bigr)
\vee\bigl(z\notin x\wedge(\forall u\in z)\,u\in y\bigr)\Bigr].}
$$

Its matrix is bounded, so this is $\Sigma_1$. Its negation is precisely the first-order power-set specification

$$
\forall z\bigl(z\in x\ \longleftrightarrow\ (\forall u\in z)\,u\in y\bigr).
$$

We prove the absoluteness fact needed to exclude a logically equivalent $\Sigma_1$ [logical formula](../../../../../logical-formula.md). If $M\subseteq N$ are [transitive sets](../../../../../transitive-set.md) and all parameters lie in $M$, bounded [logical formulas](../../../../../logical-formula.md) have the same truth value in $\langle M,\in\rangle$ and $\langle N,\in\rangle$. Atomic equality and membership agree because both structures use actual membership. Boolean operations preserve agreement. In a bounded [quantifier](../../../../../quantifier.md) over $v\in M$, transitivity ensures that every element of $v$ already lies in $M$, so the two structures quantify over exactly the same elements of $v$. Induction on [logical formulas](../../../../../logical-formula.md) proves the claim. It follows that $\Sigma_1$ [logical formulas](../../../../../logical-formula.md) are upward absolute: witnesses in $M$ remain available in $N$, and their bounded matrix retains its truth value.

Now use a finite counterexample, so no existence of a transitive model of [ZF](../../../../../zermelo-fraenkel-set-theory.md) is assumed. Let $M=4=\{0,1,2,3\}$, the [Finite von Neumann ordinal](../../../../../finite-von-neumann-ordinal.md), and let $N=V_4$. These are [transitive sets](../../../../../transitive-set.md) with $M\subseteq N$. [Set](../../../../../set-split.md) $y=2$ and $x=3$, both elements of $M$. Inside $M$, the [subsets](../../../../../subset.md) of $2$ which are available as elements of the domain are exactly $0,1,2$; the remaining domain element $3$ is not a [subset](../../../../../subset.md) of $2$. Thus $M$ satisfies the displayed power-set specification with $x=3$.

Inside $N$, however, the [set](../../../../../set-split.md) $\{1\}$ is also present and is a [subset](../../../../../subset.md) of $2$, while $\{1\}\notin3$. Thus the same specification is false in $N$. If $\neg\phi$ were logically equivalent to a $\Sigma_1$ [logical formula](../../../../../logical-formula.md), its truth in $M$ would transfer upward to $N$, a contradiction. Therefore

$$
\boxed{\neg\phi\text{ is not logically equivalent to any }\Sigma_1\text{ formula}.}
$$

This proves the requested unrestricted logical non-equivalence. The finite structures are not being claimed to satisfy all of [ZF](../../../../../zermelo-fraenkel-set-theory.md); logical equivalence must hold in them as well as in any models of a stronger theory.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [6](../../6.md)
3. [B](../../../b.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the analytic topology and axiomatic set theory course of the University of Oxford](../../../../split.md)
6. [Analytic topology and axiomatic set theory course of the University of Oxford](../../../../../analytic-topology-and-axiomatic-set-theory-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
