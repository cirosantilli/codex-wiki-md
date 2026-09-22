# Computational monad

↑ **Parent:** [Functional programming](functional-programming.md)

A [type constructor](type-constructor.md) $M$ with operations $\operatorname{result}:A\to M A$ and $\mathbin{\triangleright}:M A\to(A\to M B)\to M B$ satisfying the [monad laws](monad-laws.md). The first embeds a value; the second sequences a computation with a value-dependent continuation. This is the programming interface to a [monad](monad.md).

**Table of contents**

- [Continuation monad](continuation-monad.md)
- [Identity monad](identity-monad.md)
- [State monad](state-monad.md)
- [Monad transformer](monad-transformer.md)
  - [Continuation monad transformer](continuation-monad-transformer.md)
  - [Exception monad transformer](exception-monad-transformer.md)
  - [State monad transformer](state-monad-transformer.md)
- [Monad laws](monad-laws.md)

## ↑ Ancestors (4)

1. [Functional programming](functional-programming.md)
2. [Programming language](programming-language-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (18)

- [Call-by-value](call-by-value.md)
- [Continuation monad](continuation-monad.md)
- [Continuation monad transformer](continuation-monad-transformer.md)
- [Exception monad transformer](exception-monad-transformer.md)
- [Identity monad](identity-monad.md)
- [Monad laws](monad-laws.md)
- [Monad transformer](monad-transformer.md)
- [Monadic interpreter](monadic-interpreter.md)
- [Principles of programming languages](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2015/principles-of-programming-languages-split.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2015/principles-of-programming-languages/1/a/solution.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2015/principles-of-programming-languages/1/b/solution.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2015/principles-of-programming-languages/1/d/solution.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2015/principles-of-programming-languages/1/f/solution.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2015/principles-of-programming-languages/1/g/solution.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2015/principles-of-programming-languages/3/a/solution.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2015/principles-of-programming-languages/3/b/solution.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2015/principles-of-programming-languages/3/d/solution.md)
- [State monad transformer](state-monad-transformer.md)
