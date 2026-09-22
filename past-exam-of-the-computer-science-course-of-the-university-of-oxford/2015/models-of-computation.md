# Models of computation

↑ **Parent:** [2015](../2015.md)

Solutions to all three questions of the [University of Oxford](../../university-of-oxford.md) [computer science](../../computer-science.md) finals paper held on 12 June 2015, Trinity Term 2015. The printed cover gives the date and paper code. All numbered subparts are treated.[Cover, p. 1; questions, pp. 2–3](../../computer-science-bibliography.md#models-of-computation-examination-paper-of-the-university-of-oxford-2015)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [i](#1/b/i)
      - [Solution](#1/b/i/solution)
    - [ii](#1/b/ii)
      - [Solution](#1/b/ii/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
  - [d](#1/d)
    - [Solution](#1/d/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [i](#2/b/i)
      - [Solution](#2/b/i/solution)
    - [ii](#2/b/ii)
      - [Solution](#2/b/ii/solution)
    - [iii](#2/b/iii)
      - [Solution](#2/b/iii/solution)
    - [iv](#2/b/iv)
      - [Solution](#2/b/iv/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [i](#3/b/i)
      - [Solution](#3/b/i/solution)
    - [ii](#3/b/ii)
      - [Solution](#3/b/ii/solution)
  - [c](#3/c)
    - [i](#3/c/i)
      - [Solution](#3/c/i/solution)
    - [ii](#3/c/ii)
      - [Solution](#3/c/ii/solution)
  - [d](#3/d)
    - [i](#3/d/i)
      - [Solution](#3/d/i/solution)
    - [ii](#3/d/ii)
      - [Solution](#3/d/ii/solution)

## 1

↑ **Parent:** [Models of computation](models-of-computation.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

A [nondeterministic finite automaton](../../foundations-of-mathematics.md#nondeterministic-finite-automaton), allowing the [epsilon transitions](../../foundations-of-mathematics.md#epsilon-transition) used in this paper, is a [tuple](../../set-theory.md#finite-tuple)

$$
M=(Q,\Sigma,\delta,q_0,F),\qquad
\delta:Q\times(\Sigma\cup\{\varepsilon\})\longrightarrow\mathcal P(Q).
$$

Here $Q$ is a nonempty [finite set](../../set.md#finite-set) of [automaton states](../../foundations-of-mathematics.md#automaton-state), $\Sigma$ is a finite [alphabet](../../information-theory.md#alphabet), $\mathcal P(Q)$ is the [power set](../../set.md#power-set) of $Q$, $q_0\in Q$ is the initial [automaton state](../../foundations-of-mathematics.md#automaton-state), and $F\subseteq Q$ is the [set](../../set.md) of accepting [automaton states](../../foundations-of-mathematics.md#automaton-state). The symbol $\varepsilon\notin\Sigma$ denotes the [empty word](../../foundations-of-mathematics.md#empty-word). Membership $r\in\delta(q,a)$ permits an [automaton transition](../../foundations-of-mathematics.md#automaton-transition) from $q$ to $r$ consuming $a$ when $a\in\Sigma$, or consuming nothing when $a=\varepsilon$.

The recognized [formal language](../../theoretical-computer-science.md#formal-language) is

$$
\boxed{L(M)=\{w\in\Sigma^*: \text{some finite path from }q_0\text{ to a state in }F\text{ has label }w\}.}
$$

The label of a [graph path](../../graph-theory.md#path-in-a-graph) is the [concatenation](../../foundations-of-mathematics.md#concatenation) of its labels with all occurrences of $\varepsilon$ omitted. Thus acceptance requires consuming the entire input [word](../../foundations-of-mathematics.md#string); a single successful choice of [automaton transitions](../../foundations-of-mathematics.md#automaton-transition) suffices. A path of length zero is allowed, so the [empty word](../../foundations-of-mathematics.md#empty-word) is accepted whenever $q_0\in F$, or an accepting [automaton state](../../foundations-of-mathematics.md#automaton-state) is reachable by [epsilon transitions](../../foundations-of-mathematics.md#epsilon-transition). If [epsilon transitions](../../foundations-of-mathematics.md#epsilon-transition) are excluded from the definition of a [nondeterministic finite automaton](../../foundations-of-mathematics.md#nondeterministic-finite-automaton), the displayed version is called an [Epsilon-NFA](../../foundations-of-mathematics.md#epsilon-nfa).

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/i">i</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/i/solution">Solution</h5>

↑ **Parent:** [I](#1/b/i)

For $x$, there is an accepting [graph path](../../graph-theory.md#path-in-a-graph)

$$
q_0\xrightarrow{1}q_1\xrightarrow{1}q_2
\xrightarrow{0}q_0\xrightarrow{0}q_0
\xrightarrow{1}q_1\xrightarrow{1}q_2
\xrightarrow{0}q_0\xrightarrow{\varepsilon}q_2.
$$

Its nonempty labels spell $1100110$, and its last [automaton state](../../foundations-of-mathematics.md#automaton-state) is accepting. **Therefore $x$ is accepted.** The last [epsilon transition](../../foundations-of-mathematics.md#epsilon-transition) matters: finishing the consumed input at $q_0$ does not prevent a subsequent move to $q_2$.

For $y$, track all possible [automaton states](../../foundations-of-mathematics.md#automaton-state), including their [epsilon closure](../../foundations-of-mathematics.md#epsilon-closure), after each input prefix:

| Input prefix | Possible [automaton states](../../foundations-of-mathematics.md#automaton-state) after [epsilon closure](../../foundations-of-mathematics.md#epsilon-closure) |
| --- | --- |
| $\varepsilon$ | $\{q_0,q_2\}$ |
| $1$ | $\{q_1\}$ |
| $11$ | $\{q_2\}$ |
| $110$ | $\{q_0,q_2\}$ |
| $1100$ | $\{q_0,q_2\}$ |
| $11001$ | $\{q_1\}$ |

The final [set](../../set.md) contains no accepting [automaton state](../../foundations-of-mathematics.md#automaton-state), and $q_1$ has no outgoing [epsilon transition](../../foundations-of-mathematics.md#epsilon-transition). **Therefore $y$ is rejected.**

$$
\boxed{x\in L(M),\qquad y\notin L(M).}
$$

<h4 id="1/b/ii">ii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/b/ii)

Use [state elimination for finite automata](../../foundations-of-mathematics.md#state-elimination-for-finite-automata), with [regular expression](../../foundations-of-mathematics.md#regular-expression) labels on a [generalized finite automaton](../../foundations-of-mathematics.md#generalized-finite-automaton). Add a fresh initial [automaton state](../../foundations-of-mathematics.md#automaton-state) $s$ with $s\xrightarrow{\varepsilon}q_0$, and a fresh final [automaton state](../../foundations-of-mathematics.md#automaton-state) $f$ with $q_2\xrightarrow{\varepsilon}f$. Only $f$ is now accepting. Missing labels represent the [empty language](../../theoretical-computer-science.md#empty-language), and parallel alternatives are combined by [union](../../set.md#set-union).

When eliminating an internal [automaton state](../../foundations-of-mathematics.md#automaton-state) $k$, update every surviving label by

$$
R_{ij}\longleftarrow R_{ij}\cup R_{ik}(R_{kk})^*R_{kj}.
$$

The added [regular expression](../../foundations-of-mathematics.md#regular-expression) describes entering $k$, traversing its loop zero or more times by [Kleene star](../../foundations-of-mathematics.md#kleene-star), and leaving it. This accounts for exactly the [graph paths](../../graph-theory.md#path-in-a-graph) newly bypassing $k$.

First eliminate $q_1$. Its only incoming and outgoing labels are both $1$, and it has no loop. The [graph path](../../graph-theory.md#path-in-a-graph) through it contributes $11$, so the label from $q_0$ to $q_2$ becomes

$$
R_{02}=\varepsilon\cup11.
$$

The other relevant labels are still $R_{00}=0$, $R_{20}=0$, and $R_{2f}=\varepsilon$.

Next eliminate $q_2$. It has no loop, so the new loop at $q_0$ and the new label to $f$ are

$$
\begin{aligned}
R_{00}&=0\cup(\varepsilon\cup11)0=0\cup110,\\
R_{0f}&=(\varepsilon\cup11)\varepsilon=\varepsilon\cup11.
\end{aligned}
$$

Finally eliminate $q_0$. The label from $s$ to $f$ is

$$
\varepsilon(0\cup110)^*(\varepsilon\cup11).
$$

Thus an equivalent [regular expression](../../foundations-of-mathematics.md#regular-expression) is

$$
\boxed{(0\cup110)^*(\varepsilon\cup11).}
$$

For an independent interpretation, every completed return to $q_0$ consumes either $0$ or $110$: the latter traverses $q_1,q_2$ before returning. The last visit to $q_2$ consumes either nothing or $11$. Consequently every run of ones has length exactly two, and successive such runs require at least one zero between them. In particular, consecutive copies of $11$ without a separating zero are not accepted.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Let $A=(Q,\{0,1\},\delta,q_0,F)$ be a [deterministic finite automaton](../../foundations-of-mathematics.md#deterministic-finite-automaton) recognizing $L$. Construct a [nondeterministic finite automaton](../../foundations-of-mathematics.md#nondeterministic-finite-automaton) $B$ with [automaton state](../../foundations-of-mathematics.md#automaton-state) [set](../../set.md) $Q\times\{0,1\}$. Its second coordinate records whether the extra zero has already been consumed. Start at $(q_0,0)$ and make exactly the [automaton states](../../foundations-of-mathematics.md#automaton-state) in $F\times\{1\}$ accepting.

For each $q\in Q$, $i\in\{0,1\}$, and $a\in\{0,1\}$, include the ordinary [automaton transition](../../foundations-of-mathematics.md#automaton-transition)

$$
(q,i)\xrightarrow{a}(\delta(q,a),i).
$$

Also include the extra [automaton transition](../../foundations-of-mathematics.md#automaton-transition)

$$
\boxed{(q,0)\xrightarrow{0}(q,1)\qquad(q\in Q).}
$$

This consumes the inserted zero without changing the simulated [automaton state](../../foundations-of-mathematics.md#automaton-state) of $A$. At a zero in layer zero, both the ordinary and extra choices are available. There are no [automaton transitions](../../foundations-of-mathematics.md#automaton-transition) from layer one back to layer zero.

If $xy\in L$, run $A$ on $x$ in layer zero, consume the extra zero by the displayed [automaton transition](../../foundations-of-mathematics.md#automaton-transition), and run $A$ on $y$ in layer one. The resulting run accepts $x0y$ in $B$.

Conversely, every accepting run of $B$ starts in layer zero and finishes in layer one, so it uses exactly one extra [automaton transition](../../foundations-of-mathematics.md#automaton-transition). Split its input as $x0y$ at that move. Removing that consumed zero leaves precisely a run of $A$ on $xy$, ending in $F$. Hence $xy\in L$. The construction also permits an insertion at either end, including insertion into the [empty word](../../foundations-of-mathematics.md#empty-word).

Therefore $L(B)=L'$. Since $B$ has $2|Q|$ [automaton states](../../foundations-of-mathematics.md#automaton-state), **$L'$ is a [regular language](../../foundations-of-mathematics.md#regular-language)**. This is a [single-symbol insertion into a regular language](../../foundations-of-mathematics.md#single-symbol-insertion-into-a-regular-language).

$$
\boxed{L'=L(B)\text{ is regular}.}
$$

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

**No: [regular languages](../../foundations-of-mathematics.md#regular-language) are not closed under countably infinite [intersection](../../set.md#set-intersection).** Let $\Sigma=\{0,1\}$ and put

$$
K=\{0^n1^n:n\geq0\},\qquad
L_i=\{w\in\Sigma^*:|w|\geq i\}\cup\{0^n1^n:2n<i\},\quad i\geq1.
$$

The first term in $L_i$ has [regular expression](../../foundations-of-mathematics.md#regular-expression) $(0\cup1)^i(0\cup1)^*$, where the fixed power $i$ means $i$ copies. The second term is a [finite language](../../foundations-of-mathematics.md#finite-language), a finite [union](../../set.md#set-union) of single [words](../../foundations-of-mathematics.md#string). Their [union](../../set.md#set-union) is therefore a [regular language](../../foundations-of-mathematics.md#regular-language).

If $w\in K$, then for each $i$ either $|w|\geq i$ or $w$ belongs to the second term, so $w\in L_i$. If $w\notin K$, choose $i>|w|$. It belongs to neither term of $L_i$. Consequently

$$
\boxed{\bigcap_{i=1}^{\infty}L_i=K.}
$$

The [formal language](../../theoretical-computer-science.md#formal-language) $K$ is not a [regular language](../../foundations-of-mathematics.md#regular-language). Indeed, for a proposed [pumping length](../../foundations-of-mathematics.md#pumping-length) $p\geq1$, the [pumping lemma for regular languages](../../foundations-of-mathematics.md#pumping-lemma-for-regular-languages) applied to $0^p1^p$ must pump a nonempty block consisting only of zeros. Repeating that block increases the number of zeros without increasing the number of ones, leaving $K$. This contradiction proves the counterexample. Finite [intersection](../../set.md#set-intersection) closure does not extend to this [infinite intersection of regular languages](../../foundations-of-mathematics.md#infinite-intersection-of-regular-languages).

## 2

↑ **Parent:** [Models of computation](models-of-computation.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

A [nondeterministic pushdown automaton](../../foundations-of-mathematics.md#pushdown-automaton) is a [tuple](../../set-theory.md#finite-tuple)

$$
M=(Q,\Sigma,\Gamma,\delta,q_0,Z_0,F),\qquad
\delta:Q\times(\Sigma\cup\{\varepsilon\})\times\Gamma
\longrightarrow\mathcal P_{\mathrm{fin}}(Q\times\Gamma^*).
$$

Here $Q$ is a nonempty [finite set](../../set.md#finite-set) of control states, $\Sigma$ a finite input [alphabet](../../information-theory.md#alphabet), $\Gamma$ a finite [stack alphabet](../../information-theory.md#stack-alphabet), $q_0\in Q$ the initial control state, $Z_0\in\Gamma$ the initial [stack](../../data-structure.md#stack-data-structure) symbol, and $F\subseteq Q$ the final control states. The notation $\mathcal P_{\mathrm{fin}}$ requires each transition to have only finitely many choices. Since the domain is finite, the whole transition specification is finite.

A [pushdown automaton configuration](../../foundations-of-mathematics.md#pushdown-automaton-configuration) is $(q,w,\alpha)\in Q\times\Sigma^*\times\Gamma^*$, recording the control state, unread input [word](../../foundations-of-mathematics.md#string), and [stack](../../data-structure.md#stack-data-structure) contents. Write the top of the [stack](../../data-structure.md#stack-data-structure) on the left. For $a\in\Sigma$, the one-step relation is

$$
(q,aw,X\beta)\vdash_M(r,w,\gamma\beta)
\quad\text{if }(r,\gamma)\in\delta(q,a,X).
$$

An [epsilon transition](../../foundations-of-mathematics.md#epsilon-transition) instead has

$$
(q,w,X\beta)\vdash_M(r,w,\gamma\beta)
\quad\text{if }(r,\gamma)\in\delta(q,\varepsilon,X).
$$

Thus a move replaces the top [stack](../../data-structure.md#stack-data-structure) symbol $X$ by the [word](../../foundations-of-mathematics.md#string) $\gamma$, whose leftmost symbol becomes the new top. It consumes one input symbol or no input symbol. Under this convention there is no move from an empty [stack](../../data-structure.md#stack-data-structure).

For [acceptance by final state](../../foundations-of-mathematics.md#acceptance-by-final-state), the recognized [formal language](../../theoretical-computer-science.md#formal-language) is

$$
\boxed{L(M)=\{w\in\Sigma^*: (q_0,w,Z_0)\vdash_M^*(f,\varepsilon,\alpha)
\text{ for some }f\in F,\ \alpha\in\Gamma^*\}.}
$$

Here $\vdash_M^*$ allows any finite number of moves, including zero. The entire input must have been consumed; the final [stack](../../data-structure.md#stack-data-structure) need not be empty. Acceptance requires at least one such run of the [nondeterministic pushdown automaton](../../foundations-of-mathematics.md#pushdown-automaton).

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/i">i</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/i/solution">Solution</h5>

↑ **Parent:** [I](#2/b/i)

A [context-free grammar](../../foundations-of-mathematics.md#context-free-grammar) is **an [ambiguous grammar](../../foundations-of-mathematics.md#ambiguous-grammar) if some [word](../../foundations-of-mathematics.md#string) in its generated [formal language](../../theoretical-computer-science.md#formal-language) has two distinct [parse trees](../../foundations-of-mathematics.md#parse-tree)**. Equivalently, that [word](../../foundations-of-mathematics.md#string) has two distinct [leftmost derivations](../../foundations-of-mathematics.md#leftmost-derivation) from the start [nonterminal symbol](../../foundations-of-mathematics.md#nonterminal-symbol). A [leftmost derivation](../../foundations-of-mathematics.md#leftmost-derivation) always expands the leftmost remaining [nonterminal symbol](../../foundations-of-mathematics.md#nonterminal-symbol).

Two arbitrary [grammar derivations](../../foundations-of-mathematics.md#grammar-derivation) of the same [word](../../foundations-of-mathematics.md#string) do not by themselves prove ambiguity: expanding independent [nonterminal symbols](../../foundations-of-mathematics.md#nonterminal-symbol) in a different order can describe the same [parse tree](../../foundations-of-mathematics.md#parse-tree). Requiring distinct [parse trees](../../foundations-of-mathematics.md#parse-tree), or distinct [leftmost derivations](../../foundations-of-mathematics.md#leftmost-derivation), avoids that issue.

$$
\boxed{\text{Ambiguity means two distinct parse trees for at least one word}.}
$$

<h4 id="2/b/ii">ii</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/b/ii)

The [word](../../foundations-of-mathematics.md#string) $abb$ has these two [leftmost derivations](../../foundations-of-mathematics.md#leftmost-derivation):

$$
\begin{aligned}
S&\Rightarrow UST\Rightarrow aTST\Rightarrow abST
\Rightarrow abT\Rightarrow abb,\\
S&\Rightarrow UST\Rightarrow aST\Rightarrow aSTT
\Rightarrow aTT\Rightarrow abT\Rightarrow abb.
\end{aligned}
$$

In the first [grammar derivation](../../foundations-of-mathematics.md#grammar-derivation), $U\to aT$ supplies an extra $b$; the remaining $S$ goes directly to the [empty word](../../foundations-of-mathematics.md#empty-word). In the second [grammar derivation](../../foundations-of-mathematics.md#grammar-derivation), $U\to a$ is used, and the remaining $S$ uses $S\to ST$ before disappearing. Every step expands the leftmost [nonterminal symbol](../../foundations-of-mathematics.md#nonterminal-symbol), so these are genuinely different [leftmost derivations](../../foundations-of-mathematics.md#leftmost-derivation), with different [parse trees](../../foundations-of-mathematics.md#parse-tree) already distinguished by the [production rule](../../foundations-of-mathematics.md#production-rule) at the $U$ node.

**Therefore $G$ is an [ambiguous grammar](../../foundations-of-mathematics.md#ambiguous-grammar), witnessed by $abb$.**

$$
\boxed{abb\text{ has two distinct leftmost derivations in }G.}
$$

<h4 id="2/b/iii">iii</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#2/b/iii)

Use the standard [conversion of a context-free grammar to a pushdown automaton](../../foundations-of-mathematics.md#conversion-of-a-context-free-grammar-to-a-pushdown-automaton), implementing a [leftmost derivation](../../foundations-of-mathematics.md#leftmost-derivation) on a [stack](../../data-structure.md#stack-data-structure). Take control states $q_s,q,q_f$, input [alphabet](../../information-theory.md#alphabet) $\{a,b\}$, [stack alphabet](../../information-theory.md#stack-alphabet) $\{S,T,U,a,b,\bot\}$, initial control state $q_s$, initial [stack](../../data-structure.md#stack-data-structure) symbol $\bot$, and sole final control state $q_f$. The symbol $\bot$ is a fresh [stack bottom marker](../../data-structure.md#stack-bottom-marker). As in part (a), the top of the [stack](../../data-structure.md#stack-data-structure) is written on the left.

Initialize with

$$
\delta(q_s,\varepsilon,\bot)=\{(q,S\bot)\}.
$$

In control state $q$, replace a top [nonterminal symbol](../../foundations-of-mathematics.md#nonterminal-symbol) by one of its [production rule](../../foundations-of-mathematics.md#production-rule) right-hand sides:

$$
\begin{aligned}
\delta(q,\varepsilon,S)&=\{(q,UST),(q,ST),(q,\varepsilon)\},\\
\delta(q,\varepsilon,U)&=\{(q,a),(q,aT)\},\\
\delta(q,\varepsilon,T)&=\{(q,b)\}.
\end{aligned}
$$

The replacements are written in the order in which they are to be processed. For example, replacing $S$ by $UST$ leaves $U$ on top; an implementation using individual push operations pushes $T$, then $S$, then $U$.

Match and pop top [terminal symbols](../../foundations-of-mathematics.md#terminal-symbol) by

$$
\delta(q,a,a)=\{(q,\varepsilon)\},\qquad
\delta(q,b,b)=\{(q,\varepsilon)\}.
$$

Finally include

$$
\delta(q,\varepsilon,\bot)=\{(q_f,\bot)\}.
$$

All unlisted transitions have no choices; $q_f$ has no outgoing transitions. This is [acceptance by final state](../../foundations-of-mathematics.md#acceptance-by-final-state), leaving the bottom marker on the [stack](../../data-structure.md#stack-data-structure). Taking the last transition too early cannot cause false acceptance, because an unread input suffix remains and $q_f$ cannot consume it.

For correctness, after initialization the [stack](../../data-structure.md#stack-data-structure) contains the unprocessed part of a sentential form. Expanding a top [nonterminal symbol](../../foundations-of-mathematics.md#nonterminal-symbol) simulates one step of a [leftmost derivation](../../foundations-of-mathematics.md#leftmost-derivation), and popping a matching [terminal symbol](../../foundations-of-mathematics.md#terminal-symbol) transfers it to the already-read input prefix. Thus if the input prefix consumed so far is $u$ and the [stack](../../data-structure.md#stack-data-structure) above $\bot$ is $\alpha$, then $S\Rightarrow_G^*u\alpha$. Acceptance gives $S\Rightarrow_G^*w$ for the entire input $w$.

Conversely, any [leftmost derivation](../../foundations-of-mathematics.md#leftmost-derivation) of $w$ specifies choices of these transitions: expand the next [nonterminal symbol](../../foundations-of-mathematics.md#nonterminal-symbol), and read each resulting leading [terminal symbol](../../foundations-of-mathematics.md#terminal-symbol) when it reaches the top. After all symbols of $w$ are consumed, only $\bot$ remains, enabling the move to $q_f$. **The [nondeterministic pushdown automaton](../../foundations-of-mathematics.md#pushdown-automaton) therefore recognizes exactly $L(G)$.** The [empty word](../../foundations-of-mathematics.md#empty-word) is accepted by choosing $S\to\varepsilon$ after initialization.

$$
\boxed{L(M)=L(G),\qquad F=\{q_f\}.}
$$

<h4 id="2/b/iv">iv</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#2/b/iv)

Every generated [word](../../foundations-of-mathematics.md#string) satisfies

$$
\#_b(w)\geq\#_a(w),
$$

where $\#_a,\#_b$ count occurrences of the indicated [terminal symbols](../../foundations-of-mathematics.md#terminal-symbol). To see this, follow the unique chain of $S$ occurrences in a [parse tree](../../foundations-of-mathematics.md#parse-tree). Each use of $S\to UST$ introduces one $a$ from $U$, at least one $b$ from its rightmost $T$, and possibly one further $b$ from $U\to aT$. Each use of $S\to ST$ adds one $b$ and no $a$. The terminating $S\to\varepsilon$ contributes neither. Hence no generated [word](../../foundations-of-mathematics.md#string) has more $a$ symbols than $b$ symbols.

Also, for every $n\geq0$, the [word](../../foundations-of-mathematics.md#string) $a^nb^n$ is generated: apply $S\to UST$ exactly $n$ times, choose $U\to a$ each time, then use $S\to\varepsilon$ and all remaining $T\to b$.

Suppose $L(G)$ were a [regular language](../../foundations-of-mathematics.md#regular-language), and let $p\geq1$ be a [pumping length](../../foundations-of-mathematics.md#pumping-length) from the [pumping lemma for regular languages](../../foundations-of-mathematics.md#pumping-lemma-for-regular-languages). Apply it to $w=a^pb^p$. Every allowed decomposition $w=xyz$ with $|xy|\leq p$ and $|y|>0$ has $y=a^r$ for some $r\geq1$. Pumping twice gives

$$
xy^2z=a^{p+r}b^p,
$$

which violates the proved counting inequality and hence is not generated. This contradicts the [pumping lemma for regular languages](../../foundations-of-mathematics.md#pumping-lemma-for-regular-languages). **Therefore $L(G)$ is not a [regular language](../../foundations-of-mathematics.md#regular-language).** Ambiguity was not used: the obstruction is the unbounded constraint on symbol counts.

$$
\boxed{L(G)\text{ is not regular}.}
$$

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

**$P$ is a [co-recursively enumerable language](../../foundations-of-mathematics.md#co-recursively-enumerable-language), is not a [recursively enumerable language](../../foundations-of-mathematics.md#recursively-enumerable-language), and is not a [decidable language](../../foundations-of-mathematics.md#recursive-language).** The stipulated order on halting times includes $\infty\geq\infty$.

First, failure has a finite witness. For valid machine descriptions,

$$
\langle N_1,N_2\rangle\notin P
\quad\Longleftrightarrow\quad
\exists x\ \exists t\in\mathbb N:
\bigl[N_1(x)\text{ halts after exactly }t\text{ transitions}\bigr]
\land
\bigl[N_2(x)\text{ has not halted by }t\bigr].
$$

Indeed, a strict inequality $t(N_1,x)<t(N_2,x)$ forces the first halting time to be finite. The second can be either a larger finite time or infinity. Whether the displayed condition holds for fixed $x,t$ is decidable by a finite simulation, including the initial configurations when $t=0$.

Enumerate all pairs $(x,t)$ and perform these finite tests by [dovetailing](../../computability-theory.md#dovetailing), accepting the [complement of a set](../../set.md#complement-of-a-set) of $P$ on finding a witness. Equivalently, at stage $s$, inspect all inputs of length at most $s$ through $s$ transitions. A genuine violation eventually appears; if there is no violation, the procedure never accepts. Malformed descriptions or differing input [alphabets](../../information-theory.md#alphabet) can be recognized and accepted as nonmembers immediately. Thus the complement is a [recursively enumerable language](../../foundations-of-mathematics.md#recursively-enumerable-language), proving that $P$ is a [co-recursively enumerable language](../../foundations-of-mathematics.md#co-recursively-enumerable-language).

For non-enumerability, use the standard result that the [complement of a set](../../set.md#complement-of-a-set) of the [halting problem](../../foundations-of-mathematics.md#halting-problem)

$$
H=\{\langle M,w\rangle:M\text{ halts on }w\}
$$

is not a [recursively enumerable language](../../foundations-of-mathematics.md#recursively-enumerable-language). Given $\langle M,w\rangle$, effectively construct two [Turing machines](../../theoretical-computer-science.md#turing-machine) over the same fixed input [alphabet](../../information-theory.md#alphabet). On every input $x$, let $N_1$ ignore $x$ and simulate $M$ on the fixed [word](../../foundations-of-mathematics.md#string) $w$, halting precisely when that simulation halts. Let $N_2$ loop forever on every input.

If $M$ does not halt on $w$, both halting times are infinity for every $x$, so the pair belongs to $P$. If $M$ halts on $w$, the first halting time is finite while the second is infinity, so the pair does not belong to $P$. Therefore

$$
\boxed{\langle M,w\rangle\notin H
\quad\Longleftrightarrow\quad
\langle N_1,N_2\rangle\in P.}
$$

This is a [many-one reduction](../../computability-theory.md#many-one-reduction) from non-halting to the [pointwise running-time domination problem](../../computability-theory.md#pointwise-running-time-domination-problem). Were $P$ a [recursively enumerable language](../../foundations-of-mathematics.md#recursively-enumerable-language), constructing the pair and running its recognizer would recognize non-halting, contradicting the stated result. Hence $P$ is not a [recursively enumerable language](../../foundations-of-mathematics.md#recursively-enumerable-language). Since every [decidable language](../../foundations-of-mathematics.md#recursive-language) is a [recursively enumerable language](../../foundations-of-mathematics.md#recursively-enumerable-language), $P$ is also undecidable.

$$
\boxed{P\text{ is co-R.E., not R.E., and undecidable}.}
$$

## 3

↑ **Parent:** [Models of computation](models-of-computation.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Fix a deterministic, single-tape [Turing machine](../../theoretical-computer-science.md#turing-machine) with tape cells indexed by the [integers](../../integer.md). A precise definition is the [tuple](../../set-theory.md#finite-tuple)

$$
M=(Q,\Sigma,\Gamma,\delta,q_0,q_{\mathrm{acc}},q_{\mathrm{rej}}),\qquad
\delta:(Q\setminus\{q_{\mathrm{acc}},q_{\mathrm{rej}}\})\times\Gamma
\longrightarrow Q\times\Gamma\times\{L,R\}.
$$

Here $Q$ is a nonempty [finite set](../../set.md#finite-set) of control states, $\Gamma$ a finite tape [alphabet](../../information-theory.md#alphabet) with a designated [blank symbol](../../theoretical-computer-science.md#blank-symbol) $\square$, $\Sigma\subseteq\Gamma\setminus\{\square\}$ the input [alphabet](../../information-theory.md#alphabet), $q_0\in Q$ the initial control state, and $q_{\mathrm{acc}},q_{\mathrm{rej}}\in Q$ distinct halting control states. The transition [function](../../function.md) is total on the displayed domain. The [Turing machine instruction](../../theoretical-computer-science.md#instruction-of-a-turing-machine) $\delta(q,a)=(r,b,D)$ means to write $b$ over the scanned $a$, enter control state $r$, and move the head one cell in direction $D$.

A [Turing machine configuration](../../theoretical-computer-science.md#instantaneous-description-of-a-turing-machine) is $(q,\tau,h)$, where $q\in Q$, $h\in\mathbb Z$ is the head position, and $\tau:\mathbb Z\to\Gamma$ is the tape-content [function](../../function.md), equal to $\square$ outside a [finite set](../../set.md#finite-set). Its [next-configuration relation](../../theoretical-computer-science.md#next-configuration-relation) is

$$
(q,\tau,h)\vdash_M(r,\tau',h+d)
$$

if $\delta(q,\tau(h))=(r,b,D)$, with $d=-1$ for $D=L$ and $d=1$ for $D=R$, and

$$
\tau'(j)=\begin{cases}b&j=h,\\\tau(j)&j\ne h.\end{cases}
$$

There is no successor to either halting [Turing machine configuration](../../theoretical-computer-science.md#instantaneous-description-of-a-turing-machine).

For input $w=a_0\cdots a_{n-1}$, the initial [Turing machine configuration](../../theoretical-computer-science.md#instantaneous-description-of-a-turing-machine) is $C_0(w)=(q_0,\tau_w,0)$, where $\tau_w(j)=a_j$ for $0\leq j<n$ and is blank elsewhere. In particular, the initial tape for the [empty word](../../foundations-of-mathematics.md#empty-word) is entirely blank. The recognized [formal language](../../theoretical-computer-science.md#formal-language) is

$$
\boxed{L(M)=\{w\in\Sigma^*:C_0(w)\vdash_M^*(q_{\mathrm{acc}},\tau,h)
\text{ for some }\tau,h\}.}
$$

The relation $\vdash_M^*$ permits any finite number of transitions. An input outside $L(M)$ may reach the rejecting control state or run forever; recognition does not require halting on every input.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/i">i</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/i/solution">Solution</h5>

↑ **Parent:** [I](#3/b/i)

**The [formal language](../../theoretical-computer-science.md#formal-language) is a [regular language](../../foundations-of-mathematics.md#regular-language).** A [regular expression](../../foundations-of-mathematics.md#regular-expression) for it is

$$
\boxed{(ab)^*(bc)^*.}
$$

The first [Kleene star](../../foundations-of-mathematics.md#kleene-star) independently chooses $m$ copies of the [word](../../foundations-of-mathematics.md#string) $ab$, and the second independently chooses $n$ copies of $bc$. Their [concatenation](../../foundations-of-mathematics.md#concatenation) produces exactly the required [words](../../foundations-of-mathematics.md#string). Either count may be zero, including both counts zero, which gives the [empty word](../../foundations-of-mathematics.md#empty-word). By [Kleene theorem](../../foundations-of-mathematics.md#kleene-theorem), the [regular expression](../../foundations-of-mathematics.md#regular-expression) establishes regularity.

<h4 id="3/b/ii">ii</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/b/ii)

**The [formal language](../../theoretical-computer-science.md#formal-language) is not a [regular language](../../foundations-of-mathematics.md#regular-language).** Let $K$ denote it and consider the infinitely many prefixes

$$
u_i=(ab)^i,\qquad i\geq0.
$$

For any $i\ne j$, append the [word](../../foundations-of-mathematics.md#string) $z_i=(bc)^i$. Then $u_iz_i\in K$, whereas $u_jz_i\notin K$: the latter [word](../../foundations-of-mathematics.md#string) has $j$ occurrences of $a$ and $i$ occurrences of $c$, and every [word](../../foundations-of-mathematics.md#string) of $K$ has equal numbers of those two symbols.

Thus $u_i$ and $u_j$ are not [Myhill-Nerode equivalent](../../foundations-of-mathematics.md#myhill-nerode-equivalence). There are infinitely many [Myhill-Nerode equivalence](../../foundations-of-mathematics.md#myhill-nerode-equivalence) classes, so the [Myhill-Nerode theorem](../../foundations-of-mathematics.md#myhill-nerode-theorem) rules out a [finite-state automaton](../../foundations-of-mathematics.md#finite-state-machine) recognizing $K$. Equivalently, if two such prefixes left a [deterministic finite automaton](../../foundations-of-mathematics.md#deterministic-finite-automaton) in the same [automaton state](../../foundations-of-mathematics.md#automaton-state), appending $z_i$ could not distinguish their acceptance, giving the same contradiction.

$$
\boxed{K\text{ is not regular}.}
$$

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/i">i</h4>

↑ **Parent:** [C](#3/c)

<h5 id="3/c/i/solution">Solution</h5>

↑ **Parent:** [I](#3/c/i)

**The [formal language](../../theoretical-computer-science.md#formal-language) is a [context-free language](../../foundations-of-mathematics.md#context-free-language).** A [context-free grammar](../../foundations-of-mathematics.md#context-free-grammar) with start [nonterminal symbol](../../foundations-of-mathematics.md#nonterminal-symbol) $S$ is

$$
\boxed{S\to AB,\qquad A\to aAb\mid\varepsilon,\qquad B\to bBc\mid\varepsilon.}
$$

The [production rule](../../foundations-of-mathematics.md#production-rule) for $A$ nests one $a$ on the left and one $b$ on the right on each recursive use, so $A$ generates exactly $a^mb^m$ for $m\geq0$. Similarly, $B$ generates exactly $b^nc^n$ for $n\geq0$. The start [production rule](../../foundations-of-mathematics.md#production-rule) concatenates these [words](../../foundations-of-mathematics.md#string), yielding

$$
a^mb^m b^nc^n=a^mb^{m+n}c^n.
$$

Conversely, every choice of nonnegative [integers](../../integer.md) $m,n$ is achieved by using the recursive [production rules](../../foundations-of-mathematics.md#production-rule) exactly $m,n$ times before their [epsilon productions](../../foundations-of-mathematics.md#epsilon-production). Hence this [context-free grammar](../../foundations-of-mathematics.md#context-free-grammar) generates precisely the required [formal language](../../theoretical-computer-science.md#formal-language), including all cases where either count is zero.

<h4 id="3/c/ii">ii</h4>

↑ **Parent:** [C](#3/c)

<h5 id="3/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/c/ii)

**The [formal language](../../theoretical-computer-science.md#formal-language) is not a [context-free language](../../foundations-of-mathematics.md#context-free-language).** Suppose otherwise, and let $p\geq1$ be a [pumping length](../../foundations-of-mathematics.md#pumping-length) from the [pumping lemma for context-free languages](../../foundations-of-mathematics.md#pumping-lemma-for-context-free-languages). Choose

$$
w=a^p b^{p^2}c^p.
$$

This [word](../../foundations-of-mathematics.md#string) belongs to the [formal language](../../theoretical-computer-science.md#formal-language), since its middle exponent is the product of the two outer exponents. The [pumping lemma for context-free languages](../../foundations-of-mathematics.md#pumping-lemma-for-context-free-languages) would give

$$
w=uvxyz,\qquad |vxy|\leq p,\qquad |vy|>0,
$$

with $uv^ixy^iz$ in the [formal language](../../theoretical-computer-science.md#formal-language) for every [integer](../../integer.md) $i\geq0$.

Let $\alpha,\beta,\gamma$ be the respective numbers of $a,b,c$ symbols in the two pumped pieces $v,y$ together. The window $vxy$ cannot contain both an $a$ and a $c$: it would have to contain the entire middle block of length $p^2$, plus at least those two outer symbols, exceeding $p$. Hence

$$
\alpha\gamma=0,\qquad 1\leq\alpha+\beta+\gamma\leq p.
$$

Pump once extra, taking $i=2$. The resulting symbol counts are $p+\alpha$, $p^2+\beta$, and $p+\gamma$. A necessary condition for membership, regardless of whether the block order survives, is

$$
p^2+\beta=(p+\alpha)(p+\gamma),
\quad\text{or equivalently}\quad
\beta=p(\alpha+\gamma),
$$

where $\alpha\gamma=0$ was used.

If $\alpha+\gamma=0$, then $\beta>0$, contradicting that equality. If $\alpha+\gamma\geq1$, then

$$
\beta\leq p-(\alpha+\gamma)<p\leq p(\alpha+\gamma),
$$

again contradicting it. Thus every permissible decomposition fails at $i=2$. This contradicts the [pumping lemma for context-free languages](../../foundations-of-mathematics.md#pumping-lemma-for-context-free-languages) and proves the claim. The obstruction is the [multiplicative block-count language](../../foundations-of-mathematics.md#multiplicative-block-count-language): a bounded local change cannot preserve the product constraint.

$$
\boxed{\{a^m b^{mn}c^n:m,n\geq0\}\text{ is not context-free}.}
$$

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/i">i</h4>

↑ **Parent:** [D](#3/d)

<h5 id="3/d/i/solution">Solution</h5>

↑ **Parent:** [I](#3/d/i)

**The problem is decidable.** We need exactly one accepted [word](../../foundations-of-mathematics.md#string), even if that [word](../../foundations-of-mathematics.md#string) has several accepting runs in the [nondeterministic finite automaton](../../foundations-of-mathematics.md#nondeterministic-finite-automaton).

First convert the input [nondeterministic finite automaton](../../foundations-of-mathematics.md#nondeterministic-finite-automaton) to an equivalent [deterministic finite automaton](../../foundations-of-mathematics.md#deterministic-finite-automaton) $D$ using the [subset construction](../../foundations-of-mathematics.md#subset-construction-with-epsilon-transitions), taking [epsilon closure](../../foundations-of-mathematics.md#epsilon-closure) where necessary. In the finite transition [directed graph](../../graph-theory.md#directed-graph) of $D$, test whether an accepting [automaton state](../../foundations-of-mathematics.md#automaton-state) is reachable from the initial [automaton state](../../foundations-of-mathematics.md#automaton-state). This is the standard [finite automaton emptiness test](../../foundations-of-mathematics.md#finite-automaton-emptiness-test). If none is reachable, the recognized [formal language](../../theoretical-computer-science.md#formal-language) is empty, so answer no.

Otherwise retain a [graph path](../../graph-theory.md#path-in-a-graph) to an accepting [automaton state](../../foundations-of-mathematics.md#automaton-state) and read its labels to obtain one accepted [word](../../foundations-of-mathematics.md#string) $w$. If the initial [automaton state](../../foundations-of-mathematics.md#automaton-state) is accepting, $w$ may be the [empty word](../../foundations-of-mathematics.md#empty-word). Build a complete [deterministic finite automaton](../../foundations-of-mathematics.md#deterministic-finite-automaton) for the [singleton](../../set.md#singleton-mathematics) [formal language](../../theoretical-computer-science.md#formal-language) $\{w\}$: it tracks the matching prefix of $w$, accepts only after exactly its full length, and enters a rejecting sink on a mismatch or any extra input symbol.

Complement that complete [deterministic finite automaton](../../foundations-of-mathematics.md#deterministic-finite-automaton) by exchanging accepting and rejecting [automaton states](../../foundations-of-mathematics.md#automaton-state). Form its product with $D$, accepting exactly when the $D$ coordinate accepts and the other coordinate accepts. This product recognizes

$$
L(D)\cap(\Sigma^*\setminus\{w\})=L(D)\setminus\{w\}.
$$

Apply the [finite automaton emptiness test](../../foundations-of-mathematics.md#finite-automaton-emptiness-test) again. **Answer yes if and only if this difference is empty.** The first test guarantees that $w$ belongs to $L(D)$; the second guarantees there is no different accepted [word](../../foundations-of-mathematics.md#string). All constructions have finitely many [automaton states](../../foundations-of-mathematics.md#automaton-state) and all reachability tests terminate. This gives a [singleton-language test for finite automata](../../foundations-of-mathematics.md#singleton-language-test-for-finite-automata).

$$
\boxed{\text{Decidable: test }L(D)\ne\varnothing\text{ and }L(D)\setminus\{w\}=\varnothing.}
$$

<h4 id="3/d/ii">ii</h4>

↑ **Parent:** [D](#3/d)

<h5 id="3/d/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/d/ii)

**The problem is undecidable.** Reduce the [halting problem](../../foundations-of-mathematics.md#halting-problem) to it. Given a [Turing machine](../../theoretical-computer-science.md#turing-machine) $M$ and input [word](../../foundations-of-mathematics.md#string) $w$, construct a [Turing machine](../../theoretical-computer-science.md#turing-machine) $T$ over $\{a,b,c\}$ with the following behavior on input $x$:

- If $x\ne\varepsilon$, reject.
- If $x=\varepsilon$, simulate $M$ on the fixed [word](../../foundations-of-mathematics.md#string) $w$. If that simulation ever halts, whether accepting or rejecting, accept $x$; otherwise continue the simulation forever.

This is an effective construction: $M,w$ are fixed data stored in the description of $T$. Its recognized [formal language](../../theoretical-computer-science.md#formal-language) is

$$
\boxed{L(T)=\begin{cases}\{\varepsilon\}&M\text{ halts on }w,\\\varnothing&M\text{ does not halt on }w.\end{cases}}
$$

Therefore $T$ accepts exactly one input [word](../../foundations-of-mathematics.md#string) if and only if $M$ halts on $w$. A supposed decision procedure for the [singleton-language problem for Turing machines](../../computability-theory.md#singleton-language-problem-for-turing-machines), applied to the constructed $T$, would decide the [halting problem](../../foundations-of-mathematics.md#halting-problem). The standard undecidability of the [halting problem](../../foundations-of-mathematics.md#halting-problem) excludes that possibility.

$$
\boxed{\text{The singleton-language problem for Turing machines is undecidable}.}
$$

## ↑ Ancestors (8)

1. [2015](../2015.md)
2. [Past exam of the computer science course of the University of Oxford](../../past-exam-of-the-computer-science-course-of-the-university-of-oxford.md)
3. [Computer science course of the University of Oxford](../../university-of-oxford.md#computer-science-course-of-the-university-of-oxford)
4. [Undergraduate course of the University of Oxford](../../university-of-oxford.md#undergraduate-course-of-the-university-of-oxford)
5. [Course of the University of Oxford](../../university-of-oxford.md#course-of-the-university-of-oxford)
6. [University of Oxford](../../university-of-oxford.md)
7. [List of universities](../../README.md#list-of-universities)
8. [Codex Wiki](../../README.md)
