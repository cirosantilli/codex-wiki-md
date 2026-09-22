# Free monoid

↑ **Parent:** [Monoid](monoid.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Free_monoid)

The [free monoid](free-monoid.md) $\Sigma^*$ on an [alphabet](alphabet.md) $\Sigma$ consists of all finite [words over an alphabet](string.md), including the [empty word](empty-word.md) $\varepsilon$, with [concatenation](concatenation.md) as its [binary operation](binary-operation.md). Distinct [strings](string.md) represent distinct elements: there are no imposed equalities between different sequences of letters. The [empty word](empty-word.md) is its [identity element](identity-element.md), and [concatenation](concatenation.md) has the [associative property](associative-property.md).[§2: free monoids](group-theory-v4-01-by-james-s-milne.md)

For $\Sigma=\{a,b\}$, the elements begin $\varepsilon,a,b,aa,ab,ba,bb,\ldots$. Both $(ab)a$ and $a(ba)$ give the same [word](string.md) $aba$, but $ab\ne ba$, so this [monoid](monoid.md) is not [commutative](commutativity.md). The [length of a word over an alphabet](length-of-a-word-over-an-alphabet.md) obeys $\ell(uv)=\ell(u)+\ell(v)$; it is a [monoid homomorphism](monoid-homomorphism.md) to the nonnegative [integers](integer.md) with [addition](addition.md). A nonempty [word](string.md) has no [inverse element](inverse-element.md), since joining it to any other [word](string.md) cannot decrease its length to zero.

The defining benefit of being free is that letters can stand for arbitrary elements of another [monoid](monoid.md). Choose a value $h(a)$ for each letter $a\in\Sigma$; then $h(a_1\cdots a_n)=h(a_1)\ast\cdots\ast h(a_n)$, with $h(\varepsilon)=e$, is the unique [monoid homomorphism](monoid-homomorphism.md) extending those choices. [Associativity](associative-property.md) and the [identity element](identity-element.md) make this evaluation consistent for every finite [word](string.md). For example, interpreting the letters as [self-maps](self-map.md) evaluates a [word](string.md) as a composed transformation; interpreting them as nonnegative counts evaluates it by [addition](addition.md).

## ↑ Ancestors (9)

1. [Monoid](monoid.md)
2. [Semigroup](semigroup.md)
3. [Associative property](associative-property.md)
4. [Binary operation](binary-operation.md)
5. [Algebraic operation](algebraic-operation.md)
6. [Algebra](algebra-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (7)

- [Concatenation](concatenation.md)
- [Exponential growth of SL2 of Z](exponential-growth-of-sl2-of-z.md)
- [Free monoid](free-monoid.md)
- [Monoid](monoid.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-74/4/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-143/3/d/solution.md)
- [Semigroup](semigroup.md)
