<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Use a deterministic single-tape [Turing machine](../../../../../turing-machine.md) with finite tape alphabet $A$ containing a blank symbol $B$, and finite control states. Its [instruction of a Turing machine](../../../../../instruction-of-a-turing-machine.md) has the form

$$
\delta(q_i,a)=(q_j,b,D),\qquad a,b\in A,\quad D\in\{L,R,S\}.
$$

It reads $a$, writes $b$, changes state, and moves the head left, right, or stays. An [instantaneous description of a Turing machine](../../../../../instantaneous-description-of-a-turing-machine.md) records the state, scanned position, and tape contents; cells outside the finite recorded window are blank. The initial description places the head at the first input symbol, or at a blank for an empty input. A tape infinite in both directions is used here; extending the recorded window does not change its infinite blank surroundings.

Introduce a dedicated halting state $q_H$ and replace every undefined transition by a stay instruction to $q_H$, retaining the scanned symbol. Give $q_H$ no instructions. This effective normalization changes only the final bookkeeping step, not whether the original machine halts. Keep its initial state $q_1$ and tape alphabet unchanged. State letters, tape letters, and the new symbols $h,q$ are mutually disjoint.

Represent a finite description by the word

$$
C=h\,u\,q_i\,v\,h,\qquad u,v\in A^*.
$$

The head scans the first letter of $v$ if there is one; if $v$ is empty it scans an implicit blank just beyond the recorded right end. The letters of $u$ are in left-to-right order, and the remaining right-hand letters follow the scanned cell. The markers bound a window, not walls of the physical tape. Thus the input is represented exactly by $hq_1wh$, including $w$ empty.

Define the [semigroup simulation of a Turing machine](../../../../../semigroup-simulation-of-a-turing-machine.md) by taking generators $A$, all state letters, $h$, and $q$, with the following finite list of defining equalities. For each ordinary instruction, use its row below; in a left-move row add the first relation for every $c\in A$:

$$
\begin{array}{c|l}
\delta(q_i,a)=(q_j,b,S)&q_i a=q_j b\\
\delta(q_i,a)=(q_j,b,R)&q_i a=bq_j\\
\delta(q_i,a)=(q_j,b,L)&c q_i a=q_jcb,\quad hq_i a=hq_jBb.
\end{array}
$$

These are the cases where a scanned cell is explicitly present. For the instructions reading $B$, add boundary cases when the right-hand word is empty:

$$
\begin{array}{c|l}
\delta(q_i,B)=(q_j,b,S)&q_i h=q_jbh\\
\delta(q_i,B)=(q_j,b,R)&q_i h=bq_jh\\
\delta(q_i,B)=(q_j,b,L)&c q_i h=q_jcbh\ (c\in A),\quad hq_i h=hq_jBbh.
\end{array}
$$

A left move at the recorded left end supplies a new scanned blank $B$; a right move at the right end can keep the next blank implicit. Each equality can be checked by reading the new scanned cell and written symbol. For instance $c q_i a=q_jcb$ leaves the head scanning $c$, with the just-written $b$ to its right. Every transition is one of these local substitutions, including either finite-window boundary case.

Finally add only the terminal cleanup equalities

$$
a q_H=q_H,\quad q_Ha=q_H\quad(a\in A),\qquad hq_Hh=q.
$$

There are finitely many generators and relations, and every side is a nonempty word. Thus these equations define a [finite semigroup presentation](../../../../../finite-semigroup-presentation.md) $\gamma(T)$, not merely a rewriting program. In particular, its equalities may be used in either direction.

If $T$ halts on $w$, the simulated forward computation takes $hq_1wh$ to some $huq_Hvh$. The cleanup relations remove $u$ and $v$, then $hq_Hh=q$. This proves the forward implication.

For the converse, equality in a [semigroup presentation](../../../../../semigroup-presentation.md) is witnessed by a finite sequence of replacements in contexts, in either direction. Before the first cleanup relation is used, every word reached from $hq_1wh$ is still a valid description: it has exactly two outer $h$ markers, exactly one state letter, tape symbols between them, and nothing outside. The transition equalities and their inverses preserve this form. A forward transition sends its interpreted configuration $C$ to its unique successor $D$. Since the machine is deterministic, $C$ eventually halts if and only if $D$ eventually halts. Consequently eventual halting is invariant even when such an equality is traversed backward; no reversibility hypothesis on the machine is needed.

Any first cleanup replacement must already encounter $q_H$. The inverse erasure rules also require $q_H$, and the inverse acceptance rule requires $q$, which cannot appear before an acceptance replacement. Therefore a derivation reaching the one-letter word $q$ first reaches a description in state $q_H$ using only simulation equalities. Halting invariance along this initial part of the derivation implies that the original input configuration halts. Thus

$$
\boxed{hq_1wh=q\text{ in }\gamma(T)\quad\Longleftrightarrow\quad T\text{ halts on }w.}
$$

The converse proof is what prevents arbitrary inverse uses of the defining relations from becoming spurious halting certificates.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 1](../../paper-1-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
