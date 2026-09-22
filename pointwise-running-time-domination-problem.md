# Pointwise running-time domination problem

↑ **Parent:** [Computability theory](computability-theory-split.md)

Give a nonhalting [Turing machine](turing-machine.md) computation halting time infinity. The [formal language](formal-language.md) of pairs satisfying the displayed inequality is a [co-recursively enumerable language](co-recursively-enumerable-language.md) but is not a [recursively enumerable language](recursively-enumerable-language.md). A violation has a finite witness: $N_1$ has halted on some input after $t$ moves while $N_2$ has not halted by that time. For the other direction, reduce non-halting by making $N_1$ simulate a fixed computation on every input and making $N_2$ run forever. The pair satisfies domination exactly when the fixed computation never halts. The convention $\infty\geq\infty$ is essential to this [many-one reduction](many-one-reduction.md).

## ↑ Ancestors (5)

1. [Computability theory](computability-theory-split.md)
2. [Foundations of mathematics](foundations-of-mathematics-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2015/models-of-computation/2/c/solution.md)
