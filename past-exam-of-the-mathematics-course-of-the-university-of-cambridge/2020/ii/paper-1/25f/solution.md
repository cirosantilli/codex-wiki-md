<h1 id="25f/solution">Solution</h1>

↑ **Parent:** [25F](../25f.md)

Suppose first that the [affine variety](../../../../../affine-algebraic-set.md) $V$ is irreducible. If $fg\in I(V)$, then

$$
V=(V\cap V(f))\cup(V\cap V(g)).
$$

Both pieces are [Zariski closed](../../../../../zariski-closed-set.md) in $V$. Irreducibility forces one to equal $V$, so either $f\in I(V)$ or $g\in I(V)$. Thus $I(V)$ is a [prime ideal](../../../../../prime-ideal.md).

Conversely, suppose that $I(V)$ is prime and that $V=A\cup B$ with $A,B$ closed in $V$. If both were proper, the [Hilbert Nullstellensatz](../../../../../hilbert-nullstellensatz.md) would give

$$
I(V)\subsetneq I(A),
\qquad
I(V)\subsetneq I(B).
$$

Choose $f\in I(A)\setminus I(V)$ and $g\in I(B)\setminus I(V)$. Their product vanishes on $A\cup B=V$, so $fg\in I(V)$, contradicting primality. Hence one piece equals $V$. This proves the criterion of [irreducibility and prime vanishing ideal](../../../../../irreducibility-and-prime-vanishing-ideal.md):

$$
\boxed{V\text{ is irreducible}\iff I(V)\text{ is prime}}.
$$

For the [semicubical parabola](../../../../../semicubical-parabola.md)

$$
C=V(y^2-x^3),
$$

consider

$$
\theta:k[x,y]\to k[t],
\qquad
\theta(x)=t^2,\quad\theta(y)=t^3.
$$

Certainly $(y^2-x^3)\subseteq\ker\theta$. Divide any polynomial by the monic polynomial $y^2-x^3$ as a polynomial in $y$; its remainder is $a(x)y+b(x)$. If this remainder lies in $\ker\theta$, then

$$
a(t^2)t^3+b(t^2)=0.
$$

The first summand contains only odd powers of $t$ and the second only even powers, so both vanish and $a=b=0$. Therefore

$$
\ker\theta=(y^2-x^3),
\qquad
k[C]\cong k[t^2,t^3].
$$

The latter is a subring of the [integral domain](../../../../../integral-domain.md) $k[t]$, hence is a domain. Thus $(y^2-x^3)$ is prime and

$$
\boxed{C\text{ is irreducible}}.
$$

An affine variety of dimension $d$ is smooth at $p$ when its [Zariski tangent space](../../../../../zariski-tangent-space.md) has dimension $d$; equivalently, the [Jacobian criterion](../../../../../jacobian-criterion.md) requires the Jacobian of its defining ideal to have rank $n-d$. For this plane curve, put $F(x,y)=y^2-x^3$. Its gradient is

$$
\nabla F=(-3x^2,2y).
$$

At $(0,0)\in C$ the gradient vanishes, so the tangent space is all of $k^2$ and has dimension two rather than the curve dimension one. Hence the result on the [coordinate ring and singularity of the semicubical parabola](../../../../../coordinate-ring-and-singularity-of-the-semicubical-parabola.md) gives

$$
\boxed{C\text{ is not smooth; its origin is singular}}.
$$

## ↑ Ancestors (10)

1. [25F](../25f.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2020](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
