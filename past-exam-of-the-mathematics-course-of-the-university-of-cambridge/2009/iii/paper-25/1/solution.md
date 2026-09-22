<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The arrow in the original PDF permits partial functions. A [partial computable function](../../../../../computable-function.md) $\mathbb N^k\rightharpoonup\mathbb N$ is computed by a finite program which halts with the specified value on every input in its domain and diverges on inputs outside the domain. A [total computable function](../../../../../total-computable-function.md) is the special case with full domain. Coding finite tuples by a [primitive recursive pairing function](../../../../../primitive-recursive-pairing-function.md) identifies the different finite arities effectively, without identifying total and partial computability.

One precise machine model is a [Turing machine](../../../../../turing-machine.md). Its finite transition rules and configurations admit effective numerical coding. Bounded simulation is [primitive recursive](../../../../../primitive-recursive-function.md), and unbounded execution gives the partial result. Equivalently, start from zero, successor and projections and close under composition, [primitive recursion](../../../../../primitive-recursion.md) and [unbounded minimization](../../../../../mu-operator.md). The [Kleene normal form theorem](../../../../../kleene-normal-form-theorem.md) makes the equivalence concrete:

$$
\varphi_e(\mathbf x)\simeq U\bigl(\mu s\ T(e,\mathbf x,s)\bigr),
$$

where $T$ is a [primitive recursive](../../../../../primitive-recursive-function.md) predicate checking a coded halting computation and $U$ reads its output. If no computation exists, the minimum and hence the value are undefined. Checking a finite history is effective because every consecutive configuration must obey one of the finitely many transition rules.

The [universal partial computable function](../../../../../universal-partial-computable-function.md) evaluates the program indexed by $e$ on an input. The [S-m-n theorem](../../../../../smn-theorem.md) says that fixing finitely many input parameters can be done by a total computable operation on program [Gödel numbers](../../../../../godel-number.md): a new program stores those parameters and calls the original universal evaluator. These facts explain both universal simulation and uniform reductions. A set is [computably enumerable](../../../../../recursively-enumerable-set.md) when it is the domain of a [partial computable function](../../../../../computable-function.md), equivalently the range of an effective enumeration. It is [recursive](../../../../../computable-set.md) when its characteristic function is total computable. A set is recursive precisely when it and its complement are [computably enumerable](../../../../../recursively-enumerable-set.md): dovetail the two enumerations to decide each input.

The diagonal [halting problem](../../../../../halting-problem.md) $K=\{e:\varphi_e(e)\downarrow\}$ is [computably enumerable](../../../../../recursively-enumerable-set.md) but not recursive. A total decider would yield a program which, on $e$, diverges if the decider says $e\in K$ and halts otherwise. Applying this program to its own index gives a contradiction. There is likewise no total computable universal listing of all [total computable functions](../../../../../total-computable-function.md): the diagonal function $n\mapsto U(n,n)+1$ would be total and absent from the listing.

Here is a full proof of the [Rice theorem](../../../../../rice-s-theorem.md). Let $\mathcal P$ be a nonempty proper class of [partial computable functions](../../../../../computable-function.md) whose property depends only on the function, not its program. First suppose the everywhere-undefined function $\bot$ is not in $\mathcal P$, and choose a program for a function $g\in\mathcal P$. Given an index $e$, construct uniformly a program which on $x$ first waits for $\varphi_e(e)$ to halt and, only then, simulates $g(x)$. The [S-m-n theorem](../../../../../smn-theorem.md) gives a total computable index map $h$. If $e\notin K$, then $\varphi_{h(e)}=\bot$; if $e\in K$, then $\varphi_{h(e)}=g$. Thus

$$
e\in K\quad\Longleftrightarrow\quad\varphi_{h(e)}\in\mathcal P.
$$

A decision procedure for the property would decide $K$, impossible. If $\bot\in\mathcal P$, apply the same argument to its nontrivial complement. **Every nontrivial extensional property of [partial computable functions](../../../../../computable-function.md) has an undecidable [index set](../../../../../index-set.md).** Totality, having finite domain, and taking a particular value somewhere are examples. A syntactic property such as program length is not covered; nor does the theorem say that no individual program's behaviour can be established.

Self-reference can also be made effective. For a total computable index transformation $f$, let $d(x)$ be an index for the program which first computes $\varphi_x(x)$ and then runs the program with that resulting index on its own input. The [S-m-n theorem](../../../../../smn-theorem.md) makes $d$ total computable. Choose an index $e$ for the total function $x\mapsto f(d(x))$, and put $n=d(e)$. Then

$$
\varphi_n=\varphi_{\varphi_e(e)}=\varphi_{f(d(e))}=\varphi_{f(n)}.
$$

This proves the [recursion theorem](../../../../../kleene-s-recursion-theorem.md): every effective transformation of programs has a fixed point at the level of the function computed, though not necessarily at the level of its numerical code.

Finally, consider the [Jockusch triple coloring computing the halting set](../../../../../jockusch-triple-coloring-computing-the-halting-set.md). Fix computable finite approximations $K_0\subseteq K_1\subseteq\cdots$ with union $K$. For $x<y<z$, define

$$
c(\{x,y,z\})=\begin{cases}0,&K_y\cap\{0,\ldots,x-1\}=K_z\cap\{0,\ldots,x-1\},\\1,&\text{otherwise}.\end{cases}
$$

This is a total recursive two-coloring because both stages are finite computations. Suppose $H$ is infinite and homogeneous. Its color cannot be one: fix $x\in H$, wait until every enumeration below $x$ has stabilized, and choose later $y<z$ from $H$ beyond that stage. Their color is zero.

If $H$ has color zero, it computes $K$. On input $n$, use $H$ to find $x>n$ and $y>x$ in $H$. For arbitrarily large $z\in H$ with $z>y$, homogeneity gives $K_y\cap x=K_z\cap x$. Taking stages sufficiently large to reach the final finite approximation gives $K_y\cap x=K\cap x$. Consequently membership of $n$ in $K$ is decided by the finite stage $K_y$. A recursive $H$ would therefore make $K$ recursive, a contradiction. **There is a recursive partition of triples with no infinite recursive [homogeneous set](../../../../../homogeneous-set-for-a-colouring.md).** This is the nontrivial finite-color meaning of the partition of an infinite domain; if “infinite partition” meant infinitely many colors, the coloring by the least member would already give a trivial example. [Ramsey's theorem](../../../../../ramsey-s-theorem.md) still guarantees infinite [homogeneous sets](../../../../../homogeneous-set-for-a-colouring.md) for the displayed two-coloring, but every such set is computationally nontrivial.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 25](../../paper-25-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
