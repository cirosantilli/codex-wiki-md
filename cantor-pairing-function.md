# Cantor pairing function

↑ **Parent:** [Countable set](countable-set.md)

The Cantor pairing function is an explicit [bijection](bijection.md) between $\mathbb N^2$ and $\mathbb N$, with the [natural numbers](natural-number.md) numbered from zero:

$$
\pi(x,y)=\frac{(x+y)(x+y+1)}2+y.
$$

If $d=x+y$, there are $1+2+\cdots+d=d(d+1)/2$ pairs on earlier diagonals, and the pair $(x,y)$ is at offset $y$ along diagonal $d$. The formula therefore gives exactly the enumeration above. For example, $\pi(2,3)=5\cdot6/2+3=18$.

For the inverse at an index $k$, find the unique $d$ satisfying $d(d+1)/2\leq k<(d+1)(d+2)/2$, then put $y=k-d(d+1)/2$ and $x=d-y$. At $k=18$, these are $d=5$, $y=3$, and $x=2$. Thus both the encoding and decoding are explicit. The [bijection](bijection.md) is useful for assigning a single [natural number](natural-number.md) to a pair of indices, and iterating it does the same for fixed-length [tuples](finite-tuple.md).

## ↑ Ancestors (7)

1. [Countable set](countable-set.md)
2. [Cardinal number](cardinal-number.md)
3. [Set theory](set-theory-split.md)
4. [Foundations of mathematics](foundations-of-mathematics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (18)

- [Cantor's diagonal argument](cantor-s-diagonal-argument.md)
- [Countable set](countable-set.md)
- [Countable union of explicitly ordered finite lists without choice](countable-union-of-explicitly-ordered-finite-lists-without-choice.md)
- [Foundations of mathematics](foundations-of-mathematics-split.md)
- [Pairing function](pairing-function.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ia/paper-4/5c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ia/paper-4/8e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ia/paper-4/5d/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-83/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/ia/paper-4/7e/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ia/paper-4/8e/b/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ia/paper-4/8e/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-135/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ia/paper-2/8d/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ia/paper-4/8e/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ia/paper-4/8f/b/i/solution.md)
- [Primitive recursive pairing function](primitive-recursive-pairing-function.md)
- [Set theory](set-theory-split.md)
