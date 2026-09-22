<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Use the convention $[g,h]=g^{-1}h^{-1}gh$. In $G/K$ the images of $a$ and $b$ commute and both have order three, so $G/K$ is a quotient of $C_3\times C_3$. Thus

$$
[G:K]\leq9.
$$

Put $d=a^{-1}ba$. From the preceding section calculations,

$$
\phi(d)=(1,b,a),qquad
\phi(x)=\phi([a,b])=(a,b^{-1},a^{-1}b).
$$

Since both elements fix the first level, their commutator is computed coordinatewise, and

$$
\phi([d,x])=(1,1,x).
$$

The element $[d,x]$ belongs to $K$. The third-coordinate projection of $\phi(\operatorname{Stab}_G(1))$ is onto $G$, so conjugating this element inside the stabilizer shows that $\phi(K)$ contains $(1,1,x^g)$ for every $g\in G$. Because the conjugates $x^g$ generate $K$, it contains $1\times1\times K$. Conjugation by $a$ cyclically permutes the coordinates; hence it also contains $K\times1\times1$ and $1\times K\times1$. These coordinate subgroups commute, giving

$$
\boxed{K\times K\times K\ leq\phi(K\cap\operatorname{Stab}_G(1)).}
$$

Injectivity of $\phi$ identifies its inverse image with a subgroup of $K$ isomorphic to $K^3$.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [3](../../3.md)
3. [Paper 104](../../../paper-104-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
