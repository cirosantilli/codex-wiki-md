<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the convention that the [inner product](../../../../inner-product-split.md) is linear in its first argument. The precise [polarization identity](../../../../polarization-identity.md) is

$$
\boxed{\langle x,y\rangle=\frac14\left(
\|x+y\|^2-\|x-y\|^2+i\|x+iy\|^2-i\|x-iy\|^2\right).}
$$

If (1) holds, apply this formula before and after $U$ to get preservation of all [inner products](../../../../inner-product-split.md), proving (2). If (2) holds, the identity $\langle Ux,Uy\rangle=\langle x,U^*Uy\rangle$ gives $U^*U=I$. For $z=Ux$, surjectivity then gives $UU^*z=UU^*Ux=Ux=z$, proving (3).

From (3), $\|Ux\|^2=\langle x,U^*Ux\rangle=\|x\|^2$ and likewise $\|U^*x\|=\|x\|$, proving (4). Finally, if (4) holds, apply the same [polarization identity](../../../../polarization-identity.md) to $U^*$ to obtain $UU^*=I$. This makes $U$ onto; the other [norm](../../../../norm.md) identity supplies the remaining requirement of (1). Thus

$$
\boxed{(1)\iff(2)\iff(3)\iff(4).}
$$

These four statements are conditions in a single equivalence proof, rather than four independent source questions.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [6](../../6.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the analysis course of the University of Oxford](../../../split.md)
5. [Analysis course of the University of Oxford](../../../../analysis-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
