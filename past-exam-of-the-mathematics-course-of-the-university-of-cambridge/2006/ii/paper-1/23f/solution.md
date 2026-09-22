<h1 id="23f/solution">Solution</h1>

↑ **Parent:** [23F](../23f.md)

Uniqueness in the defining characterization gives $\wp(-z)=\wp(z)$: the reflected function has the same [poles](../../../../../pole.md), periodicity and prescribed [principal part](../../../../../principal-part-of-a-meromorphic-function.md). Hence $\wp'$ is odd and periodic. At each nonzero half-period $\omega\in\{1/2,\tau/2,(1+\tau)/2\}$, $-\omega\equiv\omega\pmod\Lambda$, so $\wp'(\omega)=-\wp'(\omega)=0$.

An [elliptic function](../../../../../elliptic-function.md) has equally many zeros and [poles](../../../../../pole.md), counted with multiplicities, in a [fundamental parallelogram](../../../../../fundamental-parallelogram-of-a-period-lattice.md). This standard property applies to $\wp'$, whose sole [pole](../../../../../pole.md) modulo the lattice has order three. The three distinct nonzero half-periods already supply three zeros, so these are all its zeros and each is simple. Thus

$$
\boxed{\{z:\wp'(z)=0\}=\bigcup_{\omega\in\{1/2,\tau/2,(1+\tau)/2\}}(\omega+\Lambda).}
$$

Evenness and the prescribed expansion give $\wp(z)=z^{-2}+a_2z^2+a_4z^4+O(z^6)$. There is no constant term because the defining difference tends to zero, and only even powers occur. Consequently

$$
\wp'(z)^2-4\wp(z)^3=-20a_2z^{-2}-28a_4+O(z^2).
$$

Adding $20a_2\wp$ cancels the last [pole](../../../../../pole.md). The resulting [elliptic function](../../../../../elliptic-function.md) is [holomorphic](../../../../../complex-differentiability-at-a-point.md) everywhere and therefore constant, by boundedness on a [fundamental parallelogram](../../../../../fundamental-parallelogram-of-a-period-lattice.md) and [Liouville theorem](../../../../../liouville-theorem.md). Its value at zero is $-28a_4$. Thus

$$
\wp'^2=4\wp^3-20a_2\wp-28a_4=Q(\wp).
$$

At the three half-periods $Q(\wp(\omega))=0$. Their values are distinct: if two such points had the same value $e$, then $\wp-e$ would have a zero of [multiplicity](../../../../../multiplicity-mathematics.md) at least two at each, because its [derivative](../../../../../derivative.md) vanishes there. That gives at least four zeros, contrary to its sole double [pole](../../../../../pole.md) and the zero-pole counting property. Hence the cubic has three distinct roots and leading coefficient four, proving

$$
\boxed{Q(w)=4(w-\wp(1/2))(w-\wp(\tau/2))(w-\wp((1+\tau)/2)).}
$$

All properties specific to $\wp$ used here were derived from its defining characterization; only the general elliptic zero-pole count and [holomorphic](../../../../../complex-differentiability-at-a-point.md) constancy were used as standard facts.

## ↑ Ancestors (10)

1. [23F](../23f.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
