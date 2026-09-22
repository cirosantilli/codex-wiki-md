<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Place a [proof of work](../../../../../proof-of-work.md) gate before Tim performs the expensive private-key [decryption](../../../../../decryption.md) in message 2. Binding the puzzle to the whole request prevents solving a cheap puzzle once and reusing it with different tickets.

For example, let $R$ be the exact encoding of message 2, including identities, Alice's [cryptographic nonce](../../../../../cryptographic-nonce.md) and Bob's encrypted component. On receiving a proposed request, Tim does only cheap length and format checks and returns a fresh challenge $r$, an expiry time $t$, a difficulty $d$ and a cookie

$$
\tau=\operatorname{MAC}_{s_T}(\text{puzzle}\Vert h(R)\Vert r\Vert t\Vert d).
$$

Here $s_T$ is Tim's cookie secret and the [message authentication code](../../../../../message-authentication-code.md) prevents alteration of the challenge or difficulty. Tim need not retain large amounts of per-request state merely to issue the cookie.

The requester finds a suffix $w$ such that

$$
\boxed{h(\text{work}\Vert h(R)\Vert r\Vert t\Vert d\Vert w)\text{ begins with }d\text{ zero bits}.}
$$

Under the usual unpredictable-hash-output model, this takes an expected $2^d$ trials; verifying a proposed suffix needs one [cryptographic hash function](../../../../../cryptographic-hash-function.md) evaluation after checking the request digest and cookie. [Preimage resistance](../../../../../preimage-resistance.md) motivates search difficulty, but the exact $2^d$ estimate also uses that distribution assumption.

The requester returns $(R,r,t,d,\tau,w)$. Before any expensive [decryption](../../../../../decryption.md), Tim verifies the cookie, expiry, work and request binding, and atomically records that this challenge has been consumed. Repeated submissions of a consumed challenge are rejected cheaply. Short expiry bounds the storage needed for spent challenges. A cookie alone is insufficient: without one-use enforcement, the attacker could replay a single valid solved request indefinitely.

To charge the work to the initiator rather than Bob, Bob can relay the challenge to Alice and forward her solution. The adversary's fake Alice must then solve each puzzle instead of making honest Bob do it. Tim must issue challenges and reject bad proofs with bounded inexpensive processing, and difficulty should be chosen so that many verified requests require substantial aggregate work. This mitigates the computational [denial-of-service attack](../../../../../denial-of-service-attack.md); it does not correct the separate [authentication](../../../../../authentication.md) flaw.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Computer security](../../../computer-security-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
