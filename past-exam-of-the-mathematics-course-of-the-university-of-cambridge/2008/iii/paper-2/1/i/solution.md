<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The identified involution is $z=g^2=h^5$. It is central: it commutes with $g$ because it is a power of $g$, and with $h$ because it is a power of $h$. We use the [normal form theorem for an amalgamated free product](../../../../../../normal-form-theorem-for-an-amalgamated-free-product.md): the two factors embed, an alternating product of elements outside the amalgamated subgroup is nonidentity, and fixed coset representatives give a unique reduced expression. Here choose representatives $1,g$ in the first [cyclic group](../../../../../../cyclic-group.md) and $1,h,h^2,h^3,h^4$ in the second.

An effective expression from the [normal form theorem for an amalgamated free product](../../../../../../normal-form-theorem-for-an-amalgamated-free-product.md) is

$$
z^\varepsilon x_1\cdots x_r,\qquad\varepsilon\in\{0,1\},
$$

where each $x_j$ is a nonidentity representative and successive representatives come from different factors. Reduce powers by $g^u=z^{\lfloor u/2\rfloor}g^{u\bmod2}$ and $h^v=z^{\lfloor v/5\rfloor}h^{v\bmod5}$, using these identities for negative integers too. Move the central $z$ factors left and reduce their total exponent modulo two. Whenever adjacent representatives come from one factor, multiply them, split off their $z$ contribution, and delete a resulting identity. Each such combination reduces the number of representatives, so the procedure terminates. By the [normal form theorem for an amalgamated free product](../../../../../../normal-form-theorem-for-an-amalgamated-free-product.md), **the input is trivial exactly when $\boxed{r=0\text{ and }\varepsilon=0}$.** In particular $z\ne1$ because each factor embeds. This gives the [soluble word problem in finite cyclic amalgams](../../../../../../soluble-word-problem-in-finite-cyclic-amalgams.md) algorithm without merely asserting that a normal form exists.

In the specified quotient, the extra [relator](../../../../../../relator.md) makes $g,h$ commute. Put $t=gh^{-2}$. Its abelian [group presentation](../../../../../../group-presentation.md) gives

$$
t^5=g^5h^{-10}=g,\qquad t^2=g^2h^{-4}=h,\qquad t^{20}=1.
$$

Conversely $g\mapsto s^5$, $h\mapsto s^2$ satisfy every quotient relator in $C_{20}=\langle s\mid s^{20}=1\rangle$, and send $t$ to $s$. Thus the quotient is exactly $C_{20}$, rather than just a cyclic group of order dividing twenty. If $M,N$ are the exponent sums of $g,h$ in the input, **its quotient word problem is**

$$
\boxed{w=1\quad\Longleftrightarrow\quad5M+2N\equiv0\pmod{20}.}
$$

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
