<h1 id="30c/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Apply the volume [mean value property](../../../../../../mean-value-property-for-harmonic-functions.md) to the two balls and use nonnegativity together with inclusion:

$$
u(w)=\frac1{|B(w,R)|}\int_{B(w,R)}u\ge\frac1{|B(w,R)|}\int_{B(z,r)}u=\boxed{\left(\frac rR\right)^3u(z).}
$$

For any $w,z\in B(x,r)$, the [triangle inequality](../../../../../../triangle-inequality.md) gives $B(z,r)\subset B(w,3r)\subset B(x,4r)\subset\Omega$. Taking $R=3r$ in the previous bound therefore gives $u(w)\ge u(z)/27$. Take the infimum over $w$ and supremum over $z$ to obtain

$$
\boxed{\inf_{B(x,r)}u\ge3^{-3}\sup_{B(x,r)}u.}
$$

No positivity stronger than nonnegativity is needed; if a value vanishes, this argument forces every value in the smaller ball to vanish too.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [30C](../../30c.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
