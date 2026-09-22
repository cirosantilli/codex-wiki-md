# Kleene normal form theorem

↑ **Parent:** [Computable function](computable-function.md)

For every [partial computable function](computable-function.md) $f(\mathbf x)$, there are total [primitive recursive functions](primitive-recursive-function.md) $C,U$ such that

$$
f(\mathbf x)=U(\mu s\,[C(\mathbf x,s)=0]).
$$

Here $C$ is zero exactly on codes of valid halting computation histories for the chosen program and input, and $U$ extracts the final output. Coding finite configurations and finite histories makes checking every local step a bounded primitive recursive operation. If a computation halts, some history code passes and every passing code has the same output; if it does not halt, none passes. This is the usual normal-form version with the program index fixed; a universal predicate can also retain that index as an input.

## ↑ Ancestors (6)

1. [Computable function](computable-function.md)
2. [Computability theory](computability-theory.md)
3. [Foundations of mathematics](foundations-of-mathematics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (6)

- [Lambda representation of partial computable functions](lambda-representation-of-partial-computable-functions.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-76/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-25/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-20/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-120/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-135/6/solution.md)
