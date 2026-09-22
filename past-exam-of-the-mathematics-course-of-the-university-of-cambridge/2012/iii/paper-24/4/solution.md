<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

For subsets $A,B\subseteq\mathbb N$, a [many-one reduction](../../../../../many-one-reduction.md) $A\leq_mB$ is a [total computable function](../../../../../total-computable-function.md) $f:\mathbb N\to\mathbb N$ such that

$$
x\in A\quad\Longleftrightarrow\quad f(x)\in B.
$$

A [Turing reduction](../../../../../turing-reduction.md) $A\leq_TB$ is an [oracle machine](../../../../../oracle-machine.md) that, using membership queries to $B$, halts on every input and computes the [indicator function](../../../../../indicator-function.md) of $A$. It may make several adaptive queries, and need not preserve the yes/no answer to a single query. A [many-one reduction](../../../../../many-one-reduction.md) yields a [Turing reduction](../../../../../turing-reduction.md) by computing $f(x)$ and querying $B$ once. Two sets have the same [Turing degree](../../../../../turing-degree.md) when each is [Turing reducible](../../../../../turing-reduction.md) to the other. Write $0'$ for the degree of the [diagonal halting set](../../../../../diagonal-halting-set.md) $K$.

We prove the [Kleene–Post incomparability theorem](../../../../../kleene-post-incomparability-theorem.md) by an [oracle-assisted finite-extension construction](../../../../../oracle-assisted-finite-extension-construction.md). Fix an effective list $(\Phi_e)$ of all [Turing functionals](../../../../../turing-functional.md). We shall build increasing finite [binary strings](../../../../../binary-string.md) $\alpha_s,\beta_s$ whose unions are the [indicator functions](../../../../../indicator-function.md) of $A,B$. A finite oracle computation $\Phi_e^\tau(n)\downarrow=v$ means that the computation halts with output $v$ and every oracle query is strictly below $|\tau|$. Its answers are supplied by $\tau$. By the finite [oracle use](../../../../../oracle-use.md) property, every infinite oracle extending $\tau$ preserves this computation.

Here is the decision available from $K$. Given $e,n$ and a finite string $\beta$, consider

$$
E(e,n,\beta)\quad\Longleftrightarrow\quad\exists\tau\supseteq\beta\ \exists v\in\{0,1\}\ [\Phi_e^\tau(n)\downarrow=v].
$$

This predicate is [semidecidable](../../../../../recursively-enumerable-set.md): enumerate all finite extensions $\tau$ of $\beta$ and dovetail their finite oracle simulations, stopping at the first halting binary output. There is a computably produced program which, on its own index as well as on every other input, performs this search and halts exactly if it succeeds. Membership of its code in $K$ therefore decides $E$. In a yes case, running the search finds an actual witness $(\tau,v)$. The decision oracle is essential in a no case; merely waiting would not produce a terminating construction.

Start with empty strings. At stage $s$ first ensure

$$
\Phi_s^B\ne\mathbf1_A.
$$

Choose $n=|\alpha_s|$, which is not yet assigned in $A$. Ask whether $E(s,n,\beta_s)$ holds. If yes, find a witness $(\tau,v)$, extend the current $B$ string to $\tau$, and append the bit $1-v$ to the current $A$ string. If no, leave the current $B$ string unchanged and append $0$ to the current $A$ string. The yes case permanently forces disagreement at $n$, since later strings extend both commitments. In the no case no final oracle extending the current $B$ string can give a binary output at $n$: any such convergent computation would use finitely many bits and hence supply a forbidden finite witness. Thus it cannot be the [indicator function](../../../../../indicator-function.md) of $A$ either, regardless of whether it diverges or returns a nonbinary value.

Next, using the strings just obtained, ensure

$$
\Phi_s^A\ne\mathbf1_B
$$

by the same procedure with the roles reversed. Choose $m$ equal to the current length of the $B$ string, ask the analogous extension question about the current $A$ string, and, if it has witness output $v$, extend $A$ to that witness and append $1-v$ to $B$. Otherwise append $0$ to $B$. Finally pad both strings with zeros if necessary so that each length is at least $s+1$, and call the resulting strings $\alpha_{s+1},\beta_{s+1}$. Every operation is computable using the membership oracle $K$ and terminates. Earlier disagreements remain protected because no already fixed bit is ever changed.

Set $\mathbf1_A=\bigcup_s\alpha_s$ and $\mathbf1_B=\bigcup_s\beta_s$. The length condition makes these total binary [functions](../../../../../function-split.md). To compute either bit $n$ with oracle $K$, run the construction through stage $n$, when both strings have length at least $n+1$, and read that bit. Consequently $A,B\leq_TK$. Every [Turing functional](../../../../../turing-functional.md) has been defeated in both directions, so

$$
\boxed{A\not\leq_TB,\qquad B\not\leq_TA,\qquad A\leq_TK,\quad B\leq_TK.}
$$

Neither set is computable, since a computable set is [Turing reducible](../../../../../turing-reduction.md) to every oracle. Neither can have degree $0'$: if $K\leq_TA$, then $B\leq_TK\leq_TA$, contrary to incomparability; the other case is symmetric. Therefore

$$
\boxed{0<\deg_T(A)<0',\qquad0<\deg_T(B)<0',\qquad\deg_T(A)\text{ and }\deg_T(B)\text{ are incomparable}.}
$$

This proves the requested theorem. The argument does not claim $A$ or $B$ is [computably enumerable](../../../../../recursively-enumerable-set.md); it constructs sets computable in $K$. Obtaining incomparable [computably enumerable](../../../../../recursively-enumerable-set.md) degrees is the stronger [Friedberg–Muchnik theorem](../../../../../friedberg-muchnik-theorem.md), which is not needed for the printed request.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 24](../../paper-24-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
