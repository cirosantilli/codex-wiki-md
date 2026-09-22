<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Represent $a+b\sqrt5$ by the pair $(a,b)$ in the [quadratic field](../../../../../quadratic-field.md) $\mathbb Q(\sqrt5)$. Its multiplication rule is

$$
\boxed{(a+b\sqrt5)(c+d\sqrt5)=(ac+5bd)+(ad+bc)\sqrt5.}
$$

The constructor copies both rational components, so later reduction through another pointer cannot change the constructed value:

```
PROCEDURE mkIrr(r,i: rational): irrational;
VAR z: irrational;
BEGIN
  NEW(z);
  z.rat := mkRat(r.num,r.den);
  z.irr := mkRat(i.num,i.den);
  RETURN z
END mkIrr;

PROCEDURE addIrr(x,y: irrational): irrational;
BEGIN
  RETURN mkIrr(addRat(x.rat,y.rat),addRat(x.irr,y.irr))
END addIrr;

PROCEDURE mulIrr(x,y: irrational): irrational;
VAR r,i: rational;
BEGIN
  r := addRat(mulRat(x.rat,y.rat),
              mulRat(mkRat(5,1),mulRat(x.irr,y.irr)));
  i := addRat(mulRat(x.rat,y.irr),mulRat(x.irr,y.rat));
  RETURN mkIrr(r,i)
END mulIrr;
```

The representation includes rational values when the second coefficient is zero; the supplied type name does not require every stored value to be irrational.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [1](../../1.md)
3. [Imperative programming (resit)](../../../imperative-programming-resit-split.md)
4. [2017](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
