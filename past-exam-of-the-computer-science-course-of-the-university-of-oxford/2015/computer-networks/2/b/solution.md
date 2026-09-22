<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

[Network address translation](../../../../../network-address-translation.md) lets a [router](../../../../../router.md) join a private [Internet Protocol](../../../../../internet-protocol.md) address realm to the public [Internet](../../../../../internet.md). On outbound [packets](../../../../../network-packet.md) it replaces the private source [IP address](../../../../../ip-address.md) by a public [IP address](../../../../../ip-address.md). On returning [packets](../../../../../network-packet.md) it applies the inverse mapping to the destination [IP address](../../../../../ip-address.md), then forwards to the internal host. Basic [network address translation](../../../../../network-address-translation.md) changes addresses; the common many-to-one form, [network address and port translation](../../../../../network-address-and-port-translation.md), also changes the source [transport port](../../../../../transport-port.md) so several internal hosts can share one public [IP address](../../../../../ip-address.md).[§§2.1–2.2 and 3.1–3.3: basic NAT, NAPT and translation phases](../../../../../traditional-ip-network-address-translator-traditional-nat-rfc-3022.md)

For example, suppose the public-facing [router](../../../../../router.md) has [IP address](../../../../../ip-address.md) `198.51.100.7`. An internal [TCP](../../../../../transmission-control-protocol.md) exchange might be translated as follows; the addresses are illustrative:

$$
\begin{aligned}
(10.0.0.2:49152)\longrightarrow(192.0.2.80:80)
&\quad\mapsto\quad
(198.51.100.7:62001)\longrightarrow(192.0.2.80:80).
\end{aligned}
$$

An entry records that traffic returning to external [transport port](../../../../../transport-port.md) 62001 belongs to `10.0.0.2:49152` for this [transport protocol](../../../../../transport-protocol.md). The destination on the return path is rewritten accordingly. A second internal host using the same private [transport port](../../../../../transport-port.md) can receive a different public [transport port](../../../../../transport-port.md). The actual lookup may also use the remote [endpoint](../../../../../communication-endpoint.md), depending on the mapping and filtering policy.

The [router](../../../../../router.md) must update the [IPv4](../../../../../ipv4.md) header [checksum](../../../../../checksum.md), and any affected [TCP](../../../../../transmission-control-protocol.md) or [UDP](../../../../../user-datagram-protocol.md) [checksum](../../../../../checksum.md): transport checking includes the relevant [IP addresses](../../../../../ip-address.md) as well as the transport header. Bindings may be allocated dynamically and removed after inactivity or observed termination. Traffic for a live exchange must traverse a translator that possesses the binding, or equivalent shared information.

An unsolicited incoming [packet](../../../../../network-packet.md) generally has no dynamic inverse mapping, so exposing a private service usually needs a configured mapping or [port forwarding](../../../../../port-forwarding.md). Application data that embeds a private [IP address](../../../../../ip-address.md) can also need special handling. Address translation saves public address space, but changes the addressing visible to the two [endpoints](../../../../../communication-endpoint.md) and can disrupt an exchange if its mapping disappears. Its essential mechanism is

$$
\boxed{\text{rewrite outbound addresses/ports; remember the binding; invert it on replies}.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Computer networks](../../../computer-networks-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
