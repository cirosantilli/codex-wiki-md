# Array rotation

↑ **Parent:** [Array (data structure)](array-data-structure.md)

A right [array rotation](array-rotation.md) by $k$ sends the entry originally at offset $j$ to offset $(j+k)\bmod n$ for nonempty length $n$. Equivalently it changes adjacent blocks $AB$ into $BA$ when $|B|=k$. Identity rotations include $k=0$ and $k=n$.

Three reversals implement the operation: $AB\to A^RB\to A^RB^R\to BA$. Alternatively repeatedly use a [block swap](block-swap.md) to put the smaller block in its final position and recurse on the remaining unresolved segment. Replacing that tail recursion by parameter updates gives constant auxiliary storage. If $S(a,b)$ counts swaps for blocks of lengths $a,b>0$, then $S(a,a)=a$ and $S(a,b)=\min(a,b)+S(\min(a,b),|a-b|)$ for unequal lengths. The [Euclidean algorithm](euclidean-algorithm.md) shows by [induction](mathematical-induction.md) that $S(a,b)=a+b-\gcd(a,b)$, so a right rotation uses $n-\gcd(n,k)$ element swaps for $0<k<n$.

## ↑ Ancestors (4)

1. [Array (data structure)](array-data-structure.md)
2. [Data structure](data-structure-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Array rotation](array-rotation.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2015/imperative-programming-resit/3/f/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2016/imperative-programming/4/c/i/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2016/imperative-programming/4/c/iii/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2016/imperative-programming/4/c/iv/solution.md)
