<h1 id="5/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Apply $h$ to both sides of $\mathcal R(h^m)=\mathcal R(h^{m+1})$. Because $h(\mathcal R(h^j))=\mathcal R(h^{j+1})$, we obtain $\mathcal R(h^{m+1})=\mathcal R(h^{m+2})$. Repeating this argument proves equality at every later step. More formally, an [induction](../../../../../mathematical-induction.md) on $k$ gives

$$
\boxed{\mathcal R(h^{m+k})=\mathcal R(h^m)\quad\text{for all }k\geq0.}
$$

The base case is $k=0$; the induction step follows from applying the [linear map](../../../../../linear-map.md) $h$ and then the assumed first equality. Thus one equality permanently stabilizes the descending sequence of [images of a linear map](../../../../../image-of-a-linear-map.md).

## ↑ Ancestors (13)

1. [D](../d.md)
2. [5](../../5.md)
3. [Linear algebra](../../linear-algebra.md)
4. [Digital systems, linear algebra and introduction to formal proof](../../../digital-systems-linear-algebra-and-introduction-to-formal-proof-split.md)
5. [2023](../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
