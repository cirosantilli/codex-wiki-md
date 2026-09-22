<h1 id="recaman-s-sequence">Recamán's sequence</h1>

↑ **Parent:** [Integer sequence](integer-sequence.md)

The [integer sequence](integer-sequence.md) proposed by [Bernardo Recamán Santos](bernardo-recaman-santos.md) starts at zero. At step $n>0$, subtract $n$ if the result is positive and has not appeared before; otherwise add $n$. The commonly written nonnegative version gives the same [sequence](sequence.md) because zero is already present. The initial values are $0,1,3,6,2,7,13,20,\ldots$. The addition branch can repeat a value: $r(20)=r(24)=42$. Avoiding a repeated subtraction is therefore not a global injectivity condition.[Definition, initial terms, and comment on the first repeat; correspondence reference dated 29 January 1991](oeis-entry-a005132.md)

Since $r(n)\leq r(n-1)+n$, [induction](mathematical-induction.md) gives $0\leq r(n)\leq n(n+1)/2$. A prefix scan needs only constant extra storage but can take quadratic membership work. A [bitset](bitset.md)-style bounded membership table makes each lookup constant time, while its allocation cost depends on the chosen value universe. This separates the number of generated terms from the range of possible stored values.

## ↑ Ancestors (8)

1. [Integer sequence](integer-sequence.md)
2. [Sequence](sequence.md)
3. [Sequence and series](sequence-and-series-split.md)
4. [Real analysis](real-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Bernardo Recamán Santos](bernardo-recaman-santos.md)
- [OEIS entry A005132](oeis-entry-a005132.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/imperative-programming/3/a/i/solution.md)
