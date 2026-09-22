# Injectivity and surjectivity under composition

↑ **Parent:** [Function composition](function-composition.md)

For $f:A\to B$ and $g:B\to C$, the following implications hold. If both are [injective](injective-function.md), equality of two composite images can be cancelled first through $g$ and then through $f$, proving that $g\circ f$ is [injective](injective-function.md). Conversely, if $g\circ f$ is [injective](injective-function.md), equality under $f$ implies equality under the composite, so $f$ is [injective](injective-function.md). If $g\circ f$ is [surjective](surjective-function.md), every $c\in C$ is $g(f(a))$, so $g$ is [surjective](surjective-function.md).

There are two useful strengthened cancellation rules. If $g\circ f$ is [injective](injective-function.md) and $f$ is [surjective](surjective-function.md), lift any $b,b'\in B$ with $g(b)=g(b')$ to preimages under $f$; composite [injectivity](injective-function.md) then proves $b=b'$. If $g\circ f$ is [surjective](surjective-function.md) and $g$ is [injective](injective-function.md), apply composite [surjectivity](surjective-function.md) to $g(b)$ and cancel $g$ to find a preimage of every $b$. Neither strengthened conclusion follows from the composite property alone.

## ↑ Ancestors (7)

1. [Function composition](function-composition.md)
2. [Function](function-split.md)
3. [Set theory](set-theory-split.md)
4. [Foundations of mathematics](foundations-of-mathematics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2023/discrete-mathematics-probability-and-continuous-mathematics/2/d/v/solution.md)
