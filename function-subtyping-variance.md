# Function subtyping variance

↑ **Parent:** [Function type](function-type.md)

If $A'<:A$ and $B<:B'$, a [function](function-split.md) of type $A\to B$ safely supplies a contract of type $A'\to B'$. Every input permitted by the new contract is already accepted, and every possible returned value meets the weakened result promise. This proves contravariance of inputs and covariance of outputs. Reversing either direction can respectively supply an unsupported input or promise a result more specific than the implementation returns. A language's generic type [object constructor](object-constructor.md) may nevertheless be invariant unless its declaration exposes the appropriate variance.

## ↑ Ancestors (5)

1. [Function type](function-type.md)
2. [Type system](type-system.md)
3. [Programming language](programming-language-split.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)
