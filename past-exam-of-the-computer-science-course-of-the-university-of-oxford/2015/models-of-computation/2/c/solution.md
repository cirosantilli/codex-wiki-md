<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

**$P$ is a [co-recursively enumerable language](../../../../../co-recursively-enumerable-language.md), is not a [recursively enumerable language](../../../../../recursively-enumerable-language.md), and is not a [decidable language](../../../../../recursive-language.md).** The stipulated order on halting times includes $\infty\geq\infty$.

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

Enumerate all pairs $(x,t)$ and perform these finite tests by [dovetailing](../../../../../dovetailing.md), accepting the [complement of a set](../../../../../complement-of-a-set.md) of $P$ on finding a witness. Equivalently, at stage $s$, inspect all inputs of length at most $s$ through $s$ transitions. A genuine violation eventually appears; if there is no violation, the procedure never accepts. Malformed descriptions or differing input [alphabets](../../../../../alphabet.md) can be recognized and accepted as nonmembers immediately. Thus the complement is a [recursively enumerable language](../../../../../recursively-enumerable-language.md), proving that $P$ is a [co-recursively enumerable language](../../../../../co-recursively-enumerable-language.md).

For non-enumerability, use the standard result that the [complement of a set](../../../../../complement-of-a-set.md) of the [halting problem](../../../../../halting-problem.md)

$$
H=\{\langle M,w\rangle:M\text{ halts on }w\}
$$

is not a [recursively enumerable language](../../../../../recursively-enumerable-language.md). Given $\langle M,w\rangle$, effectively construct two [Turing machines](../../../../../turing-machine.md) over the same fixed input [alphabet](../../../../../alphabet.md). On every input $x$, let $N_1$ ignore $x$ and simulate $M$ on the fixed [word](../../../../../string.md) $w$, halting precisely when that simulation halts. Let $N_2$ loop forever on every input.

If $M$ does not halt on $w$, both halting times are infinity for every $x$, so the pair belongs to $P$. If $M$ halts on $w$, the first halting time is finite while the second is infinity, so the pair does not belong to $P$. Therefore

$$
\boxed{\langle M,w\rangle\notin H
\quad\Longleftrightarrow\quad
\langle N_1,N_2\rangle\in P.}
$$

This is a [many-one reduction](../../../../../many-one-reduction.md) from non-halting to the [pointwise running-time domination problem](../../../../../pointwise-running-time-domination-problem.md). Were $P$ a [recursively enumerable language](../../../../../recursively-enumerable-language.md), constructing the pair and running its recognizer would recognize non-halting, contradicting the stated result. Hence $P$ is not a [recursively enumerable language](../../../../../recursively-enumerable-language.md). Since every [decidable language](../../../../../recursive-language.md) is a [recursively enumerable language](../../../../../recursively-enumerable-language.md), $P$ is also undecidable.

$$
\boxed{P\text{ is co-R.E., not R.E., and undecidable}.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Models of computation](../../../models-of-computation-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
