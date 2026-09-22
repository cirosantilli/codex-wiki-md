<h1 id="1/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

Use schoolbook multiplication on the digit coefficients:

```
function Mul(a, b: number): number
    new(result, len(a)+len(b))
    for k := 0 to len(result)-1 do
        result[k] := 0
    for i := 0 to len(a)-1 do
        for j := 0 to len(b)-1 do
            result[i+j] := result[i+j] + a[i]*b[j]
    Normal(result)
    return result
```

This is [discrete convolution](../../../../../discrete-convolution.md) of the digit arrays. Expanding the product shows

$$
\operatorname{val}(a)\operatorname{val}(b)=\sum_{i,j}a[i]b[j]\,base^{i+j}=\operatorname{val}(result)
$$

before normalization. Normalization preserves the value and establishes the digit bounds. Allocating fresh storage makes input aliasing harmless. The convolution uses $O(LM)$ coefficient products for input lengths $L,M$. Intermediate products and sums need sufficiently wide or [arbitrary-precision arithmetic](../../../../../arbitrary-precision-arithmetic.md); fitting each normalized digit into a small integer does not alone prevent accumulator overflow.

## ↑ Ancestors (12)

1. [F](../f.md)
2. [1](../../1.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2017](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
