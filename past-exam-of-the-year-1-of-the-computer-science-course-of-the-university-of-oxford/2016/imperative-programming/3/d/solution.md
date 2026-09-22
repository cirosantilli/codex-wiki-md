<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Convert the tail first and apply the reciprocal identity. Two output parameters hold the [rational number](../../../../../rational-number.md)'s numerator and denominator.
```
PROCEDURE cf2rat(f: fraction; VAR n, d: INTEGER);
VAR u, v: INTEGER;
BEGIN
  IF f.tail = NIL THEN
    n := f.head; d := 1
  ELSE
    cf2rat(f.tail, u, v);
    n := f.head * u + v;
    d := u
  END
END cf2rat;
```
The singleton case is immediate. If the recursive call returns the tail as $u/v$, then $u,v>0$ because every tail head is positive. The full value is

$$
f.\mathrm{head}+\frac1{u/v}=\frac{f.\mathrm{head}\,u+v}{u}.
$$

[Structural induction](../../../../../structural-induction.md) on the finite nonempty [linked list](../../../../../linked-list.md) proves correctness, and the denominator is always positive even if the first head is negative. If the tail pair is coprime, then $\gcd(xu+v,u)=\gcd(v,u)=1$; the base pair $(x,1)$ is coprime, so the result is in lowest terms. **Return `(head*u+v,u)` after converting the tail**, using linear node-processing time and linear recursive stack space.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [3](../../3.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2016](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
