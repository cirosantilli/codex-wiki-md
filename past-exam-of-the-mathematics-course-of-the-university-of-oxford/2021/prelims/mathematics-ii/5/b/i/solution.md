<h1 id="5/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The construction is the partial middle-third construction of the [Cantor function](../../../../../../../cantor-function.md). After $n$ rounds of assigning middle thirds, every remaining open [interval](../../../../../../../interval-mathematics.md) has endpoint values

$$
\frac{k}{2^n},\quad\frac{k+1}{2^n}
$$

for some $k=0,\ldots,2^n-1$, and every such consecutive pair occurs. This follows by [mathematical induction](../../../../../../../mathematical-induction.md). Initially the endpoint values are $0,1$. An [interval](../../../../../../../interval-mathematics.md) with those consecutive endpoint values receives the value

$$
\frac12\left(\frac{k}{2^n}+\frac{k+1}{2^n}\right)=\frac{2k+1}{2^{n+1}}
$$

on its closed middle third. Its two remaining open [intervals](../../../../../../../interval-mathematics.md) therefore have consecutive endpoint values at denominator $2^{n+1}$. All previously assigned endpoint values persist. Hence all even numerators at the next denominator were already present, and all odd numerators have just been assigned. Including the initial values zero and one proves

$$
\boxed{\{k/2^n:0\leq k\leq2^n\}\subseteq f(\mathbb R\setminus C)\quad(n\geq0).}
$$

These are precisely the [dyadic rational](../../../../../../../dyadic-rational.md) values between zero and one.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [5](../../../5.md)
4. [Mathematics II](../../../../mathematics-ii-split.md)
5. [Prelims](../../../../split.md)
6. [2021](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
