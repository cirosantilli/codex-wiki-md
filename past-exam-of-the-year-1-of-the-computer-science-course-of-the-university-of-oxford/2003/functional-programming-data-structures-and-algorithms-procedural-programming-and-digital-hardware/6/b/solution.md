<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

In [binary long division](../../../../../binary-long-division.md), first double the divisor until it exceeds `x`, then halve it successively. Keep `p = 2^j` and `d = y*p`, so no exponentiation is needed inside a loop:

```
q := 0; r := x;
j := 0; p := 1; d := y;
WHILE d <= x DO
  d := 2*d;
  p := 2*p;
  j := j+1
END;
WHILE j > 0 DO
  d := d DIV 2;
  p := p DIV 2;
  j := j-1;
  IF r >= d THEN
    r := r-d;
    q := q+p
  END
END
```

The first [loop invariant](../../../../../loop-invariant.md) is $q=0$, $r=x$, $j\geq0$, $p=2^j$ and $d=y2^j>0$. Every doubling preserves it. For [integer](../../../../../integer-split.md) inputs, after at most $1+\lfloor\log_2(x/y)\rfloor$ iterations when $x\geq y$, `d > x`; if $x<y$, this loop has no iterations. The unbounded increase of $y2^j$ proves termination. Equivalently, one can use the decreasing nonnegative [loop variant](../../../../../loop-variant.md) $\max(0,\lfloor\log_2(x/d)\rfloor+1)$ while the guard is true.

At the top of the second loop the [loop invariant](../../../../../loop-invariant.md) is

$$
\boxed{x=qy+r,\quad0\leq r<d=y2^j,\quad p=2^j,\quad q\geq0,\quad j\geq0.}
$$

It holds on entry because `d > x = r`. Suppose the old `d` is $2d'$ and the old `p` is $2p'$. After the three halving assignments, $d'=yp'$ and the old remainder satisfies $0\leq r<2d'$. If $r<d'$, the desired new bound already holds. Otherwise subtracting $d'$ leaves $0\leq r-d'<d'$ and adding $p'$ to `q` preserves $x=qy+r$ because $yp'=d'$. The divisions by two are exact: before each halving, `j > 0` makes both `p` and `d` even.

The [loop variant](../../../../../loop-variant.md) `j` decreases by one each iteration. At exit $j=0$, so `d = y` and the [loop invariant](../../../../../loop-invariant.md) gives the required remainder bound. The work per iteration is constant in the [unit-cost model](../../../../../unit-cost-model.md), and the two loops have the same number of iterations. For $0<y\leq x$,

$$
\boxed{T(x,y)=O(1+\log(x/y))=O(\log(x+1)).}
$$

The case $x<y$, including $x=0$, takes [constant time](../../../../../constant-time.md). These are arithmetic-operation counts with sufficient range for the doubled values; [arbitrary-precision arithmetic](../../../../../arbitrary-precision-arithmetic.md) incurs additional [bit complexity](../../../../../bit-complexity.md). If the inputs were arbitrary positive [real numbers](../../../../../real-number.md), the uniform bound would depend on $x/y$ rather than only $x$; the stated $O(\log x)$ is the conventional [integer division](../../../../../integer-division.md) interpretation.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [6](../../6.md)
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
