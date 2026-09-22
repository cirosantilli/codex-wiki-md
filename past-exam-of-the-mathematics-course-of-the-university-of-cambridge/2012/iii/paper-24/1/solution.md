<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Take $\mathbb N=\{0,1,2,\ldots\}$ and fix a standard effective enumeration $(\varphi_e)$ of the unary [partial computable functions](../../../../../computable-function.md) by program texts. Write

$$
K=\{e:\varphi_e(e)\downarrow\},\qquad K_s=\{e<s:\varphi_e(e)\text{ halts within }s\text{ steps}\}.
$$

The [diagonal halting set](../../../../../diagonal-halting-set.md) $K$ is not a [computable set](../../../../../computable-set.md): a supposed decision procedure would give a program that halts on input $e$ exactly when $e\notin K$, contradicting its own index. Each $K_s$ is finite and uniformly decidable by [bounded simulation of a computation](../../../../../bounded-simulation-of-a-computation.md), and $K_s\subseteq K_{s+1}$ with union $K$.

For $a<b<c$, define the [computable colouring](../../../../../computable-colouring.md)

$$
\boxed{\chi(\{a,b,c\})=\begin{cases}0&K_b\cap[0,a)=K_c\cap[0,a),\\1&K_b\cap[0,a)\ne K_c\cap[0,a).\end{cases}}
$$

This is a two-part decidable [set partition](../../../../../set-partition.md) on three-element subsets: sort the three inputs and perform the two finite simulations. Here $[0,a)=\{0,\ldots,a-1\}$. The [halting-stage colouring of triples](../../../../../halting-stage-colouring-of-triples.md) cannot have an infinite [homogeneous set for a colouring](../../../../../homogeneous-set-for-a-colouring.md) of colour $1$. Indeed, fix its least element $a$. The finitely many bits of $K_s\cap[0,a)$ eventually stabilize. Choose two later elements $b<c$ of the putative [homogeneous set for a colouring](../../../../../homogeneous-set-for-a-colouring.md) beyond that stabilization stage; the corresponding triple has colour $0$.

Now suppose $H$ is an infinite [homogeneous set for a colouring](../../../../../homogeneous-set-for-a-colouring.md) of colour $0$. Its membership oracle computes $K$: to decide whether $n\in K$, search for $a,b\in H$ with $n<a<b$, and return whether $n\in K_b$. For every $c\in H$ above $b$, homogeneity gives $K_c\cap[0,a)=K_b\cap[0,a)$. Since $H$ is unbounded, taking such $c$ arbitrarily large proves that this common finite set is $K\cap[0,a)$. Thus

$$
K\leq_T H.
$$

If $H$ were a [computable set](../../../../../computable-set.md), the displayed [Turing reduction](../../../../../turing-reduction.md) would decide $K$, a contradiction. **The displayed decidable two-colouring has no infinite decidable homogeneous set.**

For the second construction, let $2^{<\omega}$ be the finite [binary strings](../../../../../binary-string.md), with coordinates starting at $0$, and define the [computable binary tree](../../../../../computable-binary-tree.md)

$$
\boxed{T=\{\sigma\in2^{<\omega}:\ \forall e<|\sigma|,\ \forall v\in\{0,1\},\ [\varphi_e(e)\text{ halts within }|\sigma|\text{ steps with output }v\ \Longrightarrow\ \sigma(e)=1-v]\}.}
$$

Membership is decided by finitely many tests using [bounded simulation of a computation](../../../../../bounded-simulation-of-a-computation.md). It is a [binary tree of finite strings](../../../../../binary-tree-of-finite-strings.md): if a string satisfies the tests, each prefix satisfies its shorter and fewer tests. The [infinite paths through a binary tree](../../../../../infinite-path-through-a-binary-tree.md) are exactly

$$
[T]=\{f\in2^\omega:\ \varphi_e(e)\downarrow\in\{0,1\}\Longrightarrow f(e)\ne\varphi_e(e)\text{ for every }e\}.
$$

This set is nonempty: at a coordinate whose diagonal computation halts with a binary value choose the other value, and choose either bit elsewhere. This is an existence argument, not a proposed computable decision procedure for convergence. No member is a [total computable function](../../../../../total-computable-function.md). If $f=\varphi_d$ were a total binary-valued function, the condition at $d$ would say $f(d)\ne\varphi_d(d)=f(d)$. Thus each member is a [binary diagonally noncomputable function](../../../../../binary-diagonally-noncomputable-function.md).

Moreover, $[T]$ has no isolated point. There are arbitrarily large indices of programs that never halt: for example, distinct program texts with successively more unused instructions followed by an infinite loop provide infinitely many such indices in the usual syntactic program coding. At every one of these coordinates the bit is unrestricted. Given any $f\in[T]$ and any prefix length $n$, change its bit at one such index $e\geq n$ and leave all other bits unchanged. The resulting different path still belongs to $[T]$ and has the same length-$n$ prefix. Since a path space is closed in [Cantor space](../../../../../cantor-space.md), **$T$ is decidable, $[T]$ is nonempty and perfect, and no infinite path is computable.**

There is a definition issue with the adjective “perfect”. The preceding conclusion uses [perfect path space](../../../../../perfect-path-space.md), allowing finite dead ends in the decidable presentation. If “perfect tree” instead requires every node to have two incompatible extensions in the tree, the requested combination is impossible. Such a nonempty tree has no terminal nodes. Starting at the empty string, test the two immediate successors and choose the first that belongs to the tree; one always exists. This constructs a [total computable function](../../../../../total-computable-function.md) whose successive prefixes remain in the tree. Thus [computable pruned binary trees have computable paths](../../../../../computable-pruned-binary-trees-have-computable-paths.md). Our $T$ necessarily has dead ends; its subtree consisting only of prefixes of infinite paths is perfect in the pruned sense but is not decidable. The construction therefore supplies the intended perfect closed path space and also resolves the stronger, inconsistent interpretation.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 24](../../paper-24-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
