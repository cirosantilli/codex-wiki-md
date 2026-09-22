<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Maintain all pairs discovered so far. Extend every discovered path by one original [binary relation](../../../../../binary-relation.md) edge, keeping the old pairs first:

```
transclose :: Eq a => [(a, a)] -> [(a, a)]
transclose r = grow (removedup r)
  where
    grow s =
      let t = removedup (s ++ relcomp r s)
      in if length t == length s then s else grow t
```

After $j$ extensions, the represented [binary relation](../../../../../binary-relation.md) is $R\cup R^2\cup\cdots\cup R^{j+1}$. This [loop invariant](../../../../../loop-invariant.md) follows by distributivity of [composition of relations](../../../../../composition-of-relations.md) over a [union](../../../../../set-union.md). The old [list](../../../../../list-abstract-data-type.md) `s` is a duplicate-free prefix of `t`; therefore equality of lengths is equivalent to equality of the represented sets and signals a [fixed point](../../../../../fixed-point.md).

Let $V$ be the finite set of endpoints appearing in the input. No extension introduces a new endpoint, so there are at most $|V|^2$ distinct pairs. Every nonfinal iteration adds at least one pair, proving [algorithm termination](../../../../../algorithm-termination.md). At the fixed point $S$, we have $R\subseteq S$ and $R;S\subseteq S$. [Mathematical induction](../../../../../mathematical-induction.md) gives $R^i\subseteq S$ for every positive $i$, while the [loop invariant](../../../../../loop-invariant.md) says that each discovered pair belongs to some $R^i$. Hence

$$
\boxed{\operatorname{transclose}(R)=R^+=\bigcup_{i\ge1}R^i.}
$$

This is the [transitive closure of a relation](../../../../../transitive-closure-relation.md), rather than a reflexive closure: diagonal pairs appear only when supported by nonempty cycles. The empty input is handled immediately.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [2](../../2.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2014](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
