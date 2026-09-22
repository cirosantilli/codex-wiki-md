<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use [pattern matching](../../../../../pattern-matching.md) to separate the empty [list](../../../../../list-abstract-data-type.md) from a head and tail. In [Haskell](../../../../../haskell.md), hide the conflicting [Standard Prelude](../../../../../standard-prelude.md) names; the examination's `init` returns _all_ [prefixes of a list](../../../../../prefix-of-a-list.md), unlike the usual [Standard Prelude](../../../../../standard-prelude.md) function of that name.

```
import Prelude hiding (map, length, init, tails, foldr, compare)

map :: (a -> b) -> [a] -> [b]
map f [] = []
map f (x:xs) = f x : map f xs

length :: Num n => [a] -> n
length [] = 0
length (_:xs) = 1 + length xs

copy :: (Eq n, Num n) => n -> a -> [a]
copy 0 xs = []
copy n xs = xs : copy (n-1) xs

combine :: [[a]] -> [[a]] -> [[a]]
combine [] _ = []
combine _ [] = []
combine (xs:xss) (ys:yss) = (xs ++ ys) : combine xss yss

init :: [a] -> [[a]]
init [] = [[]]
init (x:xs) = [] : map (x:) (init xs)

tails :: [a] -> [[a]]
tails [] = [[]]
tails (x:xs) = (x:xs) : tails xs
```

The [map function](../../../../../map-higher-order-function.md) preserves the input [list](../../../../../list-abstract-data-type.md) shape while transforming each entry. `length` counts the cons cells. `copy` repeats the whole value `xs`, so for the specified use its second argument is a [list](../../../../../list-abstract-data-type.md) and the result is a [list](../../../../../list-abstract-data-type.md) of [lists](../../../../../list-abstract-data-type.md). Its inferred type is more general: the repeated value can have any [data type](../../../../../data-type.md). If one restricts the interface to [lists](../../../../../list-abstract-data-type.md), the corresponding type is `(Eq n, Num n) => n -> [a] -> [[a]]`. The numeric argument has the [precondition](../../../../../precondition.md) that it is a nonnegative [integer](../../../../../integer-split.md); the most general inferred numeric constraints do not guarantee termination on arbitrary values of their instances. An explicitly integral interface may instead use `Integral n => n -> [a] -> [[a]]`.

`combine` performs [list concatenation](../../../../../list-concatenation.md) head by head and stops as soon as either outer [list](../../../../../list-abstract-data-type.md) ends. For `init`, every nonempty [prefix of a list](../../../../../prefix-of-a-list.md) starts with `x` and continues with a [prefix of a list](../../../../../prefix-of-a-list.md) from `xs`; prepending `[]` supplies the shortest [prefix of a list](../../../../../prefix-of-a-list.md). For `tails`, the longest [suffix of a list](../../../../../suffix-of-a-list.md) is the whole input, followed by all [suffixes of a list](../../../../../suffix-of-a-list.md) of its tail. For example, `init [1,2] = [[],[1],[1,2]]` and `tails [1,2] = [[1,2],[2],[]]`. Thus both include the empty [list](../../../../../list-abstract-data-type.md), and

$$
\boxed{|\operatorname{init}(xs)|=|\operatorname{tails}(xs)|=|xs|+1.}
$$

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [Functional programming, data structures and algorithms, procedural programming, and digital hardware](../../../functional-programming-data-structures-and-algorithms-procedural-programming-and-digital-hardware-split.md)
4. [2003](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
