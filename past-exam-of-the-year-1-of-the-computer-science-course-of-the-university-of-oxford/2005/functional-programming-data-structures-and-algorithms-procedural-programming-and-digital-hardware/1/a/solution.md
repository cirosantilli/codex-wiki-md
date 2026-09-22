<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [map function](../../../../../map-higher-order-function.md) transforms each head and recursively processes the tail. A [right fold](../../../../../list-fold.md) combines a head with the result for its tail, whereas a [left fold](../../../../../left-fold.md) passes an updated accumulator into the recursive call. In [Haskell](../../../../../haskell.md):

```
import Prelude hiding (map, foldr, foldl, concat)

map f [] = []
map f (x:xs) = f x : map f xs

foldr op e [] = e
foldr op e (x:xs) = op x (foldr op e xs)

foldl op e [] = e
foldl op e (x:xs) = foldl op (op e x) xs

concat = foldr (++) []
```

The last [right fold](../../../../../list-fold.md) uses [list concatenation](../../../../../list-concatenation.md) to replace each outer cons by appending its inner [list](../../../../../list-abstract-data-type.md). Thus `concat [xs,ys,zs] = xs ++ (ys ++ (zs ++ []))`. Its [right fold](../../../../../list-fold.md) association matters: appending a [list](../../../../../list-abstract-data-type.md) traverses its left spine, so these equations traverse each inner spine once on finite inputs. The concise answer is

$$
\boxed{\operatorname{concat}=\operatorname{foldr}\ (\mathbin{++})\ [].}
$$

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [Functional programming, data structures and algorithms, procedural programming, and digital hardware](../../../functional-programming-data-structures-and-algorithms-procedural-programming-and-digital-hardware-split.md)
4. [2005](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
