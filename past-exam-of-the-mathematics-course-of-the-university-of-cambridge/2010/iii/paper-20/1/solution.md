<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The printed arrow is a partial-function arrow. Thus the central objects are [partial computable functions](../../../../../computable-function.md) $f:\mathbb N^k\rightharpoonup\mathbb N$, with [total computable functions](../../../../../total-computable-function.md) as the special case in which every input has an output. Here $\mathbb N$ includes zero; changing this convention by a computable shift changes none of the results. A program computing $f$ must halt with output $f(\mathbf x)$ exactly on its domain, and run forever elsewhere. A finite program is a [function in intension](../../../../../function-in-intension.md), whereas its possibly partial input-output map is a [function in extension](../../../../../function-in-extension.md); many programs have the same extension.

A precise machine model is a [register machine](../../../../../register-machine.md) with finitely many instructions to increment a register, decrement it conditionally, jump, and halt. Registers hold [natural numbers](../../../../../natural-number.md). A [Turing machine](../../../../../turing-machine.md) instead uses a finite transition table, a finite alphabet and an unbounded tape. These models simulate one another: encode the finite nonblank tape, state and head position as numbers for the register simulation; conversely represent each register by a finite tape block and implement its increment and decrement by finite scans. Tuple inputs can be encoded by a [primitive recursive pairing function](../../../../../primitive-recursive-pairing-function.md). The equivalence of these formal models is a mathematical result. Their identification with every informal effective procedure is the [Church–Turing thesis](../../../../../church-turing-thesis.md), rather than an additional mathematical theorem about an already formal notion.

There is also an algebraic description. Begin with zero, successor and projections, close under [composition of partial functions](../../../../../composition-of-partial-functions.md) and [primitive recursion](../../../../../primitive-recursion.md), and then under [unbounded minimization](../../../../../mu-operator.md). The [primitive recursion](../../../../../primitive-recursion.md) scheme is

$$
f(\mathbf x,0)=g(\mathbf x),\qquad f(\mathbf x,n+1)=h(\mathbf x,n,f(\mathbf x,n)).
$$

Applied within the [primitive recursive](../../../../../primitive-recursive-function.md) class it produces only total functions, by [mathematical induction](../../../../../mathematical-induction.md) on $n$. [Unbounded minimization](../../../../../mu-operator.md) searches $y=0,1,\ldots$ for the first zero of $g(\mathbf x,y)$; its output is defined only if that search reaches such a zero with every preceding necessary computation defined. Composition is likewise strict about the intermediate values it requires. These schemes compile into machine programs using finite subroutines, loops and an unbounded search loop.

For the converse, encode a machine's finite configurations and finite computation histories using [Gödel numbering](../../../../../godel-numbering.md). Testing that a history starts with the specified input, that every adjacent pair follows the transition table, and that its final configuration halts is [primitive recursive](../../../../../primitive-recursive-function.md): all the tests are bounded by the finite code. Extracting the final output is [primitive recursive](../../../../../primitive-recursive-function.md) too. For a suitable checking predicate $T$ and output decoder $V$ this proves the [Kleene normal form theorem](../../../../../kleene-normal-form-theorem.md):

$$
\varphi_e(\mathbf x)\simeq V\bigl(\mu s\,T(e,\mathbf x,s)\bigr).
$$

The symbol $\simeq$ means equality of values and of definedness. A halting computation has a passing history code and every passing history has its actual output; a nonhalting computation has none. This proves that the partial recursive and machine-computable functions coincide, including their domains of divergence.

Finite programs can be effectively listed. Simulating the program with index $e$ gives a [universal partial computable function](../../../../../universal-partial-computable-function.md) $U(e,\mathbf x)\simeq\varphi_e(\mathbf x)$. Fixing some inputs is effective syntactically: prepend instructions writing those constants and then call the original program. This proves the [S-m-n theorem](../../../../../smn-theorem.md) in this machine presentation. In particular, reductions that construct a program from numerical parameters really do produce its index effectively.

The [primitive recursive functions](../../../../../primitive-recursive-function.md) are a proper subclass of the [total computable functions](../../../../../total-computable-function.md). Enumerate all valid unary [primitive recursive](../../../../../primitive-recursive-function.md) descriptions, interpreting invalid descriptions as zero. Evaluating any fixed valid description terminates by [structural induction](../../../../../structural-induction.md). Thus the diagonal map $d(n)=g_n(n)+1$ is total and computable, but cannot be one of the enumerated [primitive recursive](../../../../../primitive-recursive-function.md) maps, since $d(e)\ne g_e(e)$. This is a [total computable diagonal over primitive recursive syntax](../../../../../total-computable-diagonal-over-primitive-recursive-syntax.md). The evaluator can terminate on every particular description without itself being [primitive recursive](../../../../../primitive-recursive-function.md).

In contrast, one cannot effectively enumerate exactly the programs for all [total computable functions](../../../../../total-computable-function.md). If such an infinite enumeration were available, wait for its $n$th program and run it on $n$, then add one. Totality makes this another [total computable function](../../../../../total-computable-function.md), while its diagonal disagrees with every listed function. Equivalently, there is no total computable universal evaluator listing precisely all total computable maps.

The [halting problem](../../../../../halting-problem.md) is undecidable. If $H(e,x)$ decided whether program $e$ halts on $x$, construct a program $D$ which halts on input $e$ exactly when $H(e,e)$ says that it does not halt. Taking $e$ to be $D$'s own index gives a contradiction. The halting relation is nevertheless [computably enumerable](../../../../../recursively-enumerable-set.md), since finite halting histories can be searched for.

More generally, a set is [computably enumerable](../../../../../recursively-enumerable-set.md) exactly when it is the domain of a [partial computable function](../../../../../computable-function.md). From an enumeration, halt on $x$ when $x$ appears; in the other direction use [dovetailing](../../../../../dovetailing.md) over all inputs of a partial program to enumerate its halting inputs. A set is a [computable set](../../../../../computable-set.md) exactly when both it and its complement are [computably enumerable](../../../../../recursively-enumerable-set.md): dovetail the two searches and return the answer from the one that succeeds. Neither a semidecision procedure nor an unbounded search supplies a uniform negative answer.

Finally, the [Rice theorem](../../../../../rice-s-theorem.md) explains the scope of this obstruction. Let $P$ be a nontrivial property of the extension of a partial computable program. Choose a partial computable $g$ whose $P$-status differs from that of the nowhere-defined function. Given a program $e$ and input $x$, effectively form the program which, on $z$, first waits for $e(x)$ to halt and then computes $g(z)$. If $e(x)$ never halts its extension is nowhere defined; otherwise its extension is $g$. A decision procedure for $P$ would therefore decide the [halting problem](../../../../../halting-problem.md). **Effective descriptions allow universal simulation and positive verification, but not a decision procedure for every semantic property or for termination.**

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 20](../../paper-20-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
