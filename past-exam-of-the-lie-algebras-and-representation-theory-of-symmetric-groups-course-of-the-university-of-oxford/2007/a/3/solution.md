<h1 id="a/3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Use the standard split [weight-space decomposition](../../../../weight-space-decomposition.md) in [characteristic zero](../../../../characteristic-zero.md), in particular the usual complex setting: $L=\bigoplus_\varphi L_\varphi$, with generalized weights for the nilpotent algebra $H$. The characteristic-zero condition prevents nonzero weight shifts from wrapping around; the unrestricted positive-characteristic version would need additional hypotheses.

For fixed $h\in H$, let $D=\operatorname{ad}h$. On a bracket of [vectors](../../../../vector.md) from $L_\varphi,L_\psi$, the [derivation](../../../../derivation-of-an-algebra.md) identity gives

$$
(D-(\varphi+\psi)(h))[u,v]=[(D-\varphi(h))u,v]+[u,(D-\psi(h))v].
$$

Iterating it gives the binomial expansion of these two commuting actions. At power $2n-1$, each term kills at least one factor, because generalized weight [vectors](../../../../vector.md) are killed by the $n$th power of the corresponding shifted operator. Therefore the bracket lies in the generalized eigenspace for $(\varphi+\psi)(h)$ for every $h$. Stabilization of kernels by dimension $n$ gives

$$
\boxed{[L_\varphi,L_\psi]\subseteq L_{\varphi+\psi},}
$$

where $L_\eta=0$ when $\eta$ is not a weight.

Nilpotence of $H$ gives $H\subseteq L_0$. If $H$ is a [Cartan subalgebra](../../../../cartan-subalgebra.md) and $L_0/H\ne0$, the action of $H$ on this quotient consists of nilpotent operators. [Engel's theorem](../../../../engel-s-theorem.md) supplies a nonzero coset $v+H$ killed by $H$, giving $[H,v]\subseteq H$ with $v\notin H$, a contradiction to self-normalization. Conversely, if $L_0=H$ and $v$ normalizes $H$, then $[h,v]\in H$ for each $h$. Applying further powers of $\operatorname{ad}h$ kills this [vector](../../../../vector.md) because its restriction to $H$ is nilpotent. Hence $v\in L_0=H$. This proves the equivalence.

The operator $\operatorname{ad}e$ sends $L_\varphi$ into $L_{\varphi+\alpha}$. Repetition follows a consecutive $\alpha$-string; after $r$ steps it must leave the weight set, because $r$ is the largest number of weights in any such string. Thus $\boxed{(\operatorname{ad}e)^r=0}$ on every [weight space](../../../../weight-space.md) and hence on $L$.

Finally put $E=\operatorname{ad}e$ and $F=\operatorname{ad}f$. Expand $(E+F)^n$ as the sum of all words of length $n$, without commuting $E$ and $F$. Acting on $L_\gamma$, each word follows weights $\gamma+i\alpha+j\beta$ with $i+j$ increasing by one at each step. [Linear independence](../../../../linear-independence.md) of $\alpha,\beta$ in [characteristic zero](../../../../characteristic-zero.md) makes the successive weights distinct. A nonzero length-$n$ path would require $n+1$ different [weight spaces](../../../../weight-space.md), but $\dim L=n$. Every word therefore vanishes, giving

$$
\boxed{(\operatorname{ad}(e+f))^n=0.}
$$

## ↑ Ancestors (12)

1. [3](../3.md)
2. [A](../../a.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the Lie algebras and representation theory of symmetric groups course of the University of Oxford](../../../split.md)
5. [Lie algebras and representation theory of symmetric groups course of the University of Oxford](../../../../lie-algebras-and-representation-theory-of-symmetric-groups-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
