# Round-trip testing

↑ **Parent:** [Software testing](software-testing.md)

Test a conversion together with its intended inverse. Equality of representations may need normalization, while equality of numerical values can be limited by [floating-point rounding](floating-point-rounding.md) or truncation. Distinct [strings](string.md) can encode the same value, so a value round trip and a character-for-character round trip are different properties.

An independent oracle is still needed: the wrong [functions](function-split.md) $f(x)=x+1$ and $g(y)=y-1$ satisfy both composition identities on [integers](integer-split.md), although neither implements an intended identity conversion. Thus passing inverse-consistency tests does not alone establish the specification of either conversion.

## ↑ Ancestors (4)

1. [Software testing](software-testing.md)
2. [Software](software.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/imperative-programming/1/g/solution.md)
