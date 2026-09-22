<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

For the converse, let $f$ be bounded and $\|f\|=f(1)=c$. If $c=0$, it is zero and positive. Suppose $c>0$. For any Hermitian $h$, the [Banach algebra exponential](../../../../../banach-algebra-exponential.md) $e^{ith}$ is unitary for real $t$, so its norm is one by the [C-star identity](../../../../../c-star-identity.md). Consequently

$$
|f(e^{ith})|\leq c,\qquad f(e^{ith})=c+itf(h)+O(t^2).
$$

Writing $f(h)=u+iv$ and squaring moduli gives $|f(e^{ith})|^2=c^2-2cvt+O(t^2)$. The bound for both signs of small $t$ forces $v=0$, so $f(h)$ is real.

For a Hermitian element $a$, repeated applications of the C-star identity give $\|a^{2^n}\|=\|a\|^{2^n}$. The [spectral radius formula](../../../../../spectral-radius-formula.md) therefore gives $\|a\|=r(a)$. Take $h=x^*x$; by the permitted spectral positivity assumption, $\sigma(h)\subseteq[0,\|h\|]$. If $M=\|h\|>0$, affine spectral mapping and the just-proved Hermitian norm identity give $\|1-h/M\|\leq1$. Hence $|c-f(h)/M|\leq c$. Since $f(h)$ is real, this implies $f(h)\geq0$. If $M=0$, $h=0$ and the result is immediate. Thus **a bounded functional with $\|f\|=f(1)$ is positive**.

For the spectral-value request, let $\lambda\in\sigma(x)$ and define a functional on the linear span of $1,x$ by $g(a1+bx)=a+b\lambda$. If $b\ne0$, the scalar $a+b\lambda$ belongs to $\sigma(a1+bx)$: subtracting it from that element gives $b(x-\lambda1)$, which is not invertible. The same norm bound is immediate for $b=0$. Therefore

$$
|a+b\lambda|\leq r(a1+bx)\leq\|a1+bx\|.
$$

This also proves well-definedness if that span is one-dimensional. We have $g(1)=1$ and $\|g\|=1$. The complex [Hahn-Banach theorem](../../../../../hahn-banach-theorem.md) extends it to a functional $f$ on all of $A$ with norm one and $f(1)=1$. The converse just proved makes that extension positive. Thus **there is a state with $f(x)=\lambda$**, the [spectral values attained by C-star states](../../../../../spectral-values-attained-by-c-star-states.md) result.

Finally, for $x\ne0$, write $x=h+ik$ with $h,k$ Hermitian. At least one of them is nonzero. Its norm equals its spectral radius, so compactness of its nonempty spectrum supplies a nonzero spectral value. Apply the preceding state construction to that Hermitian element. Part (i) makes $f(h),f(k)$ real; the selected one is nonzero, so $f(x)=f(h)+if(k)\ne0$. This proves **positive functionals separate every nonzero element**, the [states separate elements of a C-star algebra](../../../../../states-separate-elements-of-a-c-star-algebra.md) property. Looking only at $\sigma(x)$ would not prove this last step, since a nonzero quasinilpotent $x$ can have spectrum $\{0\}$.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 10](../../paper-10-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
