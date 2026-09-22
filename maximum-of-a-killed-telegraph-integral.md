# Maximum of a killed telegraph integral

↑ **Parent:** [Strong Markov property](strong-markov-property.md)

Let $X$ switch between $\pm1$ at rate $q$ and be killed into zero at rate $\lambda$. To exceed a new level it must cross it in state $+1$. Restarting there by the [Strong Markov property](strong-markov-property.md) gives the multiplicative identity $\psi_+(c+d)=\psi_+(c)\psi_+(d)$, hence an exponential tail. First-step conditioning gives $\psi_-(c)=\int_0^\infty qe^{-(q+\lambda)u}\psi_+(c+u)du$ and $\psi_+(c)=e^{-(q+\lambda)c}+\int_0^cqe^{-(q+\lambda)u}\psi_-(c-u)du$. Substituting the exponential determines its rate as $\sqrt{\lambda(2q+\lambda)}$.

## ↑ Ancestors (8)

1. [Strong Markov property](strong-markov-property.md)
2. [Markov chain](markov-chain.md)
3. [Markov process](markov-process-split.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)
