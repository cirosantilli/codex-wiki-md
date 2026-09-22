# Multiplicative self-maps of a finite field

↑ **Parent:** [Finite field](finite-field.md)

For a [finite field](finite-field.md) with $q$ elements, exactly $q+1$ [functions](function-split.md) from the field to itself preserve multiplication, without requiring additivity or preservation of the identity. They are the constant-zero map, the constant-one map, and the $q-1$ power maps $x\mapsto x^k$ for $1\le k\le q-1$.

To prove completeness, $f(1)^2=f(1)$ forces $f(1)\in\{0,1\}$ because a field has no [zero divisors](zero-divisor.md). The zero choice forces the constant-zero map. For $f(1)=1$, nonzero elements must map to nonzero elements, and the restriction is a [group homomorphism](group-homomorphism.md) of the cyclic [multiplicative group of a finite field](multiplicative-group-of-a-finite-field.md). Its generator has $q-1$ possible images, giving the $q-1$ power maps on nonzero elements. Setting $f(0)=0$ extends each. The only further possibility is $f(0)=1$, which forces every value to be one. For $q=5$, this gives six maps. These are generally not [field homomorphisms](field-homomorphism.md), because preservation of addition was never required.

## ↑ Ancestors (5)

1. [Finite field](finite-field.md)
2. [Algebra](algebra-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/discrete-mathematics-continuous-mathematics-and-probability/1/e/solution.md)
