# Paper 24

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2012/paper_24.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2012/paper_24.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)

## 1

↑ **Parent:** [Paper 24](paper-24.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Take $\mathbb N=\{0,1,2,\ldots\}$ and fix a standard effective enumeration $(\varphi_e)$ of the unary [partial computable functions](../../../foundations-of-mathematics.md#computable-function) by program texts. Write

$$
K=\{e:\varphi_e(e)\downarrow\},\qquad K_s=\{e<s:\varphi_e(e)\text{ halts within }s\text{ steps}\}.
$$

The [diagonal halting set](../../../foundations-of-mathematics.md#diagonal-halting-set) $K$ is not a [computable set](../../../foundations-of-mathematics.md#computable-set): a supposed decision procedure would give a program that halts on input $e$ exactly when $e\notin K$, contradicting its own index. Each $K_s$ is finite and uniformly decidable by [bounded simulation of a computation](../../../foundations-of-mathematics.md#bounded-simulation-of-a-computation), and $K_s\subseteq K_{s+1}$ with union $K$.

For $a<b<c$, define the [computable colouring](../../../ramsey-theory.md#computable-colouring)

$$
\boxed{\chi(\{a,b,c\})=\begin{cases}0&K_b\cap[0,a)=K_c\cap[0,a),\\1&K_b\cap[0,a)\ne K_c\cap[0,a).\end{cases}}
$$

This is a two-part decidable [set partition](../../../combinatorics.md#set-partition) on three-element subsets: sort the three inputs and perform the two finite simulations. Here $[0,a)=\{0,\ldots,a-1\}$. The [halting-stage colouring of triples](../../../ramsey-theory.md#halting-stage-colouring-of-triples) cannot have an infinite [homogeneous set for a colouring](../../../ramsey-theory.md#homogeneous-set-for-a-colouring) of colour $1$. Indeed, fix its least element $a$. The finitely many bits of $K_s\cap[0,a)$ eventually stabilize. Choose two later elements $b<c$ of the putative [homogeneous set for a colouring](../../../ramsey-theory.md#homogeneous-set-for-a-colouring) beyond that stabilization stage; the corresponding triple has colour $0$.

Now suppose $H$ is an infinite [homogeneous set for a colouring](../../../ramsey-theory.md#homogeneous-set-for-a-colouring) of colour $0$. Its membership oracle computes $K$: to decide whether $n\in K$, search for $a,b\in H$ with $n<a<b$, and return whether $n\in K_b$. For every $c\in H$ above $b$, homogeneity gives $K_c\cap[0,a)=K_b\cap[0,a)$. Since $H$ is unbounded, taking such $c$ arbitrarily large proves that this common finite set is $K\cap[0,a)$. Thus

$$
K\leq_T H.
$$

If $H$ were a [computable set](../../../foundations-of-mathematics.md#computable-set), the displayed [Turing reduction](../../../foundations-of-mathematics.md#turing-reduction) would decide $K$, a contradiction. **The displayed decidable two-colouring has no infinite decidable homogeneous set.**

For the second construction, let $2^{<\omega}$ be the finite [binary strings](../../../computer-science.md#binary-string), with coordinates starting at $0$, and define the [computable binary tree](../../../geometry-and-topology.md#computable-binary-tree)

$$
\boxed{T=\{\sigma\in2^{<\omega}:\ \forall e<|\sigma|,\ \forall v\in\{0,1\},\ [\varphi_e(e)\text{ halts within }|\sigma|\text{ steps with output }v\ \Longrightarrow\ \sigma(e)=1-v]\}.}
$$

Membership is decided by finitely many tests using [bounded simulation of a computation](../../../foundations-of-mathematics.md#bounded-simulation-of-a-computation). It is a [binary tree of finite strings](../../../geometry-and-topology.md#binary-tree-of-finite-strings): if a string satisfies the tests, each prefix satisfies its shorter and fewer tests. The [infinite paths through a binary tree](../../../geometry-and-topology.md#infinite-path-through-a-binary-tree) are exactly

$$
[T]=\{f\in2^\omega:\ \varphi_e(e)\downarrow\in\{0,1\}\Longrightarrow f(e)\ne\varphi_e(e)\text{ for every }e\}.
$$

This set is nonempty: at a coordinate whose diagonal computation halts with a binary value choose the other value, and choose either bit elsewhere. This is an existence argument, not a proposed computable decision procedure for convergence. No member is a [total computable function](../../../foundations-of-mathematics.md#total-computable-function). If $f=\varphi_d$ were a total binary-valued function, the condition at $d$ would say $f(d)\ne\varphi_d(d)=f(d)$. Thus each member is a [binary diagonally noncomputable function](../../../foundations-of-mathematics.md#binary-diagonally-noncomputable-function).

Moreover, $[T]$ has no isolated point. There are arbitrarily large indices of programs that never halt: for example, distinct program texts with successively more unused instructions followed by an infinite loop provide infinitely many such indices in the usual syntactic program coding. At every one of these coordinates the bit is unrestricted. Given any $f\in[T]$ and any prefix length $n$, change its bit at one such index $e\geq n$ and leave all other bits unchanged. The resulting different path still belongs to $[T]$ and has the same length-$n$ prefix. Since a path space is closed in [Cantor space](../../../geometry-and-topology.md#cantor-space), **$T$ is decidable, $[T]$ is nonempty and perfect, and no infinite path is computable.**

There is a definition issue with the adjective “perfect”. The preceding conclusion uses [perfect path space](../../../geometry-and-topology.md#perfect-path-space), allowing finite dead ends in the decidable presentation. If “perfect tree” instead requires every node to have two incompatible extensions in the tree, the requested combination is impossible. Such a nonempty tree has no terminal nodes. Starting at the empty string, test the two immediate successors and choose the first that belongs to the tree; one always exists. This constructs a [total computable function](../../../foundations-of-mathematics.md#total-computable-function) whose successive prefixes remain in the tree. Thus [computable pruned binary trees have computable paths](../../../geometry-and-topology.md#computable-pruned-binary-trees-have-computable-paths). Our $T$ necessarily has dead ends; its subtree consisting only of prefixes of infinite paths is perfect in the pruned sense but is not decidable. The construction therefore supplies the intended perfect closed path space and also resolves the stronger, inconsistent interpretation.

## 2

↑ **Parent:** [Paper 24](paper-24.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

A [function in intension](../../../foundations-of-mathematics.md#function-in-intension) is a finite description of a computation, such as a program or a formal construction expression. A [function in extension](../../../foundations-of-mathematics.md#function-in-extension) is the resulting input-output map, including its domain if it is partial. Different descriptions may have the same extension: the programs that return $x$ directly and that compute $x+0$ describe the same [function](../../../function.md). Finite descriptions have [Gödel numbers](../../../mathematical-logic.md#godel-number); equality of the resulting [partial computable functions](../../../foundations-of-mathematics.md#computable-function) is a separate semantic question.

The [primitive recursive functions](../../../foundations-of-mathematics.md#primitive-recursive-function) are the smallest class of numerical [functions](../../../function.md) containing the [zero functions](../../../foundations-of-mathematics.md#zero-function), the [successor function](../../../foundations-of-mathematics.md#successor-function) and all [projection functions](../../../foundations-of-mathematics.md#projection-function), and closed under [function composition in recursion theory](../../../foundations-of-mathematics.md#function-composition-in-recursion-theory) and [primitive recursion](../../../foundations-of-mathematics.md#primitive-recursion). More explicitly, from $g:\mathbb N^k\to\mathbb N$ and $h:\mathbb N^{k+2}\to\mathbb N$ the latter operation forms

$$
f(\mathbf x,0)=g(\mathbf x),\qquad f(\mathbf x,n+1)=h(\mathbf x,n,f(\mathbf x,n)).
$$

For [function composition in recursion theory](../../../foundations-of-mathematics.md#function-composition-in-recursion-theory), an $m$-ary $g$ and $k$-ary $h_1,\ldots,h_m$ give $g(h_1(\mathbf x),\ldots,h_m(\mathbf x))$. Zero functions of all allowed arities can be included, with nullary zero included if arity $0$ is part of the coding convention. Every resulting [function](../../../function.md) is total: the initial functions are total, [function composition in recursion theory](../../../foundations-of-mathematics.md#function-composition-in-recursion-theory) preserves totality, and [mathematical induction](../../../foundations-of-mathematics.md#mathematical-induction) on $n$ verifies totality of [primitive recursion](../../../foundations-of-mathematics.md#primitive-recursion). Applying [structural induction for primitive recursive functions](../../../foundations-of-mathematics.md#structural-induction-for-primitive-recursive-functions) then covers all construction expressions.

Use a fixed effective [Gödel numbering](../../../mathematical-logic.md#godel-numbering) of finite tagged construction trees with decidable decoding. A node is tagged as zero, successor, projection, composition, or recursion. The [primitive recursive syntax and arity checking](../../../foundations-of-mathematics.md#primitive-recursive-syntax-and-arity-checking) algorithm first checks that the input decodes as a finite tree, then works upwards from its leaves. A projection tag $(k,j)$ is legal exactly when $1\leq j\leq k$, with output arity $k$. A composition node declares its output arity $k$ and is legal when its outer child has arity $m$, there are exactly $m$ inner children, and each has arity $k$; its arity is $k$. The declared arity also handles the case $m=0$. A recursion node is legal when its base child has arity $k$ and its step child has arity $k+2$; its arity is $k+1$. Zero and successor tags have their declared arities. Ill-formed nodes are rejected. The process terminates because there are only finitely many nodes. Thus, for each fixed $i$,

$$
\boxed{D_i=\{p:p\text{ is a valid primitive-recursive construction of arity }i\}\text{ is decidable}.}
$$

This is a syntactic assertion about [functions in intension](../../../foundations-of-mathematics.md#function-in-intension). It does not assert that arbitrary machine indices computing [primitive recursive functions](../../../foundations-of-mathematics.md#primitive-recursive-function) form a decidable set. That extensional property is nontrivial, hence undecidable by [Rice theorem](../../../foundations-of-mathematics.md#rice-s-theorem). For an explicit reduction, given a program $e$ construct a program that, on every input, waits for $\varphi_e(e)$ to halt and then returns $0$. Its extension is a [primitive recursive function](../../../foundations-of-mathematics.md#primitive-recursive-function) if $e\in K$, and otherwise is nowhere defined and so is not a [primitive recursive function](../../../foundations-of-mathematics.md#primitive-recursive-function). A decision procedure for this latter semantic set would decide the [diagonal halting set](../../../foundations-of-mathematics.md#diagonal-halting-set).

Enumerate the decidable syntax set $D_1$ in increasing code order as $p_0,p_1,\ldots$. There are infinitely many such descriptions; iterating successor after a unary zero expression already supplies infinitely many. Let $F_p$ be the extension of a valid construction and define

$$
U(n,x)=F_{p_n}(x),\qquad \boxed{d(n)=U(n,n)+1.}
$$

To compute $U$, find $p_n$ by the syntax test and interpret its finite construction tree. Evaluate [function composition in recursion theory](../../../foundations-of-mathematics.md#function-composition-in-recursion-theory) by evaluating the children, and evaluate [primitive recursion](../../../foundations-of-mathematics.md#primitive-recursion) by the prescribed finite loop of length equal to its final input. Termination follows from the totality argument above, so $U$ and $d$ are [total computable functions](../../../foundations-of-mathematics.md#total-computable-function).

If $d$ were a unary [primitive recursive function](../../../foundations-of-mathematics.md#primitive-recursive-function), some construction $p_j$ would have extension $d$. Then the [diagonal argument](../../../foundations-of-mathematics.md#diagonal-argument) gives

$$
d(j)=F_{p_j}(j)+1=d(j)+1,
$$

which is impossible. **The displayed $d$ is total and computable but not primitive recursive.** Repetitions of extensions in the enumeration cause no problem: every possible extension is represented, which is all the [diagonal argument](../../../foundations-of-mathematics.md#diagonal-argument) needs. The same argument shows that the two-variable interpreter $U$ cannot itself be [primitive recursive](../../../foundations-of-mathematics.md#primitive-recursive-function).

## 3

↑ **Parent:** [Paper 24](paper-24.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Let $(W_e)_{e\in\mathbb N}$ enumerate all [computably enumerable sets](../../../foundations-of-mathematics.md#recursively-enumerable-set), with finite uniformly computable approximations $W_{e,s}$ increasing to $W_e$. For example, take $W_e=\operatorname{dom}\varphi_e$ and

$$
W_{e,s}=\{x<s:\varphi_e(x)\text{ halts within }s\text{ steps}\}.
$$

We construct a [simple set](../../../foundations-of-mathematics.md#simple-set) by meeting the requirements $R_e$: if $W_e$ is infinite, then $W_e\cap X\ne\varnothing$. Begin with no enumerated elements and all requirements unmarked. At stage $s$, process $e=0,1,\ldots,s$ in this order. For an unmarked $R_e$, if there is an $x\in W_{e,s}$ with $x>2e$, enumerate the least such $x$ into $X$ and mark $R_e$ permanently. All membership tests at a stage are finite, and marking requires no test for eventual infinitude. The [sparse-witness construction of a simple set](../../../foundations-of-mathematics.md#sparse-witness-construction-of-a-simple-set) therefore gives a [computably enumerable set](../../../foundations-of-mathematics.md#recursively-enumerable-set) $X$; it is [semidecidable](../../../foundations-of-mathematics.md#recursively-enumerable-set) by simulating this enumeration and halting when the input appears.

Each requirement enumerates at most one element. If an element in $[0,2n]$ is enumerated by $R_e$, then $2e<x\leq2n$, so $e<n$. At most $n$ elements of that interval can therefore enter $X$, even if some requirements choose the same element. Consequently

$$
\boxed{|[0,2n]\setminus X|\geq(2n+1)-n=n+1.}
$$

The [complement of a set](../../../set.md#complement-of-a-set) $\mathbb N\setminus X$ is infinite.

If $W_e$ is infinite, it contains some $x>2e$, and that element eventually belongs to $W_{e,s}$ at a stage with $s\geq e$. If $R_e$ has already acted, it already placed an element of $W_e$ in $X$. Otherwise it acts by this stage and does so now. Thus every infinite [semidecidable set](../../../foundations-of-mathematics.md#recursively-enumerable-set) meets $X$. Equivalently, its infinite [complement of a set](../../../set.md#complement-of-a-set) is an [immune set](../../../foundations-of-mathematics.md#immune-set). **The constructed $X$ is semidecidable, coinfinite, and meets every infinite semidecidable set.**

As a useful check on the construction, $X$ cannot be a [computable set](../../../foundations-of-mathematics.md#computable-set). If it were, its infinite [complement of a set](../../../set.md#complement-of-a-set) would also be a [computably enumerable set](../../../foundations-of-mathematics.md#recursively-enumerable-set) disjoint from $X$, contradicting the property just proved. The argument requires neither deciding which $W_e$ are infinite nor protecting a prechosen infinite list of omitted numbers; the numerical witness bound provides all the required room.

## 4

↑ **Parent:** [Paper 24](paper-24.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

For subsets $A,B\subseteq\mathbb N$, a [many-one reduction](../../../foundations-of-mathematics.md#many-one-reduction) $A\leq_mB$ is a [total computable function](../../../foundations-of-mathematics.md#total-computable-function) $f:\mathbb N\to\mathbb N$ such that

$$
x\in A\quad\Longleftrightarrow\quad f(x)\in B.
$$

A [Turing reduction](../../../foundations-of-mathematics.md#turing-reduction) $A\leq_TB$ is an [oracle machine](../../../computer-science.md#oracle-machine) that, using membership queries to $B$, halts on every input and computes the [indicator function](../../../measure-theory.md#indicator-function) of $A$. It may make several adaptive queries, and need not preserve the yes/no answer to a single query. A [many-one reduction](../../../foundations-of-mathematics.md#many-one-reduction) yields a [Turing reduction](../../../foundations-of-mathematics.md#turing-reduction) by computing $f(x)$ and querying $B$ once. Two sets have the same [Turing degree](../../../foundations-of-mathematics.md#turing-degree) when each is [Turing reducible](../../../foundations-of-mathematics.md#turing-reduction) to the other. Write $0'$ for the degree of the [diagonal halting set](../../../foundations-of-mathematics.md#diagonal-halting-set) $K$.

We prove the [Kleene–Post incomparability theorem](../../../foundations-of-mathematics.md#kleene-post-incomparability-theorem) by an [oracle-assisted finite-extension construction](../../../foundations-of-mathematics.md#oracle-assisted-finite-extension-construction). Fix an effective list $(\Phi_e)$ of all [Turing functionals](../../../foundations-of-mathematics.md#turing-functional). We shall build increasing finite [binary strings](../../../computer-science.md#binary-string) $\alpha_s,\beta_s$ whose unions are the [indicator functions](../../../measure-theory.md#indicator-function) of $A,B$. A finite oracle computation $\Phi_e^\tau(n)\downarrow=v$ means that the computation halts with output $v$ and every oracle query is strictly below $|\tau|$. Its answers are supplied by $\tau$. By the finite [oracle use](../../../foundations-of-mathematics.md#oracle-use) property, every infinite oracle extending $\tau$ preserves this computation.

Here is the decision available from $K$. Given $e,n$ and a finite string $\beta$, consider

$$
E(e,n,\beta)\quad\Longleftrightarrow\quad\exists\tau\supseteq\beta\ \exists v\in\{0,1\}\ [\Phi_e^\tau(n)\downarrow=v].
$$

This predicate is [semidecidable](../../../foundations-of-mathematics.md#recursively-enumerable-set): enumerate all finite extensions $\tau$ of $\beta$ and dovetail their finite oracle simulations, stopping at the first halting binary output. There is a computably produced program which, on its own index as well as on every other input, performs this search and halts exactly if it succeeds. Membership of its code in $K$ therefore decides $E$. In a yes case, running the search finds an actual witness $(\tau,v)$. The decision oracle is essential in a no case; merely waiting would not produce a terminating construction.

Start with empty strings. At stage $s$ first ensure

$$
\Phi_s^B\ne\mathbf1_A.
$$

Choose $n=|\alpha_s|$, which is not yet assigned in $A$. Ask whether $E(s,n,\beta_s)$ holds. If yes, find a witness $(\tau,v)$, extend the current $B$ string to $\tau$, and append the bit $1-v$ to the current $A$ string. If no, leave the current $B$ string unchanged and append $0$ to the current $A$ string. The yes case permanently forces disagreement at $n$, since later strings extend both commitments. In the no case no final oracle extending the current $B$ string can give a binary output at $n$: any such convergent computation would use finitely many bits and hence supply a forbidden finite witness. Thus it cannot be the [indicator function](../../../measure-theory.md#indicator-function) of $A$ either, regardless of whether it diverges or returns a nonbinary value.

Next, using the strings just obtained, ensure

$$
\Phi_s^A\ne\mathbf1_B
$$

by the same procedure with the roles reversed. Choose $m$ equal to the current length of the $B$ string, ask the analogous extension question about the current $A$ string, and, if it has witness output $v$, extend $A$ to that witness and append $1-v$ to $B$. Otherwise append $0$ to $B$. Finally pad both strings with zeros if necessary so that each length is at least $s+1$, and call the resulting strings $\alpha_{s+1},\beta_{s+1}$. Every operation is computable using the membership oracle $K$ and terminates. Earlier disagreements remain protected because no already fixed bit is ever changed.

Set $\mathbf1_A=\bigcup_s\alpha_s$ and $\mathbf1_B=\bigcup_s\beta_s$. The length condition makes these total binary [functions](../../../function.md). To compute either bit $n$ with oracle $K$, run the construction through stage $n$, when both strings have length at least $n+1$, and read that bit. Consequently $A,B\leq_TK$. Every [Turing functional](../../../foundations-of-mathematics.md#turing-functional) has been defeated in both directions, so

$$
\boxed{A\not\leq_TB,\qquad B\not\leq_TA,\qquad A\leq_TK,\quad B\leq_TK.}
$$

Neither set is computable, since a computable set is [Turing reducible](../../../foundations-of-mathematics.md#turing-reduction) to every oracle. Neither can have degree $0'$: if $K\leq_TA$, then $B\leq_TK\leq_TA$, contrary to incomparability; the other case is symmetric. Therefore

$$
\boxed{0<\deg_T(A)<0',\qquad0<\deg_T(B)<0',\qquad\deg_T(A)\text{ and }\deg_T(B)\text{ are incomparable}.}
$$

This proves the requested theorem. The argument does not claim $A$ or $B$ is [computably enumerable](../../../foundations-of-mathematics.md#recursively-enumerable-set); it constructs sets computable in $K$. Obtaining incomparable [computably enumerable](../../../foundations-of-mathematics.md#recursively-enumerable-set) degrees is the stronger [Friedberg–Muchnik theorem](../../../foundations-of-mathematics.md#friedberg-muchnik-theorem), which is not needed for the printed request.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2012](../../2012.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
