<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

A [partial computable function](../../../../../computable-function.md) is the [function](../../../../../function-split.md) computed by a finite program, with an undefined value when its computation never terminates. A [total computable function](../../../../../total-computable-function.md) terminates on every input. Fix an effective enumeration $(\varphi_e)_{e\in\omega}$ of the [partial computable functions](../../../../../computable-function.md), with a [universal partial computable function](../../../../../universal-partial-computable-function.md) $U(e,x)=\varphi_e(x)$. Composition, [primitive recursion](../../../../../primitive-recursion.md) and [unbounded minimization](../../../../../mu-operator.md) give a machine-independent description of this class. [Unbounded minimization](../../../../../mu-operator.md) is allowed to diverge. The [S-m-n theorem](../../../../../smn-theorem.md) permits parameters in a program to be specialized effectively: an algorithm described uniformly in $e$ has an index obtained computably from $e$.

The [halting set](../../../../../halting-set.md) $K=\{e:\varphi_e(e)\text{ halts}\}$ is [computably enumerable](../../../../../recursively-enumerable-set.md): simulate all computations in parallel and enumerate each index whose diagonal computation terminates. It is not a [computable set](../../../../../computable-set.md). Otherwise the program which terminates exactly when the proposed decision procedure says its own diagonal computation does not terminate gives a contradiction. There is also no effective enumeration consisting exactly of all [total computable functions](../../../../../total-computable-function.md): from such an enumeration $(f_n)$ the [total computable function](../../../../../total-computable-function.md) $g(n)=f_n(n)+1$ differs from every listed [function](../../../../../function-split.md). Thus the effective enumeration of partial programs cannot be replaced by a decidable catalogue of total ones.

For the [Rice theorem](../../../../../rice-s-theorem.md), let $C$ be a nontrivial property of [partial computable functions](../../../../../computable-function.md), depending on the computed [function](../../../../../function-split.md) rather than the program text. First suppose the nowhere-defined [function](../../../../../function-split.md) is not in $C$, and choose a program computing some $g\in C$. Uniformly in $e$, define a program which, on input $x$, first waits for $\varphi_e(e)$ to terminate and then runs the computation of $g(x)$. The [S-m-n theorem](../../../../../smn-theorem.md) gives a computable index map $e\mapsto p(e)$, and

$$
\varphi_{p(e)}=\begin{cases}g,&e\in K,\\\text{nowhere-defined function},&e\notin K.\end{cases}
$$

Consequently a decision procedure for membership in $C$ would decide the [halting set](../../../../../halting-set.md). If the nowhere-defined [function](../../../../../function-split.md) belongs to $C$, apply the same argument to its complement. **Every nontrivial extensional property of [partial computable functions](../../../../../computable-function.md) has an undecidable index [set](../../../../../set-split.md).** Syntactic properties of program descriptions are outside this assertion, and the theorem concerns unrestricted program indices, not merely an assumed list of terminating programs.

Here is an explicit [Jockusch triple coloring computing the halting set](../../../../../jockusch-triple-coloring-computing-the-halting-set.md). Choose computable increasing finite stages $K_s$ with [union](../../../../../set-union.md) $K$. For $x<y<z$, put

$$
c(\{x,y,z\})=\begin{cases}0,&K_y\cap x=K_z\cap x,\\1,&K_y\cap x\ne K_z\cap x.\end{cases}
$$

This is a [computable colouring](../../../../../computable-colouring.md). An infinite [monochromatic](../../../../../monochromatic-set.md) [set](../../../../../set-split.md) cannot have color $1$: fix its first element $x$ and choose two later elements beyond the stage at which $K_s\cap x$ stabilizes. Their triple has color $0$.

Suppose $H$ is infinite and homogeneous of color $0$. To decide whether $n\in K$ using $H$, find $x\in H$ with $x>n$, and then $y\in H$ with $y>x$. For every $z\in H$ above $y$, homogeneity gives $K_y\cap x=K_z\cap x$. Such $z$ are unbounded, so $K_y\cap x=K\cap x$. Testing $n\in K_y$ therefore decides $n\in K$. Hence every [homogeneous set](../../../../../homogeneous-set-for-a-colouring.md) computes the [halting set](../../../../../halting-set.md), and **there is no infinite recursive [monochromatic set](../../../../../monochromatic-set.md).** The [infinity](../../../../../infinity.md) qualification is essential: finite [homogeneous sets](../../../../../homogeneous-set-for-a-colouring.md) are recursive.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 25](../../paper-25-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
