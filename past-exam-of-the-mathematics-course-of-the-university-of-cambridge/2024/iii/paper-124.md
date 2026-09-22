# Paper 124

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2024/Paper_124.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2024/Paper_124.pdf)

**Table of contents**

- [1](#1)
  - [i](#1/i)
    - [Solution](#1/i/solution)
  - [ii](#1/ii)
    - [Solution](#1/ii/solution)
- [2](#2)
  - [i](#2/i)
    - [Solution](#2/i/solution)
  - [ii](#2/ii)
    - [Solution](#2/ii/solution)
  - [iii](#2/iii)
    - [Solution](#2/iii/solution)
- [3](#3)
  - [i](#3/i)
    - [Solution](#3/i/solution)
  - [ii](#3/ii)
    - [Solution](#3/ii/solution)
  - [iii](#3/iii)
    - [Solution](#3/iii/solution)
- [4](#4)
  - [i](#4/i)
    - [Solution](#4/i/solution)
  - [ii](#4/ii)
    - [Solution](#4/ii/solution)
  - [iii](#4/iii)
    - [Solution](#4/iii/solution)

## 1

↑ **Parent:** [Paper 124](paper-124.md)

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

This is [Ladner's theorem](../../../computer-science.md#ladner-s-theorem). Assume $\mathbf P\ne\mathbf{NP}$ and let $S$ be the [Boolean satisfiability problem](../../../computer-science.md#boolean-satisfiability-problem). Enumerate all clocked polynomial-time deterministic machines as $D_0,D_1,\ldots$ and all clocked polynomial-time candidate reductions as $R_0,R_1,\ldots$. A standard delayed-diagonalization schedule gives a nondecreasing, unbounded, polynomial-time computable function $s:\mathbb N\to\mathbb N$ that increases only by one. Define

$$
L=\{x\in S:s(|x|)\text{ is even}\}.
$$

The schedule alternates two requirements. At even stage $2j$, it holds $s$ fixed while searching successively larger finite sets of strings for an $x$ on which $D_j(x)$ disagrees with membership in $L$; after finding one it increments $s$. At odd stage $2j+1$, it searches for an $x$ such that

$$
x\in S\quad\Longleftrightarrow\quad R_j(x)\notin L,
$$

and then increments $s$. Length and simulation budgets are increased slowly enough that each finite search is eventually exhaustive but computing $s(n)$ still takes polynomial time. This is achieved, for example, by permitting only $n$ simulation steps and searches on strings of logarithmic length before deciding $s(n+1)$.

Every stage must finish. If an even stage $2j$ remained forever, then $s$ would eventually be a fixed even number, so $L$ and $S$ would differ on only finitely many strings. If $D_j$ decided $L$, those finitely many exceptions could be hardwired to decide $S$ in [P](../../../computer-science.md#p-complexity), contradicting $\mathbf P\ne\mathbf{NP}$. If an odd stage $2j+1$ remained forever, then $s$ would eventually be odd and $L$ would be finite. A correct [polynomial-time many-one reduction](../../../computer-science.md#polynomial-time-many-one-reduction) $R_j$ from $S$ to $L$ would again put $S$ in P. Thus every $D_j$ fails to decide $L$, and every $R_j$ fails to reduce $S$ to $L$.

Finally, $L\in\mathbf{NP}$: compute $s(|x|)$ and, when it is even, use the usual polynomial-time certificate for satisfiability. Hence

$$
\boxed{L\in\mathbf{NP}\setminus\mathbf P
\quad\text{and}\quad L\text{ is not NP-complete}.}
$$

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

The problem belongs to [NP](../../../computer-science.md#np-complexity): an assignment in $\mathbb F_2^n$ is a polynomial-length [certificate in computational complexity](../../../computer-science.md#certificate-complexity), and substitution verifies every equation in polynomial time.

For [NP-hardness](../../../computer-science.md#np-hardness), reduce the [Circuit satisfiability problem](../../../computer-science.md#circuit-satisfiability-problem). Introduce one variable in $\mathbb F_2$ for every wire of a [Boolean circuit](../../../computer-science.md#boolean-circuit). A [logical negation](../../../computer-science.md#negation) gate $w=\neg u$ is enforced by $w=1-u$, and a [logical conjunction](../../../mathematical-logic.md#logical-conjunction) gate $w=u\wedge v$ is enforced by $w=uv$. For a [logical disjunction](../../../mathematical-logic.md#logical-disjunction) gate use the suggested quadratic equation

$$
(1-u)(1-v)=1-w,
$$

which is equivalent to $w=u\vee v$ for bits $u,v,w$. Add the linear equation $w_{\rm out}=1$ for the designated output wire.

The construction introduces one variable and one equation per wire or gate, so it is a [polynomial-time many-one reduction](../../../computer-science.md#polynomial-time-many-one-reduction). A satisfying circuit input extends uniquely through its gates to a solution of the equations, and any solution gives a consistent accepting circuit computation. Since circuit satisfiability is NP-complete, [quadratic-equation satisfiability over F2](../../../computer-science.md#quadratic-equation-satisfiability-over-f2) is therefore

$$
\boxed{\mathbf{NP}\text{-complete}.}
$$

## 2

↑ **Parent:** [Paper 124](paper-124.md)

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

A decision problem $B$ is [NL-complete](../../../computer-science.md#nl-complete) when $B\in\mathbf{NL}$ and every language $A\in\mathbf{NL}$ has a deterministic [logarithmic space](../../../computer-science.md#logarithmic-space) many-one reduction to $B$.

The [directed graph reachability problem](../../../computer-science.md#st-connectivity) is the standard example. It lies in NL because a machine stores the current vertex and a counter, nondeterministically guesses at most $|V|-1$ successive edges, and accepts upon reaching $t$; this uses $O(\!\log|V|)$ space. For hardness, given an NL machine $M$ and input $x$, construct its [configuration graph](../../../computer-science.md#configuration-graph). Its configurations have logarithmic length, adjacency can be computed in logarithmic space, and

$$
M\text{ accepts }x
\quad\Longleftrightarrow\quad
\text{an accepting configuration is reachable from the initial configuration}.
$$

Adding one target joined from every accepting configuration gives the required logarithmic-space reduction.

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

It suffices to recognize non-reachability in [NL](../../../computer-science.md#nl-complexity), since directed reachability is NL-complete. Let $c_k$ be the number of vertices reachable from $s$ by a directed path of length at most $k$. Clearly $c_0=1$. The [inductive counting](../../../computer-science.md#inductive-counting) argument computes and verifies $c_{k+1}$ from $c_k$ using logarithmic space.

For each vertex $v$, reachability within $k+1$ steps has an NL certificate: guess such a path. Non-reachability within $k+1$ steps can be certified relative to the trusted value $c_k$ by enumerating vertices $u$, exhibiting paths of length at most $k$ to exactly $c_k$ distinct vertices, and checking that none is $v$ or has an edge to $v$. Because there are exactly $c_k$ reachable vertices, this list cannot omit a reachable predecessor. Counters, vertex names and one guessed path need only logarithmic space. Repeating this check in a fixed vertex order and counting the positive cases produces the exact $c_{k+1}$.

After $|V|-1$ rounds, the procedure knows the number of all vertices reachable from $s$. It accepts non-reachability of $t$ after certifying, by the same complete enumeration, that $t$ is absent. Thus the complement of directed reachability belongs to NL. Since every NL language reduces to reachability and log-space reductions are closed under complementation, this proves the [Immerman–Szelepcsényi theorem](../../../computer-science.md#immerman-szelepcsenyi-theorem)

$$
\boxed{\mathbf{NL}=\mathbf{co\text{-}NL}.}
$$

<h3 id="2/iii">iii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#2/iii)

Membership follows from $\mathbf{NL}=\mathbf{co\text{-}NL}$. A directed graph is not [strongly connected](../../../graph-theory.md#strong-connectivity) exactly when there is a pair $(u,v)$ for which $v$ is not reachable from $u$. Guessing the pair and using the NL procedure for non-reachability puts non-strong-connectivity in NL, hence strong connectivity is in co-NL and therefore in NL.

For NL-hardness, reduce directed reachability. Given $(G,s,t)$, form $G'$ by retaining all edges of $G$, adding $v\to s$ for every vertex $v$, and adding $t\to v$ for every vertex $v$. If $t$ is reachable from $s$ in $G$, then any $u$ reaches any $v$ in $G'$ along

$$
u\longrightarrow s\longrightarrow t\longrightarrow v.
$$

Conversely, if $G'$ is strongly connected then $s$ reaches $t$. A simple $s$-to-$t$ path cannot use an added edge out of $t$ before arriving at $t$, and every added edge into $s$ merely returns the path to its starting vertex; deleting the resulting cycle leaves an $s$-to-$t$ path made from edges of $G$. The construction is computable in logarithmic space, so deciding [strong connectivity](../../../graph-theory.md#strong-connectivity) is

$$
\boxed{\mathbf{NL}\text{-complete}.}
$$

## 3

↑ **Parent:** [Paper 124](paper-124.md)

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

Let $V(x,w)$ be a polynomial-time verifier for $f\in\mathbf{NP}$, with witnesses of length $p(|x|)$. Consider the prefix language

$$
B=\{(x,u):\text{there exists }v\text{ such that }V(x,uv)=1\}.
$$

This language lies in NP, so the assumption $\mathbf{NP}\subseteq\mathbf P/\mathrm{poly}$ supplies a [polynomial-size circuit family](../../../computer-science.md#polynomial-size-circuit-family) deciding $B$.

Apply the usual [search-to-decision reduction](../../../computer-science.md#search-to-decision-reduction). Starting with the empty prefix, append zero if the circuit says that some accepting witness has that extended prefix; otherwise append one. Repeat for $p(n)$ positions. Composing the polynomially many copies of the decision circuit produces a polynomial-size circuit $C_n$. Whenever $f(x)=1$, at least one accepting extension exists at every step, so the final string $C_n(x)$ satisfies

$$
\boxed{V(x,C_n(x))=1.}
$$

On negative inputs the output may be arbitrary, as required.

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

This is the [Karp–Lipton theorem](../../../computer-science.md#karp-lipton-theorem). It is enough to place $\Pi_2^{\mathbf P}$ inside $\Sigma_2^{\mathbf P}$. Let $L\in\Pi_2^{\mathbf P}$, so for a polynomial-time predicate $R$ and polynomially bounded strings,

$$
x\in L
\quad\Longleftrightarrow\quad
\forall y\ \exists z\ R(x,y,z).
$$

The NP search problem that receives $(x,y)$ and seeks such a $z$ has, by part (i), a [polynomial-size circuit family](../../../computer-science.md#polynomial-size-circuit-family) producing a valid witness whenever one exists. For each input length there is therefore a polynomial-size circuit $C$ such that, for every relevant $x,y$, existence of a witness implies $R(x,y,C(x,y))$.

Consequently

$$
x\in L
\quad\Longleftrightarrow\quad
\exists C\ \forall y\ R(x,y,C(x,y)),
$$

where the existentially guessed circuit description has polynomial length and evaluation of $C$ is polynomial time. This is a $\Sigma_2^{\mathbf P}$ description. Hence $\Pi_2^{\mathbf P}\subseteq\Sigma_2^{\mathbf P}$; complementation gives the reverse inclusion, and merging adjacent equal quantifier blocks collapses every higher level. Thus the [polynomial hierarchy](../../../computer-science.md#polynomial-hierarchy) satisfies

$$
\boxed{\mathbf{PH}=\Sigma_2^{\mathbf P}.}
$$

<h3 id="3/iii">iii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#3/iii)

**Yes.** The usual collapse relativizes because every machine involved receives the same [oracle](../../../computer-science.md#oracle-machine) $A$. Induct on the levels of the [polynomial hierarchy](../../../computer-science.md#polynomial-hierarchy). The hypothesis gives

$$
\Sigma_1^{\mathbf P,A}=\mathbf{NP}^A=\mathbf P^A.
$$

If the preceding level is contained in $\mathbf P^A$, then its oracle queries can be simulated in polynomial time with oracle $A$. A nondeterministic machine for the next existential level is therefore only an $\mathbf{NP}^A$ machine, hence a $\mathbf P^A$ machine by hypothesis. Complements give the corresponding universal level. The induction yields

$$
\boxed{\mathbf{PH}^A=\mathbf P^A.}
$$

## 4

↑ **Parent:** [Paper 124](paper-124.md)

<h3 id="4/i">i</h3>

↑ **Parent:** [4](#4)

<h4 id="4/i/solution">Solution</h4>

↑ **Parent:** [I](#4/i)

A language $L$ belongs to [RP](../../../computer-science.md#rp-complexity) when a polynomial-time [randomized algorithm](../../../computer-science.md#randomized-algorithm) rejects every $x\notin L$ and accepts every $x\in L$ with probability at least $1/2$.

Amplify the algorithm on length-$n$ inputs with $n+1$ independent repetitions, accepting if any repetition accepts. Its error on each positive input is at most $2^{-(n+1)}$, while it still never accepts a negative input. Choose all random bits for all repetitions in advance. By the [union bound](../../../probability-inequality.md#boole-s-inequality), the probability that this one fixed choice fails on at least one of the at most $2^n$ positive strings is at most

$$
2^n2^{-(n+1)}=\frac12.
$$

Thus some random string works simultaneously for every input of length $n$. Hardwire that string into the polynomial-time computation and compile it into a [Boolean circuit](../../../computer-science.md#boolean-circuit). The resulting [polynomial-size circuit family](../../../computer-science.md#polynomial-size-circuit-family) decides $L$, proving

$$
\boxed{\mathbf{RP}\subseteq\mathbf P/\mathrm{poly}.}
$$

<h3 id="4/ii">ii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#4/ii)

First suppose $L\in\mathbf{RP}\cap\mathbf{co\text{-}RP}$. Run the RP algorithm for $L$ and the RP algorithm for its complement with fresh random bits. If the first accepts, output one; if the second accepts, output zero; otherwise repeat. Neither output can be wrong, and on every input the appropriate algorithm accepts in each round with probability at least $1/2$. The number of rounds is dominated by a [geometric distribution](../../../discrete-probability-distribution.md#geometric-distribution) of mean two, so this is an always-correct algorithm with polynomial [expected running time](../../../probability-theory.md#expected-value).

Conversely, let $T$ be always correct when it halts and have expected running time at most $p(n)$. Run it for $2p(n)$ steps. [Markov inequality](../../../probability-inequality.md#markov-inequality) gives

$$
\mathbb P(T\text{ has not halted by }2p(n))\leq\frac12.
$$

Accept exactly when $T$ halts and outputs one; this is an RP algorithm for $L$. Accepting exactly when it halts and outputs zero is an RP algorithm for the complement. Therefore

$$
\boxed{\mathbf{ZPP}=\mathbf{RP}\cap\mathbf{co\text{-}RP}}
$$

is equivalent to zero-error expected polynomial time.

<h3 id="4/iii">iii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#4/iii)

We give the [Agrawal–Biswas primality test](../../../computer-science.md#agrawal-biswas-primality-test), which has one-sided error. Small inputs and [perfect powers](../../../number-theory.md#perfect-power) can first be recognized deterministically. For every remaining integer $n$, put $d=\lceil4\log_2n\rceil$ and choose a uniformly random monic polynomial

$$
r(X)=X^d+a_{d-1}X^{d-1}+\cdots+a_0
\in(\mathbb Z/n\mathbb Z)[X].
$$

Using repeated squaring in the quotient ring $(\mathbb Z/n\mathbb Z)[X]/(r)$, test the [identity](../../../computer-science.md#polynomial-identity-testing)

$$
(X+1)^n\equiv X^n+1\pmod{n,r(X)}.
$$

This takes time polynomial in $\log n$ because every intermediate polynomial has degree below $d=O(\!\log n)$.

If $n$ is [prime](../../../number-theory.md#prime-number), the intermediate [binomial coefficients](../../../combinatorics.md#binomial-coefficient) are divisible by $n$, so the identity always holds. Now suppose that $n$ is composite and is not a prime power. Choose a prime divisor $p$ and write $n=p^am$ with $p\nmid m$ and $m>1$. Over $\mathbb F_p$,

$$
(X+1)^n=(X^{p^a}+1)^m\ne X^n+1,
$$

because an intermediate coefficient equal to $m$ is nonzero modulo $p$. Hence

$$
F(X)=(X+1)^n-X^n-1
$$

is a nonzero polynomial of degree below $n$ over $\mathbb F_p$.

Reduction of random $r$ modulo $p$ is uniform among the $p^d$ monic degree-$d$ polynomials. The polynomial $F$ has at most $n/d$ distinct monic [irreducible](../../../polynomial.md#irreducible-polynomial) factors of degree $d$. On the other hand, the number $I_p(d)$ of monic irreducibles of degree $d$ obeys the standard lower bound

$$
I_p(d)\geq\frac{p^d}{d}-p^{d/2}.
$$

Whenever $r\bmod p$ is one of these irreducibles but does not divide $F$, the tested congruence fails. Thus one trial detects compositeness with probability at least

$$
\frac{I_p(d)-n/d}{p^d}
\geq\frac1d-p^{-d/2}-\frac{n}{dp^d}
\geq\frac1{2d}
$$

after the finitely many small $n$ are handled directly. Repeating $2d$ times makes the probability of missing a composite less than $(1-1/(2d))^{2d}<1/2$, while a prime is never rejected. Therefore compositeness is in [RP](../../../computer-science.md#rp-complexity), and primality testing is in

$$
\boxed{\mathbf{co\text{-}RP}.}
$$

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2024](../../2024.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
