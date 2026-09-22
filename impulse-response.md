# Impulse response

↑ **Parent:** [Green's function](green-s-function.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Impulse_response)

The impulse response records the response to a unit impulse, with specified initial or boundary conditions. In continuous time the impulse is a [Dirac delta function](dirac-delta-function.md); in discrete time it is the [Kronecker delta](kronecker-delta.md) $\delta[n]$. For a [linear time-invariant system](linear-time-invariant-system.md) with zero initial state, the response to a general [input](input-computer-science.md) is its [convolution](convolution.md) with the impulse response. The impulse response of a [causal filter](causal-filter.md) is zero before the impulse.

For the five-sample [moving average](moving-average.md), a discrete impulse produces $h[n]=1/5$ at $n=0,1,2,3,4$ and zero otherwise. The response lasts five samples, so this is a [finite impulse response](finite-impulse-response.md) system. Its [frequency response](frequency-response.md) is the finite sum of the five delayed phase contributions: one short input experiment determines how every sustained sinusoid is filtered.

## ↑ Ancestors (5)

1. [Green's function](green-s-function.md)
2. [Analysis](analysis-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (12)

- [Causal response of a first-order relaxation equation](causal-response-of-a-first-order-relaxation-equation.md)
- [Convolution](convolution.md)
- [Convolution kernel](convolution-kernel.md)
- [Finite impulse response](finite-impulse-response.md)
- [Frequency response](frequency-response.md)
- [Laplace transform](laplace-transform.md)
- [Linear filter](linear-filter.md)
- [Linear time-invariant system](linear-time-invariant-system.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ia/paper-2/7b/i/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ia/paper-2/7b/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ib/paper-3/6a/solution.md)
- [Signal processing](signal-processing.md)
