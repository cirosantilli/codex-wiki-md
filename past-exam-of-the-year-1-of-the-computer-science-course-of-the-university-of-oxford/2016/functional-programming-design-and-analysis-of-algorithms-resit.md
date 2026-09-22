# Functional programming, design and analysis of algorithms (resit)

↑ **Parent:** [2016](../2016.md)

Source paper: [released examination archive](https://www.whatdotheyknow.com/request/past_exam_papers_for_1st_year_of/response/1398416/attach/2/Fakour%20Zip%20Final%201.zip?cookie_passthrough=1), member `a10097w1-2.pdf`; original cover dated 2016-09-16.

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
  - [d](#1/d)
    - [Solution](#1/d/solution)
  - [e](#1/e)
    - [Solution](#1/e/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
  - [d](#2/d)
    - [Solution](#2/d/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
  - [d](#3/d)
    - [Solution](#3/d/solution)
  - [e](#3/e)
    - [Solution](#3/e/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)
  - [d](#4/d)
    - [Solution](#4/d/solution)
  - [e](#4/e)
    - [Solution](#4/e/solution)
  - [f](#4/f)
    - [Solution](#4/f/solution)
  - [g](#4/g)
    - [Solution](#4/g/solution)
  - [h](#4/h)
    - [Solution](#4/h/solution)
- [5](#5)
  - [a](#5/a)
    - [Solution](#5/a/solution)
  - [b](#5/b)
    - [Solution](#5/b/solution)
  - [c](#5/c)
    - [Solution](#5/c/solution)
  - [d](#5/d)
    - [Solution](#5/d/solution)
  - [e](#5/e)
    - [Solution](#5/e/solution)
  - [f](#5/f)
    - [Solution](#5/f/solution)
- [6](#6)
  - [a](#6/a)
    - [Solution](#6/a/solution)
  - [b](#6/b)
    - [Solution](#6/b/solution)
  - [c](#6/c)
    - [Solution](#6/c/solution)
  - [d](#6/d)
    - [Solution](#6/d/solution)
  - [e](#6/e)
    - [Solution](#6/e/solution)
  - [f](#6/f)
    - [Solution](#6/f/solution)
- [7](#7)
  - [a](#7/a)
    - [Solution](#7/a/solution)
  - [b](#7/b)
    - [Solution](#7/b/solution)
  - [c](#7/c)
    - [Solution](#7/c/solution)
  - [d](#7/d)
    - [Solution](#7/d/solution)
  - [e](#7/e)
    - [Solution](#7/e/solution)
- [8](#8)
  - [a](#8/a)
    - [Solution](#8/a/solution)
  - [b](#8/b)
    - [i](#8/b/i)
      - [Solution](#8/b/i/solution)
    - [ii](#8/b/ii)
      - [Solution](#8/b/ii/solution)
    - [iii](#8/b/iii)
      - [Solution](#8/b/iii/solution)
  - [c](#8/c)
    - [Solution](#8/c/solution)
  - [d](#8/d)
    - [Solution](#8/d/solution)

## 1

↑ **Parent:** [Functional programming, design and analysis of algorithms (resit)](functional-programming-design-and-analysis-of-algorithms-resit.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

The [Haskell](../../programming-language.md#haskell) [type signatures](../../programming-language.md#type-signature) are **`take :: Int -> [a] -> [a]` and `drop :: Int -> [a] -> [a]`**. These definitions also handle nonpositive counts as the Prelude does:
```
take n _ | n <= 0 = []
take _ [] = []
take n (x:xs) = x : take (n-1) xs

drop n xs | n <= 0 = xs
drop _ [] = []
drop n (_:xs) = drop (n-1) xs
```
The wildcard in the first equation matters under [lazy evaluation](../../programming-language.md#lazy-evaluation): `take 0 undefined` yields `[]` without inspecting its [list](../../data-structure.md#list-abstract-data-type) argument. The remainder of this question uses nonnegative counts.[§9, Standard Prelude, definitions and types of take and drop](../../computer-science-bibliography.md#haskell-2010-language-report)

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

For finite, defined [lists](../../data-structure.md#list-abstract-data-type), [structural induction](../../foundations-of-mathematics.md#structural-induction) requires $P([])$ and $P(xs)\Rightarrow P(x:xs)$ for every head $x$ and tail $xs$. This proves $P$ for every finite [list](../../data-structure.md#list-abstract-data-type).

An infinite [list](../../data-structure.md#list-abstract-data-type) cannot be reached by finitely many constructor steps. For [structural induction on lazy lists](../../foundations-of-mathematics.md#structural-induction-on-lazy-lists), also check $P(\bot)$, where $\bot$ is the [bottom value](../../programming-language.md#bottom-value), and require an [admissible predicate on lazy lists](../../foundations-of-mathematics.md#admissible-predicate-on-lazy-lists): if increasingly defined finite approximations all satisfy $P$, their limit does too. Together with the empty-list and constructor cases this covers finite, partial and infinite [lists](../../data-structure.md#list-abstract-data-type). Merely asserting the two finite-list cases is insufficient; “the list is finite” itself satisfies those cases but fails on infinite lists.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Use [mathematical induction](../../foundations-of-mathematics.md#mathematical-induction) on $n$, which is finite even when the [list](../../data-structure.md#list-abstract-data-type) is infinite. At $n=0$, the left side is `[] ++ xs = xs`. For the successor step, an empty [list](../../data-structure.md#list-abstract-data-type) gives `[]`; for `x:xs`, the defining equations and [list concatenation](../../data-structure.md#list-concatenation) give
```
take (n+1) (x:xs) ++ drop (n+1) (x:xs)
= (x : take n xs) ++ drop n xs
= x : (take n xs ++ drop n xs)
= x : xs
```
The last step applies the [induction hypothesis](../../foundations-of-mathematics.md#induction-hypothesis) to the tail. A [bottom value](../../programming-language.md#bottom-value) tail is allowed: for a wholly undefined list and a positive count both sides are undefined. Thus the equality is observationally valid for finite and infinite [lists](../../data-structure.md#list-abstract-data-type); no evaluation of an infinite length is used.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

For finite [lists](../../data-structure.md#list-abstract-data-type) and $n\geq0$, the answers are
```
reverse (xs ++ ys) = reverse ys ++ reverse xs
length (drop n xs) = max 0 (length xs - n)
```
The maximum is necessary when the count exceeds the [list](../../data-structure.md#list-abstract-data-type) length.

<h3 id="1/e">e</h3>

↑ **Parent:** [1](#1)

<h4 id="1/e/solution">Solution</h4>

↑ **Parent:** [E](#1/e)

Write `u = take n xs`, `v = drop n xs`, and `len = length xs`. Part (c) gives `xs = u ++ v`; part (d) gives `length v = len-n` because $0\leq n\leq\mathrm{len}$. Use the finite-[list](../../data-structure.md#list-abstract-data-type) laws `take (length v) (v ++ w) = v`, `length (reverse v) = length v`, and `reverse (reverse v) = v`. Then [equational reasoning](../../foundations-of-mathematics.md#equational-reasoning) gives
```
reverse (take (len-n) (reverse xs))
= reverse (take (length v) (reverse (u ++ v)))
= reverse (take (length (reverse v)) (reverse v ++ reverse u))
= reverse (reverse v)
= v
= drop n xs
```
The first and second steps use the decomposition and the length equation; the third uses reversal of a concatenation; the fourth uses the stated take law. This is an algebraic proof using established laws, rather than a new [induction](../../foundations-of-mathematics.md#mathematical-induction) proof.

## 2

↑ **Parent:** [Functional programming, design and analysis of algorithms (resit)](functional-programming-design-and-analysis-of-algorithms-resit.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

All three [Haskell](../../programming-language.md#haskell) definitions have **`filter :: (a -> Bool) -> [a] -> [a]`**. A recursive [list filter](../../programming-language.md#list-filter) is
```
filter p [] = []
filter p (x:xs)
  | p x       = x : filter p xs
  | otherwise = filter p xs
```
A [list comprehension](../../programming-language.md#list-comprehension) gives `filter p xs = [x | x <- xs, p x]`. A [right fold](../../programming-language.md#list-fold) gives
```
filter p = foldr (\x ys -> if p x then x:ys else ys) []
```
Each version retains the input order and needs no [equality](../../set-theory.md#equality-mathematics) or [Haskell Ord class](../../programming-language.md#haskell-ord-class) constraint on the element type.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Use [merge sort](../../algorithm.md#merge-sort), then project the second component of each [pair](../../set.md#pair). Under the ordinary [Haskell Ord class](../../programming-language.md#haskell-ord-class) instance for pairs, “ascending” means [lexicographic order](../../extremal-set-theory.md#lexicographic-order), requiring both component types to be ordered:
```
sort :: (Ord a, Ord b) => [(a,b)] -> [b]
sort = map snd . mergeSort

mergeSort :: Ord a => [a] -> [a]
mergeSort [] = []
mergeSort [x] = [x]
mergeSort xs = merge (mergeSort left) (mergeSort right)
  where (left,right) = splitAt (length xs `div` 2) xs

merge :: Ord a => [a] -> [a] -> [a]
merge [] ys = ys
merge xs [] = xs
merge (x:xs) (y:ys)
  | x <= y    = x : merge xs (y:ys)
  | otherwise = y : merge (x:xs) ys
```
If the intended convention is to sort only by the first component as a [sort key](../../algorithm.md#sort-key), replace `x <= y` by `fst x <= fst y` and specialize the merge routines to pairs. The weaker signature is then `sort :: Ord a => [(a,b)] -> [b]`, and equal keys keep their original order. These conventions differ when first components tie; the question does not explicitly specify that tie rule.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Merging two sorted [lists](../../data-structure.md#list-abstract-data-type) consumes one head per comparison and takes $O(n)$ time in their combined length, assuming constant-cost comparisons. Computing the length and splitting also takes $O(n)$ time. The balanced [recursion](../../algorithm.md#recursion-computer-science) therefore satisfies

$$
T(n)=T(\lfloor n/2\rfloor)+T(\lceil n/2\rceil)+O(n),\qquad T(0),T(1)=O(1).
$$

Each recursion level has total linear work, and there are $O(\log n)$ levels. Thus [merge sort](../../algorithm.md#merge-sort) takes $O(n\log n)$ worst-case time. The final `map snd` adds $O(n)$, preserving the bound. Costs of comparing variable-size keys must be included separately.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

All three denote **`iterate :: (a -> a) -> a -> [a]`**, producing $x,g(x),g^2(x),\ldots$. With [lazy evaluation](../../programming-language.md#lazy-evaluation), demanding and fully evaluating the first $n$ elements costs **$\Theta(n)$ for `f1` and `f2`, and $\Theta(n^2)$ worst-case for `f3`**, under the unit-cost application assumption.

In `f1` the next state is obtained with one new application of `g`. In `f2`, the shared binding `xs` points back to the already generated [list](../../data-structure.md#list-abstract-data-type); each new element maps `g` over a shared predecessor once. In `f3`, the recursive `f3 g x` is a fresh computation. Producing output position $j$ passes through $j$ separately constructed map layers, so a strict `g` causes $0+1+\cdots+(n-1)$ applications. A non-strict function such as `const 0` can avoid work, so the quadratic statement is a worst-case evaluation bound, not a lower bound for every possible `g`. Merely demanding the outer list spine without its elements is a different cost question.

## 3

↑ **Parent:** [Functional programming, design and analysis of algorithms (resit)](functional-programming-design-and-analysis-of-algorithms-resit.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Map over the optional payload, preserving failure:
```
mapMaybe :: (a -> b) -> Maybe a -> Maybe b
mapMaybe _ Nothing = Nothing
mapMaybe f (Just x) = Just (f x)
```
This is the optional-value mapping operation, equivalent to `fmap` for `Maybe`. The question's local name is distinct from the library function `Data.Maybe.mapMaybe`, which filters and maps an entire [list](../../data-structure.md#list-abstract-data-type). The [algebraic data type](../../programming-language.md#algebraic-data-type) keeps absence separate from every ordinary payload value.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

The most general [type signature](../../programming-language.md#type-signature) is **`foldMaybe :: (a -> b) -> b -> Maybe a -> b`**. The `Nothing` branch returns the default of type `b`; the `Just` branch applies the supplied function to an `a`, also producing a `b`.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Separate the maximal decimal prefix from the unconsumed suffix, rejecting an empty prefix:
```
import Data.Char (isDigit, digitToInt)

type Parse a = String -> Maybe (a,String)

parseInt :: Parse Int
parseInt input =
  case span isDigit input of
    ([],_)  -> Nothing
    (ds,ys) -> Just (foldl (\n d -> 10*n + digitToInt d) 0 ds, ys)
```
The [left fold](../../programming-language.md#left-fold) uses the [positional notation](../../integer.md#positional-notation) recurrence $N_{j+1}=10N_j+d_j$. This parses unsigned decimal operands as illustrated, leaving the first nondigit and everything after it untouched. As the required result type is `Int`, correct mathematical values require the parsed integer to fit that bounded type; arbitrary-length exact values would instead need `Integer` or an explicit [integer overflow](../../programming-language.md#integer-overflow) check.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

The parser recognizes exactly one leading operator character:
```
parseOp :: Parse Char
parseOp (c:cs)
  | c `elem` "+-*/" = Just (c,cs)
parseOp _ = Nothing
```
An empty input fails, and any later characters remain for the next parser. The last example printed in this part uses the name `parseInt`; its failure result does not change the requested operator parser.

<h3 id="3/e">e</h3>

↑ **Parent:** [3](#3)

<h4 id="3/e/solution">Solution</h4>

↑ **Parent:** [E](#3/e)

Compose the three parsing stages using the supplied [fold](../../planetary-science.md#fold), and accept only when no suffix remains:
```
eval :: String -> Maybe Int
eval input = foldMaybe first Nothing (parseInt input)
  where
    first (a,rest) = foldMaybe (second a) Nothing (parseOp rest)
    second a (op,rest) = foldMaybe (finish a op) Nothing (parseInt rest)
    finish a op (b,rest)
      | null rest = Just (apply op a b)
      | otherwise = Nothing
    apply '+' a b = a+b
    apply '-' a b = a-b
    apply '*' a b = a*b
    apply '/' a b = a `div` b
    apply _ _ _ = error "unreachable: parseOp rejected this operator"
```
Every failed intermediate [parser](../../programming-language.md#parser) is converted to `Nothing` by `foldMaybe`. Checking `null rest` rejects both a second operation and trailing letters. In particular, integer division makes `eval "34/4" = Just 8`. As permitted by the question, division by zero is outside the specified inputs; the bounded-`Int` proviso also applies to arithmetic results.

## 4

↑ **Parent:** [Functional programming, design and analysis of algorithms (resit)](functional-programming-design-and-analysis-of-algorithms-resit.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

A [type synonym](../../programming-language.md#type-synonym) is a name for an existing type expression, introduced with `type`, for example `type Name = String`. It improves documentation and makes type signatures easier to maintain. It creates **no new distinct type**: a synonym and its expansion remain interchangeable. An [algebraic data type](../../programming-language.md#algebraic-data-type) declared with `data` or `newtype` has a different role.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Use
```
type Point = (Double,Double)
type Polygon = [Point]
```
A valid [polygon](../../euclidean-geometry.md#polygon) is a finite list of at least three [vertices](../../graph.md#vertex-graph-theory) in boundary order, with the final vertex connected back to the first. The first vertex is not repeated at the end. A simple [polygon](../../euclidean-geometry.md#polygon) also has no intersecting nonadjacent [edges](../../graph-theory.md#edge-of-a-graph). Numerical routines below use finite coordinates; `NaN` and infinite coordinates are outside this representation's intended domain.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

The [Euclidean distance](../../topological-analysis.md#euclidean-distance) is
```
distBetween :: Point -> Point -> Double
distBetween (x,y) (u,v) = sqrt ((x-u)^2 + (y-v)^2)
```
Thus $d((x,y),(u,v))=\sqrt{(x-u)^2+(y-v)^2}$. The type synonym expands to pairs of floating-point coordinates.

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

First include the closing [edge](../../graph-theory.md#edge-of-a-graph) exactly once:
```
edges :: Polygon -> [(Point,Point)]
edges [] = []
edges ps = zip ps (tail ps ++ [head ps])

perimeter :: Polygon -> Double
perimeter = total . edges
  where total [] = 0
        total ((p,q):es) = distBetween p q + total es

perimeterFold :: Polygon -> Double
perimeterFold = foldr (\(p,q) s -> distBetween p q + s) 0 . edges
```
The recursive version and [right fold](../../programming-language.md#list-fold) both sum the [Euclidean distances](../../topological-analysis.md#euclidean-distance) between consecutive [vertices](../../graph.md#vertex-graph-theory), including the last-to-first pair. They take [linear time](../../theoretical-computer-science.md#linear-time). The empty-list convention gives zero, although an empty list is not a valid [polygon](../../euclidean-geometry.md#polygon).

<h3 id="4/e">e</h3>

↑ **Parent:** [4](#4)

<h4 id="4/e/solution">Solution</h4>

↑ **Parent:** [E](#4/e)

Equal side lengths alone are insufficient: a nonsquare rhombus is not a [regular polygon](../../euclidean-geometry.md#regular-polygon). Use the [regular polygon edge rotation criterion](../../euclidean-geometry.md#regular-polygon-edge-rotation-criterion): for $n\geq3$, successive nonzero [edge vectors](../../vector-space.md#edge-vector) must be related by the same [rotation](../../riemannian-geometry.md#rotation-mathematics) through either $2\pi/n$ or $-2\pi/n$.
```
regular :: Polygon -> Bool
regular ps
  | length ps < 3 = False
  | otherwise = norm2 (head es) > 0 && (fits 1 || fits (-1))
  where
    es = [ (u-x,v-y) | ((x,y),(u,v)) <- edges ps ]
    angle = 2*pi / fromIntegral (length ps)
    norm2 (x,y) = x*x+y*y
    close x y = abs (x-y) <= 1e-10 * max 1 (max (abs x) (abs y))
    same (x,y) (u,v) = close x u && close y v
    turn s (x,y) = (cos angle*x - s*sin angle*y,
                    s*sin angle*x + cos angle*y)
    fits s = and (zipWith (\a b -> same (turn s a) b)
                          es (tail es ++ [head es]))
```
With exact real coordinates and exact equality in `same`, this is an if-and-only-if test for an ordinary convex [regular polygon](../../euclidean-geometry.md#regular-polygon), in either boundary orientation. The displayed `Double` implementation tests that condition to the stated tolerance; it cannot promise exact geometric classification near the tolerance boundary. Both orientations are needed, and using the fundamental turn $2\pi/n$ excludes regular star traversals. A repeated zero-length side fails the exact criterion.

<h3 id="4/f">f</h3>

↑ **Parent:** [4](#4)

<h4 id="4/f/solution">Solution</h4>

↑ **Parent:** [F](#4/f)

Here “centroid” means the **[vertex centroid](../../euclidean-geometry.md#vertex-centroid)**, the arithmetic mean of the listed [vertices](../../graph.md#vertex-graph-theory), rather than the uniform-area [centroid](../../euclidean-geometry.md#centroid) of the polygon's interior:
```
centroid :: Polygon -> Point
centroid [] = error "centroid: empty vertex list"
centroid ps = (sx/n,sy/n)
  where
    (sx,sy) = foldr (\(x,y) (u,v) -> (x+u,y+v)) (0,0) ps
    n = fromIntegral (length ps)
```
The nonempty input restriction prevents division by zero; computing both sums and the length takes [linear time](../../theoretical-computer-science.md#linear-time).

<h3 id="4/g">g</h3>

↑ **Parent:** [4](#4)

<h4 id="4/g/solution">Solution</h4>

↑ **Parent:** [G](#4/g)

Apply the same [translation](../../geometry-and-topology.md#translation-geometry) to every [vertex](../../graph.md#vertex-graph-theory):
```
translate :: Point -> Polygon -> Polygon
translate (u,v) = map (\(x,y) -> (x+u,y+v))
```
Every [edge vector](../../vector-space.md#edge-vector) is unchanged because the added displacement cancels on subtraction. Hence lengths, angles, orientation and shape are preserved.

<h3 id="4/h">h</h3>

↑ **Parent:** [4](#4)

<h4 id="4/h/solution">Solution</h4>

↑ **Parent:** [H](#4/h)

Translate the [vertex centroid](../../euclidean-geometry.md#vertex-centroid) to the origin, rotate, and translate back:
```
rotatePoly :: Polygon -> Double -> Polygon
rotatePoly ps theta =
  (translate c . map turn . translate (-cx,-cy)) ps
  where
    c@(cx,cy) = centroid ps
    turn (x,y) = (cos theta*x + sin theta*y,
                 -sin theta*x + cos theta*y)
```
This follows the supplied [rotation matrix](../../linear-algebra.md#rotation-matrix), so **positive $\theta$ rotates clockwise** in the usual Cartesian axes. The opposite signs give the conventional counterclockwise matrix. Since the [vertex centroid](../../euclidean-geometry.md#vertex-centroid) of the centered vertices is zero and a [linear map](../../vector-space.md#linear-map) commutes with their average, the final centroid remains `c`.

## 5

↑ **Parent:** [Functional programming, design and analysis of algorithms (resit)](functional-programming-design-and-analysis-of-algorithms-resit.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

A [connected component](../../geometry-and-topology.md#connected-component) of an [undirected graph](../../graph-theory.md#undirected-graph) is a maximal set of [vertices](../../graph.md#vertex-graph-theory) such that each pair is joined by a [path](../../geometry-and-topology.md#continuous-path). Equivalently, components are the [equivalence classes](../../set-theory.md#equivalence-class) of the relation “reachable by a path”. The length-zero path ensures that an isolated [vertex](../../graph.md#vertex-graph-theory) is a one-vertex component.

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

Start a [depth-first search](../../algorithm.md#depth-first-search) from each as-yet unlabelled [vertex](../../graph.md#vertex-graph-theory), propagating a fresh component number:
```
component = 0
for u in V:
    cc[u] = UNLABELLED
for u in V:
    if cc[u] == UNLABELLED:
        visit(u, component)
        component = component + 1

visit(u, label):
    cc[u] = label
    for v in adjacency[u]:
        if cc[v] == UNLABELLED:
            visit(v, label)
```
A search follows only [edges](../../graph-theory.md#edge-of-a-graph), so every vertex it labels is reachable from its root. Conversely, if a reachable vertex remained unlabelled, a path to it would contain a first edge from a visited vertex to an unvisited one; scanning that edge would visit the latter, a contradiction. Thus each search labels exactly one [connected component](../../geometry-and-topology.md#connected-component), proving both directions of the required equivalence.

<h3 id="5/c">c</h3>

↑ **Parent:** [5](#5)

<h4 id="5/c/solution">Solution</h4>

↑ **Parent:** [C](#5/c)

With an [adjacency list](../../data-structure.md#adjacency-list), initialization and the outer loop cost $O(|V|)$. Each [vertex](../../graph.md#vertex-graph-theory) is visited once, and the adjacency scans inspect each [edge of a graph](../../graph-theory.md#edge-of-a-graph) twice, once from each endpoint. The total worst-case time is therefore **$O(|V|+|E|)$**, with $O(|V|)$ labels and recursion-stack space. An [adjacency matrix](../../graph-theory.md#adjacency-matrix) representation instead incurs $O(|V|^2)$ scanning time.

<h3 id="5/d">d</h3>

↑ **Parent:** [5](#5)

<h4 id="5/d/solution">Solution</h4>

↑ **Parent:** [D](#5/d)

A [disjoint-set data structure](../../data-structure.md#disjoint-set-data-structure) maintains a [partition of a set](../../set.md#partition-of-a-set) into pairwise disjoint sets. `Make-Set(v)` creates the singleton containing a new vertex. `Find-Set(v)` returns the [disjoint-set representative](../../data-structure.md#disjoint-set-representative) of its current set. `Union(u,v)` merges the two sets containing its arguments, preserving the partition; it has no effect if they are already the same set. A [disjoint-set forest](../../data-structure.md#disjoint-set-forest) can implement these operations without explicitly moving every member when sets are joined.

<h3 id="5/e">e</h3>

↑ **Parent:** [5](#5)

<h4 id="5/e/solution">Solution</h4>

↑ **Parent:** [E](#5/e)

Test **`Find-Set(u) == Find-Set(v)`**. Initially the sets are singleton [connected components](../../geometry-and-topology.md#connected-component) of the edgeless graph; processing an edge joins precisely the components it connects. By [induction](../../foundations-of-mathematics.md#mathematical-induction) over the processed edges, the final sets are exactly the [connected components](../../geometry-and-topology.md#connected-component) of $G$.

<h3 id="5/f">f</h3>

↑ **Parent:** [5](#5)

<h4 id="5/f/solution">Solution</h4>

↑ **Parent:** [F](#5/f)

The displayed procedure calls `Find-Set` **$2|E|$ times explicitly**, since it tests the two endpoints of every edge. Each successful `Union` decreases the number of sets by one, from $|V|$ initially to $k$ finally, so **there are $|V|-k$ `Union` calls**.

These are calls at the displayed pseudocode level. If a concrete `Union(u,v)` implementation performs two further internal finds rather than accepting already found roots, its implementation adds $2(|V|-k)$ find invocations. Counting those separately avoids confusing the procedure's explicit call count with the implementation of a [disjoint-set union operation](../../data-structure.md#disjoint-set-union-operation).

## 6

↑ **Parent:** [Functional programming, design and analysis of algorithms (resit)](functional-programming-design-and-analysis-of-algorithms-resit.md)

<h3 id="6/a">a</h3>

↑ **Parent:** [6](#6)

<h4 id="6/a/solution">Solution</h4>

↑ **Parent:** [A](#6/a)

Use [merge sort](../../algorithm.md#merge-sort): recursively sort the left and right halves of the [array](../../data-structure.md#array-data-structure), then merge their ordered outputs using two advancing indices. A merge reads or writes each element a constant number of times, so it costs $O(n)$. There are $O(\log n)$ balanced recursion levels with $O(n)$ total work per level. Hence the worst-case running time is **$O(n\log n)$**; the standard array implementation uses $O(n)$ auxiliary storage.

<h3 id="6/b">b</h3>

↑ **Parent:** [6](#6)

<h4 id="6/b/solution">Solution</h4>

↑ **Parent:** [B](#6/b)

**Yes**, if a merge takes from its left half when two [sort keys](../../algorithm.md#sort-key) compare equal. Within each half the [induction hypothesis](../../foundations-of-mathematics.md#induction-hypothesis) preserves equal-key order. Across the two halves every left-half occurrence originally preceded every right-half occurrence, and the tie rule preserves that order. Reversing the tie rule would lose [stable sorting](../../algorithm.md#stable-sorting).

<h3 id="6/c">c</h3>

↑ **Parent:** [6](#6)

<h4 id="6/c/solution">Solution</h4>

↑ **Parent:** [C](#6/c)

On $n$ distinct opaque keys, a [comparison sorting](../../algorithm.md#comparison-sort) algorithm must distinguish all $n!$ input orders. Its [binary decision tree](../../theoretical-computer-science.md#binary-decision-tree) has at least $n!$ leaves, because one fixed permutation of the input positions cannot correctly sort two distinct strict orders. A tree of height $h$ has at most $2^h$ leaves. Therefore some input needs

$$
\boxed{h\geq\lceil\log_2(n!)\rceil=\Omega(n\log n)}.
$$

The bound is worst-case and specific to algorithms obtaining order information through binary comparisons; it does not apply to every possible representation of keys.

<h3 id="6/d">d</h3>

↑ **Parent:** [6](#6)

<h4 id="6/d/solution">Solution</h4>

↑ **Parent:** [D](#6/d)

Use [counting sort](../../algorithm.md#counting-sort) with 26 counters, indexed by the character code minus the code for `A`. Scan the input to obtain each character's count, then emit that many copies in alphabetic order. Counting costs $O(n)$; visiting 26 counters and writing $n$ outputs costs $O(n+26)=O(n)$.

The comparison lower bound does not apply because the algorithm uses a fixed-size known alphabet and direct key indexing. It does not have to distinguish $n!$ distinct-key orders by binary comparisons; for $n>26$, distinctness is not even possible in this alphabet.

<h3 id="6/e">e</h3>

↑ **Parent:** [6](#6)

<h4 id="6/e/solution">Solution</h4>

↑ **Parent:** [E](#6/e)

For bare characters, equal occurrences are indistinguishable. The count-and-reconstruct implementation in (d) nevertheless **does not preserve the identities of equal-key records**, and so cannot provide [stable sorting](../../algorithm.md#stable-sorting) of associated payloads.

A stable refinement computes cumulative counts $C[j]$, the number of input keys at most $j$, then scans the original records right to left. For a record with key $j$, decrement $C[j]$ and place the complete record at output index $C[j]$. Equal-key records are placed from the end of their allocated range in reverse scanning order, preserving their original relative order. This costs $O(n+26)$ time and $O(n+26)$ auxiliary storage.

<h3 id="6/f">f</h3>

↑ **Parent:** [6](#6)

<h4 id="6/f/solution">Solution</h4>

↑ **Parent:** [F](#6/f)

Precompute the 26 cumulative counts $C[j]=\#\{i:a_i\leq j\}$ using [prefix sums](../../arithmetic.md#prefix-sum). Then

$$
\boxed{\#\{i:c<a_i\leq d\}=C[d]-C[c]\quad\text{if }c<d,}
$$

and the answer is zero if $c\geq d$. Counting and prefix summation take $O(n+26)=O(n)$ preprocessing time and constant storage for this fixed alphabet. Each query uses two indexed reads and one subtraction, hence $O(1)$ time. The guard for $c>d$ prevents a negative answer for an empty interval.

## 7

↑ **Parent:** [Functional programming, design and analysis of algorithms (resit)](functional-programming-design-and-analysis-of-algorithms-resit.md)

<h3 id="7/a">a</h3>

↑ **Parent:** [7](#7)

<h4 id="7/a/solution">Solution</h4>

↑ **Parent:** [A](#7/a)

[Dynamic programming](../../mathematical-optimization.md#dynamic-programming) solves overlapping subproblems once and stores their values for reuse. The [principle of optimality](../../mathematical-optimization.md#principle-of-optimality) says that the remaining decisions within an optimal solution must solve the corresponding residual subproblem optimally; otherwise replacing them by a better residual solution would improve the original one. Here removing one chosen stamp leaves an optimal way to form the remaining postage.

<h3 id="7/b">b</h3>

↑ **Parent:** [7](#7)

<h4 id="7/b/solution">Solution</h4>

↑ **Parent:** [B](#7/b)

Let $F[x]$ be the minimum number of stamps for total $x$. Since denomination 1 is available, every nonnegative total is reachable. The [dynamic programming recurrence](../../mathematical-optimization.md#dynamic-programming-recurrence) is

$$
F[0]=0,\qquad F[x]=1+\min_{d_i\leq x}F[x-d_i]\quad(x\geq1).
$$

Fill the table in increasing order of $x$:
```
F[0] = 0
for x = 1,...,m:
    F[x] = infinity
    for i = 1,...,n:
        if d[i] <= x:
            F[x] = min(F[x], 1 + F[x-d[i]])
return F[m]
```
Every representation of $x$ has a last stamp $d_i$, so its remaining count is at least $F[x-d_i]$. Conversely, appending $d_i$ to an optimal residual representation attains each candidate. Thus the recurrence is exact by the [principle of optimality](../../mathematical-optimization.md#principle-of-optimality). Worst-case time is **$O(mn)$**, with $O(m)$ storage. This is [pseudo-polynomial time](../../theoretical-computer-science.md#pseudo-polynomial-time) in the numerical target, rather than polynomial time in its binary encoding length.

<h3 id="7/c">c</h3>

↑ **Parent:** [7](#7)

<h4 id="7/c/solution">Solution</h4>

↑ **Parent:** [C](#7/c)

Whenever an update improves $F[x]$, store `choice[x] = i`. Starting at `x = m`, repeatedly increment `count[choice[x]]` and subtract that denomination from `x`, stopping at zero. The invariant is that the selected stamps plus an optimal representation of the residual total attain the original optimum; every step reduces $F[x]$ by one. Reconstruction uses $F[m]\leq m$ steps and $O(n)$ output counters, preserving the $O(mn)$ total time bound.

<h3 id="7/d">d</h3>

↑ **Parent:** [7](#7)

<h4 id="7/d/solution">Solution</h4>

↑ **Parent:** [D](#7/d)

The [greedy algorithm](../../algorithm.md#greedy-algorithm) repeatedly takes the largest denomination no greater than the remaining postage. For denominations **$1,3,4$ and target $6$**, it returns $4+1+1$, using three stamps. The optimum is $3+3$, using two. Thus local preference for the largest stamp does not generally solve the [coin change problem](../../mathematical-optimization.md#coin-change-problem) optimally.

<h3 id="7/e">e</h3>

↑ **Parent:** [7](#7)

<h4 id="7/e/solution">Solution</h4>

↑ **Parent:** [E](#7/e)

Use [greedy coin change for powers of an integer](../../mathematical-optimization.md#greedy-coin-change-for-powers-of-an-integer), with integer $p\geq2$. In any optimal solution, there can be no $p$ or more stamps of denomination $p^j$ for $j<k$: replacing $p$ of them by one stamp $p^{j+1}$ preserves value and reduces the stamp count by $p-1$.

Consequently each lower-denomination count lies in $\{0,\ldots,p-1\}$, and their total value is at most

$$
(p-1)(1+p+\cdots+p^{k-1})=p^k-1<p^k.
$$

The number of largest stamps must therefore be $\lfloor m/p^k\rfloor$, leaving a residual below $p^k$. Apply the same argument successively to lower powers. This forces exactly the greedy quotients, proving optimality. For $k=0$, only unit stamps are available and the conclusion is immediate. Integer $p$ is essential to the carry argument and follows from the stated integer denominations whenever denomination $p$ is present.

## 8

↑ **Parent:** [Functional programming, design and analysis of algorithms (resit)](functional-programming-design-and-analysis-of-algorithms-resit.md)

<h3 id="8/a">a</h3>

↑ **Parent:** [8](#8)

<h4 id="8/a/solution">Solution</h4>

↑ **Parent:** [A](#8/a)

A [spanning tree](../../tree-graph-theory.md#spanning-tree) is a connected acyclic subgraph containing every [vertex](../../graph.md#vertex-graph-theory). A [minimum spanning tree](../../tree-graph-theory.md#minimum-spanning-tree) minimizes the sum of edge weights over all spanning trees. In a three-vertex triangle with every edge weight 1, deleting any of the three edges gives a different spanning tree of total weight 2. Hence there are three minimum spanning trees; minimum total weight need not mean a unique tree.

<h3 id="8/b">b</h3>

↑ **Parent:** [8](#8)

<h4 id="8/b/i">i</h4>

↑ **Parent:** [B](#8/b)

<h5 id="8/b/i/solution">Solution</h5>

↑ **Parent:** [I](#8/b/i)

**True.** Every [spanning tree](../../tree-graph-theory.md#spanning-tree) contains precisely the vertex set $V$ by definition. Thus every [minimum spanning tree](../../tree-graph-theory.md#minimum-spanning-tree) has $|V|$ nodes, independently of the weights or which minimum tree is chosen.

<h4 id="8/b/ii">ii</h4>

↑ **Parent:** [B](#8/b)

<h5 id="8/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#8/b/ii)

**True.** Every finite [tree](../../tree-graph-theory.md) on $|V|$ vertices has exactly $|V|-1$ edges. One proof removes a leaf and its incident edge, preserving a tree on one fewer vertex, and applies [induction](../../foundations-of-mathematics.md#mathematical-induction) from the one-vertex tree. Therefore all [minimum spanning trees](../../tree-graph-theory.md#minimum-spanning-tree) have the same edge count.

<h4 id="8/b/iii">iii</h4>

↑ **Parent:** [B](#8/b)

<h5 id="8/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#8/b/iii)

**False.** Take a triangle with $w(ab)=w(bc)=2$ and $w(ac)=3$. Its unique [minimum spanning tree](../../tree-graph-theory.md#minimum-spanning-tree) uses $ab$ and $bc$, with total weight 4. The [shortest path](../../shortest-path-problem.md#shortest-path) from $a$ to $c$ in the original graph is the direct edge of weight 3; the tree's only path has weight 4. A [minimum spanning tree](../../tree-graph-theory.md#minimum-spanning-tree) optimizes total tree weight, not every pairwise path length.

<h3 id="8/c">c</h3>

↑ **Parent:** [8](#8)

<h4 id="8/c/solution">Solution</h4>

↑ **Parent:** [C](#8/c)

[Prim's algorithm](../../tree-graph-theory.md#prim-s-algorithm) grows a tree from any root $r$. For each vertex outside the current tree, its [priority queue](../../data-structure.md#priority-queue) key is the cheapest single edge connecting it to the tree, not the total length of a root-to-vertex path:
```
for v in V:
    key[v] = infinity
    parent[v] = NONE
key[r] = 0
Q = indexed_min_priority_queue(V, key)
while Q is not empty:
    u = Q.extract_min()
    for (v,weight) in adjacency[u]:
        if Q.contains(v) and weight < key[v]:
            parent[v] = u
            key[v] = weight
            Q.decrease_key(v, weight)
return {(parent[v],v) : v != r}
```
The [indexed priority queue](../../data-structure.md#indexed-priority-queue) supports membership and locating a vertex's heap entry. After the first extraction, the chosen parent edge is a least-weight edge crossing the cut between the current tree and its complement. The [minimum spanning tree cut property](../../tree-graph-theory.md#minimum-spanning-tree-cut-property) makes that edge safe: exchanging it for a crossing edge of a suitable minimum tree preserves minimality. Repeating this establishes a minimum tree. Connectivity ensures every nonroot vertex eventually has a parent; edge weights may be negative.

<h3 id="8/d">d</h3>

↑ **Parent:** [8](#8)

<h4 id="8/d/solution">Solution</h4>

↑ **Parent:** [D](#8/d)

An indexed [binary heap](../../data-structure.md#binary-heap) builds the initial queue in $O(|V|)$ time; `extract_min` and `decrease_key` each cost $O(\log |V|)$, while a position table supports membership in $O(1)$. There are $|V|$ extractions and at most $2|E|$ edge inspections, with at most one successful decrease per inspection. Thus the bound is **$O((|V|+|E|)\log |V|)$**, or **$O(|E|\log |V|)$** for a connected graph with at least two vertices. The singleton case is constant time. An unindexed heap cannot provide decrease-key by vertex without an additional position structure.

## ↑ Ancestors (9)

1. [2016](../2016.md)
2. [Past exam of the year 1 of the computer science course of the University of Oxford](../../past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
3. [Year 1 of the computer science course of the University of Oxford](../../university-of-oxford.md#year-1-of-the-computer-science-course-of-the-university-of-oxford)
4. [Computer science course of the University of Oxford](../../university-of-oxford.md#computer-science-course-of-the-university-of-oxford)
5. [Undergraduate course of the University of Oxford](../../university-of-oxford.md#undergraduate-course-of-the-university-of-oxford)
6. [Course of the University of Oxford](../../university-of-oxford.md#course-of-the-university-of-oxford)
7. [University of Oxford](../../university-of-oxford.md)
8. [List of universities](../../README.md#list-of-universities)
9. [Codex Wiki](../../README.md)
