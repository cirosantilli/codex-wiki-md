# Factorial recursion and returning frames

↑ **Parent:** [Recursion (computer science)](recursion-computer-science.md)

For a [natural number](natural-number.md) $n$, the [factorial](factorial.md) satisfies $0!=1$ and $n!=n(n-1)!$ for $n\geq1$. The following description includes the zero [base case](base-case.md) explicitly; a negative or nonintegral [input](input-computer-science.md) is outside its [precondition](precondition.md):
```
F(n):
    require n is an integer and n >= 0
    if n == 0:
        return 1
    child_result = F(n - 1)
    return n * child_result
```
For $n=4$, the arguments on descent are $4,3,2,1,0$. Each positive-argument invocation postpones one [multiplication](multiplication.md) until its [recursive call](recursive-call.md) returns. At the deepest point, the [call stack](call-stack.md) has five [stack frames](stack-frame.md): four suspended callers and the active zero [base case](base-case.md). The invocation at zero returns $1$ to the invocation at one, rather than finishing the entire computation. Returns then give

$$
F(0)=1,\quad F(1)=1\cdot1=1,\quad F(2)=2\cdot1=2,\quad F(3)=3\cdot2=6,\quad F(4)=4\cdot6=24.
$$

A [stack frame](stack-frame.md) retains the caller's argument and where to resume. When the invocation at three receives $2$, it uses its own $n=3$, obtains $6$, and returns that value to the invocation at four. The [recursive calls](recursive-call.md) share a definition, but their local [variables](variable-mathematics.md) belong to separate invocations.

<a id="image-factorial-descent-builds-pending-work-returning-frames-complete-it"></a>
![](recursion-factorial-returning-frames.png)

**[Figure 14](#image-factorial-descent-builds-pending-work-returning-frames-complete-it). Factorial descent builds pending work; returning frames complete it**. Original trace of $F(4)$ with [base case](base-case.md) $F(0)=1$. The central snapshot shows all five [stack frames](stack-frame.md) at maximum depth. Downward arrows create [recursive calls](recursive-call.md); upward arrows carry completed answers to suspended callers. A return removes only the completed invocation's [stack frame](stack-frame.md).

The [natural number](natural-number.md) measure $n$ decreases by one on every [recursive call](recursive-call.md), so [algorithm termination](algorithm-termination.md) follows. For [algorithm correctness](algorithm-correctness.md), use [mathematical induction](mathematical-induction.md): the zero [base case](base-case.md) returns $0!=1$; assuming the child's answer is $(n-1)!$, the caller returns $n(n-1)!=n!$. This also explains why keeping the caller's $n$ matters.

There are exactly $n+1$ invocations and $n$ [multiplications](multiplication.md), including one invocation and no [multiplications](multiplication.md) when $n=0$. Ordinary execution of this [recursive process](recursive-process.md) uses at most $n+1$ active [stack frames](stack-frame.md), hence $O(n)$ frames for $n\geq1$ in [Big O notation](big-o-notation.md). If each test, call, [subtraction](subtraction.md) and [multiplication](multiplication.md) is counted as constant cost, its [time complexity](time-complexity.md) is $O(n)$. That is an arithmetic-operation model: exact arbitrary-length [integer](integer-split.md) [multiplication](multiplication.md) has growing cost, and neither the [factorial](factorial.md) [output](output-computing.md) nor every [stack frame](stack-frame.md)'s numeric contents occupies a universally fixed number of [bits](bit.md).

## ↑ Ancestors (4)

1. [Recursion (computer science)](recursion-computer-science.md)
2. [Algorithm](algorithm-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)
