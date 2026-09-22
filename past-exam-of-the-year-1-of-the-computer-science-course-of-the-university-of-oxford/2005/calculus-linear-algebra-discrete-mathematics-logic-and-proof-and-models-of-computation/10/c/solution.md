<h1 id="10/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [halting problem](../../../../../halting-problem.md) asks, given the encoding $\langle M,w\rangle$ of a [Turing machine](../../../../../turing-machine.md) and an input [string](../../../../../string.md), whether that machine eventually halts on that input. Its [formal language](../../../../../formal-language.md) is

$$
\operatorname{HALT}=\{\langle M,w\rangle:M\text{ halts on }w\}.
$$

Suppose a [Turing machine](../../../../../turing-machine.md) $H$ decided this [formal language](../../../../../formal-language.md). Construct another [Turing machine](../../../../../turing-machine.md) $D$ that, on an input encoding $\langle M\rangle$, runs $H$ on $\langle M,\langle M\rangle\rangle$. If $H$ answers that $M$ halts on its own encoding, $D$ enters an infinite loop. If $H$ answers that $M$ does not halt, $D$ halts. Handling malformed encodings by immediate rejection makes $D$ well-defined on arbitrary [strings](../../../../../string.md).

Now run $D$ on its own encoding. If $H$ says that $D$ halts, the construction makes $D$ loop; if $H$ says that $D$ does not halt, the construction makes $D$ halt. Either answer contradicts the assumed correctness of $H$. Therefore

$$
\boxed{\operatorname{HALT}\text{ is not a decidable language}.}
$$

The contradiction concerns a decider that must give a correct terminating answer for every encoded machine and input. Simulating $M$ does detect a halt when one occurs, but cannot in general certify that a running computation will continue forever.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [10](../../10.md)
3. [Calculus, linear algebra, discrete mathematics, logic and proof, and models of computation](../../../calculus-linear-algebra-discrete-mathematics-logic-and-proof-and-models-of-computation-split.md)
4. [2005](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
