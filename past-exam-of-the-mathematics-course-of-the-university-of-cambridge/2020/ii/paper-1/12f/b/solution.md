<h1 id="12f/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [partial recursive functions](../../../../../../computable-function.md) form the smallest class containing the [zero function](../../../../../../zero-function.md), [successor function](../../../../../../successor-function.md), and [projection functions](../../../../../../projection-function.md) and closed under [composition](../../../../../../function-composition-in-recursion-theory.md), [primitive recursion](../../../../../../primitive-recursion.md), and [unbounded minimization](../../../../../../mu-operator.md).

Fix a [register machine](../../../../../../register-machine.md) $P$ with $k$ inputs. By the permitted result, its complete configuration after $t$ steps,

$$
S(\mathbf x,t),
$$

is a [recursive function](../../../../../../total-computable-function.md) of the inputs and time. The predicate $H(\mathbf x,t)$ saying that this configuration is halted is therefore recursive. Its halting time is the partial recursive function

$$
\tau(\mathbf x)=\mu t\,[H(\mathbf x,t)],
$$

where [unbounded minimization](../../../../../../mu-operator.md) is undefined when no halting time exists. Extracting the output register from a configuration is recursive, so

$$
f(\mathbf x)=\operatorname{out}(S(\mathbf x,\tau(\mathbf x)))
$$

is partial recursive. Hence every [partial computable function](../../../../../../computable-function.md) is partial recursive.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [12F](../../12f.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
