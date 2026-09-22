<h1 id="2/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Alice's own freshness evidence is the ticket

$$
U=E_{\mathit{pk}_A}(\mathit{nonce}_A\Vert\mathit{secret}_A\Vert A\Vert B\Vert k_{AB}).
$$

After [decryption](../../../../../../decryption.md), she checks her pending [cryptographic nonce](../../../../../../cryptographic-nonce.md), the long-term shared secret and both identities. Only Alice and Tim know $\mathit{secret}_A$; with honest Tim and an unpredictable new $\mathit{nonce}_A$, a valid matching ticket establishes that Tim generated this [session key](../../../../../../session-key.md) after that challenge was issued. A merely unused but predictable challenge does not establish that temporal ordering.

The claimed [authentication](../../../../../../authentication.md) of Alice to Bob, however, is false for the printed [protocol](../../../../../../communication-protocol.md). To exhibit the failure, let $I$ initiate message 1 using Alice's name while Alice is absent. Bob and Tim carry out messages 2 and 3 normally. Write the genuine message 3 as $(U,b,V)$, where $b=\mathit{nonce}_B$ and $V=E_{\mathit{pk}_B}(A\Vert B\Vert k_{AB})$. The adversary intercepts it, learns the unencrypted $b$, and chooses a symmetric key $z$ of its own.

The adversary sends Bob

$$
\bigl(U,b,E_{\mathit{pk}_B}(A\Vert B\Vert z)\bigr).
$$

Bob's checks of $b$ and the ticket identities pass, because anyone can encrypt using his [public key](../../../../../../public-key.md). Bob sends message 4 using $z$; the adversary suppresses that message and returns $E_z(\text{Hello Bob})$ as message 5. Bob accepts Alice, although Alice has done nothing. No [encryption](../../../../../../encryption.md) has been broken.

$$
\boxed{\text{Alice can check her ticket's freshness, but Bob has not authenticated Alice.}}
$$

The tempting intended argument is that only Alice, Bob and Tim could know the transported key, so message 5 proves Alice's participation. The substituted ticket invalidates its premise: Bob's accepted key is $z$, which the adversary knows.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [Computer security](../../../../computer-security-split.md)
5. [2015](../../../../split.md)
6. [Past exam of the computer science course of the University of Oxford](../../../../../split.md)
7. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)

## ← Incoming links (3)

- [Solution](../ii/solution.md)
- [Solution](../iii/solution.md)
- [Solution](../v/solution.md)
