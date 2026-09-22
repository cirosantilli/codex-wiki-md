# Computer network

↑ **Parent:** [Computer science](computer-science.md)

A [computer network](computer-network.md) connects computing devices so they can exchange data using [communication protocols](#communication-protocol). [Packet switching](#packet-switching) shares communication links among many exchanges; [routers](#router) forward [network packets](#network-packet) between connected networks. The arrangement of machines and links need not coincide with the arrangement of administrative control.

**Table of contents**

- [Ring network](#ring-network)
- [Unicast](#unicast)
- [Multicast](#multicast)
- [Line code](#line-code)
  - [Block code for line coding](#block-code-for-line-coding)
  - [Differential Manchester encoding](#differential-manchester-encoding)
  - [Manchester code](#manchester-code)
  - [Clock recovery](#clock-recovery)
- [Symbol rate](#symbol-rate)
- [Bit rate](#bit-rate)
- [Network latency](#network-latency)
  - [Round-trip time](#round-trip-time)
- [Router](#router)
- [Packet switching](#packet-switching)
  - [Network packet](#network-packet)
- [Layered network architecture](#layered-network-architecture)
  - [Data link layer](#data-link-layer)
    - [Framing](#framing)
      - [Bit stuffing](#bit-stuffing)
      - [Frame delimiter](#frame-delimiter)
    - [Frame (networking)](#frame-networking)
  - [Transport protocol](#transport-protocol)
    - [Flow control](#flow-control)
      - [Backpressure](#backpressure)
    - [Sliding window protocol](#sliding-window-protocol)
      - [Receive window](#receive-window)
      - [Send window](#send-window)
    - [Acknowledgement](#acknowledgement)
      - [Delayed acknowledgement](#delayed-acknowledgement)
    - [Transport sequence number](#transport-sequence-number)
    - [Retransmission (data networks)](#retransmission-data-networks)
    - [Transport port](#transport-port)
    - [QUIC](#quic)
    - [User Datagram Protocol](#user-datagram-protocol)
    - [Transmission Control Protocol](#transmission-control-protocol)
      - [Zero-window probe](#zero-window-probe)
        - [Persist timer](#persist-timer)
      - [Silly window syndrome](#silly-window-syndrome)
        - [Nagle's algorithm](#nagle-s-algorithm)
      - [TCP segment](#tcp-segment)
- [Internet](#internet)
  - [Content delivery network](#content-delivery-network)
    - [CDN edge](#cdn-edge)
  - [Domain Name System](#domain-name-system)
  - [Internet Protocol](#internet-protocol)
    - [IP multicast](#ip-multicast)
      - [Multicast routing](#multicast-routing)
        - [Reverse path forwarding](#reverse-path-forwarding)
        - [Multicast distribution tree](#multicast-distribution-tree)
    - [IPv6](#ipv6)
    - [IPv4](#ipv4)
    - [IP address](#ip-address)
  - [Internet architecture](#internet-architecture)
    - [Internet service federation](#internet-service-federation)
    - [Middlebox](#middlebox)
      - [Proxy server](#proxy-server)
      - [Firewall](#firewall)
      - [Network address translation](#network-address-translation)
        - [Network address and port translation](#network-address-and-port-translation)
          - [Port forwarding](#port-forwarding)
    - [Fate-sharing](#fate-sharing)
    - [IP hourglass](#ip-hourglass)
    - [Network decentralisation](#network-decentralisation)
      - [Geographical replication does not imply decentralised control](#geographical-replication-does-not-imply-decentralised-control)
    - [End-to-end principle](#end-to-end-principle)
      - [Application correctness is not determined by a network trace](#application-correctness-is-not-determined-by-a-network-trace)
- [Communication protocol](#communication-protocol)
  - [Application-layer acknowledgement](#application-layer-acknowledgement)
  - [Communication endpoint](#communication-endpoint)
  - [Protocol ossification](#protocol-ossification)

## Ring network

↑ **Parent:** [Computer network](computer-network.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Ring_network)

A [computer network](computer-network.md) with nodes connected around a cycle. A unidirectional [ring network](#ring-network) permits messages to move only in the chosen direction.

## Unicast

↑ **Parent:** [Computer network](computer-network.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Unicast)

[Unicast](#unicast) addresses a transmission to a single destination, in contrast with group-addressed [multicast](#multicast) delivery.

## Multicast

↑ **Parent:** [Computer network](computer-network.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Multicast)

[Multicast](#multicast) delivers data to a group of interested receivers. A [multicast distribution tree](#multicast-distribution-tree) can share transmissions over common links and copy them where routes branch.

## Line code

↑ **Parent:** [Computer network](computer-network.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Line_code)

A [line code](#line-code) maps data to a sequence of physical signal levels or transitions for transmission. Timing, polarity and the length of runs of equal levels affect the choice.

### Block code for line coding

↑ **Parent:** [Line code](#line-code)

A [block code for line coding](#block-code-for-line-coding) maps fixed-size groups of data [bits](information-theory.md#bit) to fixed-size transmitted [codewords](coding-theory.md#codeword), chosen to meet signal constraints as well as to distinguish inputs. Constraints on long runs must also be checked across word boundaries.

### Differential Manchester encoding

↑ **Parent:** [Line code](#line-code)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Differential_Manchester_encoding)

[Differential Manchester encoding](#differential-manchester-encoding) has a transition at every [bit](information-theory.md#bit) midpoint and encodes the data by the presence or absence of a boundary transition. A consistent signal polarity reversal preserves those transition decisions.

### Manchester code

↑ **Parent:** [Line code](#line-code)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Manchester_code)

[Manchester encoding](#manchester-code) represents each data [bit](information-theory.md#bit) by two opposite half-bit levels. The compulsory midpoint transition supports [clock recovery](#clock-recovery).

### Clock recovery

↑ **Parent:** [Line code](#line-code)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Clock_recovery)

[Clock recovery](#clock-recovery) extracts a timing reference from a received signal so that a receiver can locate symbol boundaries.

## Symbol rate

↑ **Parent:** [Computer network](computer-network.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Symbol_rate)

The [symbol rate](#symbol-rate), measured in baud, counts signal elements per second. Its relation to [bit rate](#bit-rate) depends on the representation and on which signal element is counted as a symbol.

## Bit rate

↑ **Parent:** [Computer network](computer-network.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Bit_rate)

The [bit rate](#bit-rate) counts transmitted data [bits](information-theory.md#bit) per unit time. State which representation is being counted: payload [bits](information-theory.md#bit) and encoded link [bits](information-theory.md#bit) need not have the same rate.

## Network latency

↑ **Parent:** [Computer network](computer-network.md)

[Network latency](#network-latency) is the delay associated with communication over a network, distinguished from the rate at which data can be transferred. Moving a delivery [endpoint](#communication-endpoint) closer to demand can reduce some path delay, but does not by itself establish application correctness or independent control.

### Round-trip time

↑ **Parent:** [Network latency](#network-latency)

The [round-trip time](#round-trip-time) measures the elapsed time for an exchange to travel to a peer and for a response to return. Feedback-based sending can be limited by this delay as well as by link capacity.

## Router

↑ **Parent:** [Computer network](computer-network.md)

A [router](#router) forwards [network packets](#network-packet) between networks using forwarding information. Ordinary [Internet Protocol](#internet-protocol) forwarding is distinct from a [middlebox](#middlebox) function that translates addresses, terminates a transport connection or applies an application-specific transformation.

## Packet switching

↑ **Parent:** [Computer network](computer-network.md)

[Packet switching](#packet-switching) carries separately represented units of data over shared communication links. Different [packets](#network-packet) can share forwarding resources; the network service need not reserve one dedicated circuit for an entire application exchange.

### Network packet

↑ **Parent:** [Packet switching](#packet-switching)

A [network packet](#network-packet) carries a unit of data together with [protocol](#communication-protocol) information used to interpret or deliver it. [Internet Protocol](#internet-protocol) carries datagrams; transport and application messages can span several such [packets](#network-packet).

## Layered network architecture

↑ **Parent:** [Computer network](computer-network.md)

A [layered network architecture](#layered-network-architecture) separates responsibilities behind communication interfaces. A [transport protocol](#transport-protocol) can offer an application a service built over [Internet Protocol](#internet-protocol) without requiring each underlying network to implement that application. Layer boundaries are engineering choices: the [end-to-end principle](#end-to-end-principle) helps assess which properties a lower layer can actually establish.

### Data link layer

↑ **Parent:** [Layered network architecture](#layered-network-architecture)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Data_link_layer)

The [data link layer](#data-link-layer) organizes communication over a link, typically using [data-link frames](#frame-networking) and local checking or access rules.

#### Framing

↑ **Parent:** [Data link layer](#data-link-layer)

[Framing](#framing) identifies the boundaries of [data-link frames](#frame-networking) in a transmitted stream, allowing a receiver to locate separately interpretable link-level units.

##### Bit stuffing

↑ **Parent:** [Framing](#framing)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Bit_stuffing)

[Bit stuffing](#bit-stuffing) inserts extra [bits](information-theory.md#bit) according to an agreed rule, for example after five consecutive ones, so that a reserved [frame delimiter](#frame-delimiter) cannot occur inside encoded contents. The receiver reverses the insertion rule.

##### Frame delimiter

↑ **Parent:** [Framing](#framing)

A [frame delimiter](#frame-delimiter) marks a [data-link frame](#frame-networking) boundary. A transparency rule such as [bit stuffing](#bit-stuffing) prevents data from accidentally imitating the reserved delimiter.

#### Frame (networking)

↑ **Parent:** [Data link layer](#data-link-layer)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Frame_(networking))

A [data-link frame](#frame-networking) is a delimited unit of link-level transmission containing data and any associated control or checking fields.

### Transport protocol

↑ **Parent:** [Layered network architecture](#layered-network-architecture)

A [transport protocol](#transport-protocol) provides communication services between its transport [endpoints](#communication-endpoint) over an underlying network. [Transmission Control Protocol](#transmission-control-protocol) supplies a reliable ordered byte stream; [User Datagram Protocol](#user-datagram-protocol) supplies datagrams without that built-in recovery service. Applications can implement further mechanisms over either interface.

#### Flow control

↑ **Parent:** [Transport protocol](#transport-protocol)

[Flow control](#flow-control) limits a sender according to a receiver's buffering or processing capacity, rather than the capacity of the intervening [computer network](computer-network.md).

##### Backpressure

↑ **Parent:** [Flow control](#flow-control)

A dependency by which an unready receiver delays upstream acceptance of further work. In [synchronous message passing](operating-system.md#synchronous-message-passing) it can propagate through a chain of blocked sends; a finite buffer postpones this propagation until its capacity is used.

#### Sliding window protocol

↑ **Parent:** [Transport protocol](#transport-protocol)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Sliding_window_protocol)

A [sliding window protocol](#sliding-window-protocol) permits a range of numbered data to be outstanding or accepted, advancing that range as transmission makes progress.

##### Receive window

↑ **Parent:** [Sliding window protocol](#sliding-window-protocol)

A [receive window](#receive-window) bounds the numbered data a receiver is prepared to accept. In [TCP](#transmission-control-protocol), the receiver advertises a window that limits the sender independently of the sender's [congestion window](queueing-theory.md#congestion-window).

##### Send window

↑ **Parent:** [Sliding window protocol](#sliding-window-protocol)

A [send window](#send-window) specifies the numbered data a sender may transmit before further progress permits the range to advance.

#### Acknowledgement

↑ **Parent:** [Transport protocol](#transport-protocol)

An [acknowledgement](#acknowledgement) reports receipt according to the [protocol](#communication-protocol)'s rules. A [TCP](#transmission-control-protocol) cumulative [acknowledgement](#acknowledgement) names the next expected [byte](computer-memory.md#byte); it does not establish that the application has durably acted on all preceding data.

##### Delayed acknowledgement

↑ **Parent:** [Acknowledgement](#acknowledgement)

A [delayed acknowledgement](#delayed-acknowledgement) postpones a response briefly so that one [acknowledgement](#acknowledgement) may cover more data or accompany returning data. Its timer can interact with [Nagle's algorithm](#nagle-s-algorithm) to delay a short exchange.

#### Transport sequence number

↑ **Parent:** [Transport protocol](#transport-protocol)

A [transport sequence number](#transport-sequence-number) identifies a data position within an exchange, supporting ordering, duplicate rejection and precise [acknowledgements](#acknowledgement). [TCP](#transmission-control-protocol) numbers [bytes](computer-memory.md#byte) rather than simply numbering [packets](#network-packet).

#### Retransmission (data networks)

↑ **Parent:** [Transport protocol](#transport-protocol)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Retransmission_(data_networks))

[Data retransmission](#retransmission-data-networks) sends data again to recover from loss or detected corruption. [Transport sequence numbers](#transport-sequence-number) let a receiver recognize a duplicate if the original transmission arrived but its [acknowledgement](#acknowledgement) was lost.

#### Transport port

↑ **Parent:** [Transport protocol](#transport-protocol)

A [transport port](#transport-port) is a numbered identifier used by a [transport protocol](#transport-protocol) to distinguish communication [endpoints](#communication-endpoint) at a host. [TCP](#transmission-control-protocol) and [UDP](#user-datagram-protocol) have separate port spaces.

#### QUIC

↑ **Parent:** [Transport protocol](#transport-protocol)

[QUIC](#quic) is a [transport protocol](#transport-protocol) designed over [User Datagram Protocol](#user-datagram-protocol) with multiple streams and cryptographic protection. At the 17 January 2020 examination date, the cited November 2019 design was an Internet-Draft and work in progress. This historical description does not treat a later standard as already available.[4 November 2019, §1 and Status of This Memo](computer-science-bibliography.md#quic-a-udp-based-multiplexed-and-secure-transport-internet-draft-24)

#### User Datagram Protocol

↑ **Parent:** [Transport protocol](#transport-protocol)

[User Datagram Protocol](#user-datagram-protocol) supplies a datagram transport interface without built-in reliable ordered-stream delivery. An application or another [protocol](#communication-protocol) can add recovery over that interface, as the pre-2020 [QUIC](#quic) design illustrates.

#### Transmission Control Protocol

↑ **Parent:** [Transport protocol](#transport-protocol)

[Transmission Control Protocol](#transmission-control-protocol) provides a reliable ordered byte-stream service between its [endpoints](#communication-endpoint), using sequencing, acknowledgements and retransmission. Receipt by that transport does not establish that a receiving application has durably stored the data or completed a user operation.[§§1.5 and 2.6: operation and reliable communication](computer-science-bibliography.md#transmission-control-protocol-rfc-793)

##### Zero-window probe

↑ **Parent:** [Transmission Control Protocol](#transmission-control-protocol)

A [zero-window probe](#zero-window-probe) solicits a current [receive window](#receive-window) advertisement when a sender has been stopped by a zero window. Repeated probes recover from a lost reopening [acknowledgement](#acknowledgement).

###### Persist timer

↑ **Parent:** [Zero-window probe](#zero-window-probe)

The [persist timer](#persist-timer) schedules repeated [zero-window probes](#zero-window-probe), preventing an exchange from waiting forever after a window-reopening message is lost.

##### Silly window syndrome

↑ **Parent:** [Transmission Control Protocol](#transmission-control-protocol)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Silly_window_syndrome)

[Silly window syndrome](#silly-window-syndrome) is inefficient transmission in tiny [TCP segments](#tcp-segment), arising through small writes or small increments of advertised receiving space. Sender and receiver measures address different causes.

<h6 id="nagle-s-algorithm">Nagle's algorithm</h6>

↑ **Parent:** [Silly window syndrome](#silly-window-syndrome)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Nagle's_algorithm)

[Nagle's algorithm](#nagle-s-algorithm) coalesces small writes while data are unacknowledged, permitting another send when a full [TCP segment](#tcp-segment) can be formed or the outstanding data have been acknowledged. It reduces tiny transmissions but can add delay.

##### TCP segment

↑ **Parent:** [Transmission Control Protocol](#transmission-control-protocol)

A [TCP segment](#tcp-segment) contains a [TCP](#transmission-control-protocol) header and zero or more data [bytes](computer-memory.md#byte). The header carries sequencing, [acknowledgement](#acknowledgement) and [receive window](#receive-window) information.

## Internet

↑ **Parent:** [Computer network](computer-network.md)

The [Internet](#internet) interconnects independently operated [computer networks](computer-network.md) using the [Internet Protocol](#internet-protocol) suite. Its common inter-network interface supports diverse underlying networks and applications; individual services can still depend on centrally controlled providers.

### Content delivery network

↑ **Parent:** [Internet](#internet)

A [content delivery network](#content-delivery-network) uses delivery infrastructure, often at multiple locations, to supply content and direct requests to suitable delivery [endpoints](#communication-endpoint). It can retain objects through [caching](computer-memory.md#caching) or retrieve them from an origin. Distribution across sites does not imply that those sites have independent administrative control.[§1.2 and §2.1: reference model and request redirection](computer-science-bibliography.md#framework-for-content-distribution-network-interconnection-rfc-7336)

#### CDN edge

↑ **Parent:** [Content delivery network](#content-delivery-network)

A [CDN edge](#cdn-edge) is a delivery [endpoint](#communication-endpoint) of a [content delivery network](#content-delivery-network). It may use [caching](computer-memory.md#caching) or fetch content, and a provider can authorise it to terminate a [client](computer-science.md#network-client) connection. Its location near demand and its administrative authority are separate properties.

### Domain Name System

↑ **Parent:** [Internet](#internet)

The [Domain Name System](#domain-name-system) provides a hierarchical namespace with delegated administration and distributed [servers](computer-science.md#network-server). Caching and replication help supply its service. A consistent namespace is compatible with distribution of responsibility across organisations.[§2.2, §3 and §4.2: goals, namespace and zones](computer-science-bibliography.md#domain-names-concepts-and-facilities-rfc-1034)

### Internet Protocol

↑ **Parent:** [Internet](#internet)

[Internet Protocol](#internet-protocol) supplies an inter-network datagram interface. Its basic [packet](#network-packet) delivery does not itself guarantee arrival, order, absence of duplicates or completion of an application operation. [IPv4](#ipv4) and [IPv6](#ipv6) are versions of this network-layer [protocol](#communication-protocol).

#### IP multicast

↑ **Parent:** [Internet Protocol](#internet-protocol)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/IP_multicast)

[IP multicast](#ip-multicast) sends an [Internet Protocol](#internet-protocol) datagram to a group identified by a multicast [IP address](#ip-address). Delivery retains the underlying best-effort nature of [Internet Protocol](#internet-protocol).

##### Multicast routing

↑ **Parent:** [IP multicast](#ip-multicast)

[Multicast routing](#multicast-routing) establishes and maintains the forwarding decisions that deliver group-addressed [packets](#network-packet) to interested receivers.

###### Reverse path forwarding

↑ **Parent:** [Multicast routing](#multicast-routing)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Reverse_path_forwarding)

[Reverse path forwarding](#reverse-path-forwarding) accepts a source's [multicast](#multicast) traffic only on the interface selected for the reverse route to that source. With consistent loop-free routing, those parent choices define a source-rooted [tree](tree-graph-theory.md). Membership pruning can then remove unneeded branches.

###### Multicast distribution tree

↑ **Parent:** [Multicast routing](#multicast-routing)

A [multicast distribution tree](#multicast-distribution-tree) describes the parent and outgoing branches used to distribute [packets](#network-packet) to a group. Source-rooted and shared-group designs make different state and path choices.

#### IPv6

↑ **Parent:** [Internet Protocol](#internet-protocol)

[IPv6](#ipv6) uses 128-bit addresses and a revised [packet](#network-packet) format. More address space does not remove [firewalls](#firewall) or decide which application providers must be trusted.[§1: expanded addressing and other protocol changes](computer-science-bibliography.md#internet-protocol-version-6-ipv6-specification-rfc-8200)

#### IPv4

↑ **Parent:** [Internet Protocol](#internet-protocol)

[IPv4](#ipv4) uses 32-bit addresses. Address sharing through [network address and port translation](#network-address-and-port-translation) is one response to pressure on its globally usable address space.

#### IP address

↑ **Parent:** [Internet Protocol](#internet-protocol)

An [IP address](#ip-address) identifies an interface or destination according to the relevant [Internet Protocol](#internet-protocol) addressing rules. It is not inherently the identity of a person, and address translation can change the address visible across a boundary.

### Internet architecture

↑ **Parent:** [Internet](#internet)

The [Internet architecture](#internet-architecture) comprises its [protocol](#communication-protocol) interfaces, addressing and naming arrangements, placement of functions and assumptions about communication. Physical connectivity, administrative control and application trust are distinct dimensions of this architecture.[§§2–3: internetwork layer and design issues](computer-science-bibliography.md#architectural-principles-of-the-internet-rfc-1958)

#### Internet service federation

↑ **Parent:** [Internet architecture](#internet-architecture)

[Internet service federation](#internet-service-federation) permits independently administered services to communicate through agreed [protocols](#communication-protocol). [Internet](#internet) mail is an example: separate domains can exchange messages without every user joining one provider. Federation differs from placing many replicas behind one mandatory account authority, and it does not itself establish [cryptographic confidentiality](computer-science.md#cryptographic-confidentiality) or freedom from software failures.[§§2.1–2.3: communication model and domain-based delivery](computer-science-bibliography.md#simple-mail-transfer-protocol-rfc-5321)

#### Middlebox

↑ **Parent:** [Internet architecture](#internet-architecture)

A [middlebox](#middlebox) performs a function on a communication path beyond ordinary [Internet Protocol](#internet-protocol) forwarding, such as address translation, traffic filtering or proxying. The function can be embedded in a device rather than implemented in a separate physical box. Its state and assumptions can affect failure recovery and [protocol](#communication-protocol) evolution.[§1.1 and §4: definition and architectural issues](computer-science-bibliography.md#middleboxes-taxonomy-and-issues-rfc-3234)

##### Proxy server

↑ **Parent:** [Middlebox](#middlebox)

A [proxy server](#proxy-server) performs communication operations on behalf of another participant. Whether it can inspect plaintext depends on the [protocols](#communication-protocol) and keys it uses: relaying opaque encrypted bytes differs from authorised [TLS termination](computer-science.md#tls-termination).

##### Firewall

↑ **Parent:** [Middlebox](#middlebox)

A [firewall](#firewall) enforces a communication policy, for example by filtering [packets](#network-packet) or tracking permitted exchanges. Blocking unwanted incoming traffic is a policy decision; it is not the definition of [network address translation](#network-address-translation).

##### Network address translation

↑ **Parent:** [Middlebox](#middlebox)

[Network address translation](#network-address-translation) maps [IP addresses](#ip-address) between address realms. State and path constraints can affect sessions. [Network address and port translation](#network-address-and-port-translation) additionally maps transport ports. Translation does not itself require decryption of application payloads.[Abstract and §§1–2: address and port translation, state and limitations](computer-science-bibliography.md#traditional-ip-network-address-translator-traditional-nat-rfc-3022)

###### Network address and port translation

↑ **Parent:** [Network address translation](#network-address-translation)

[Network address and port translation](#network-address-and-port-translation) permits several internal addresses and transport ports to share an external address by maintaining distinct translated bindings. Losing a binding can disrupt an exchange even when the application [endpoints](#communication-endpoint) retain their own state.

###### Port forwarding

↑ **Parent:** [Network address and port translation](#network-address-and-port-translation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Port_forwarding)

[Port forwarding](#port-forwarding) configures a mapping from an external [transport port](#transport-port) to an internal service, allowing selected inbound traffic through a translator.

#### Fate-sharing

↑ **Parent:** [Internet architecture](#internet-architecture)

[Fate-sharing](#fate-sharing) places state needed by a communicating [endpoint](#communication-endpoint) with that [endpoint](#communication-endpoint), so that failure of an unrelated forwarding component need not erase the state of an ongoing exchange. This can help communication recover after a route change when a path becomes available again. It does not mean every [router](#router) lacks state or that communication can survive loss of all paths.[§4: survivability and placement of essential connection state](computer-science-bibliography.md#the-design-philosophy-of-the-darpa-internet-protocols-by-david-d-clark)

#### IP hourglass

↑ **Parent:** [Internet architecture](#internet-architecture)

The [IP hourglass](#ip-hourglass) describes a common narrow inter-network layer supporting many applications above it and many network technologies below it. Keeping that interface general limits the need for every application developer and link provider to coordinate separate application-specific changes.[§§2.1–2.4: common internetwork protocol and independence from underlying media](computer-science-bibliography.md#architectural-principles-of-the-internet-rfc-1958)

#### Network decentralisation

↑ **Parent:** [Internet architecture](#internet-architecture)

[Network decentralisation](#network-decentralisation) concerns the distribution of relevant control, authority or indispensable dependencies across independently operated participants. It is a property relative to a specified decision or service: distributed forwarding can coexist with centralised naming, credentials or application data. Counting physical [servers](computer-science.md#network-server) is insufficient.

##### Geographical replication does not imply decentralised control

↑ **Parent:** [Network decentralisation](#network-decentralisation)

Construct a service with replicas in ten locations, all controlled by the same operator and all requiring that operator's account authority. The physical deployment is distributed, but control and the account dependency remain centralised. Increasing the number of sites leaves that counterexample intact. To assess decentralisation, state which operators can independently authorise participation, change [protocol](#communication-protocol) behaviour or preserve service when another operator fails.

#### End-to-end principle

↑ **Parent:** [Internet architecture](#internet-architecture)

When fully implementing a required function needs [endpoint](#communication-endpoint) information, a lower-layer implementation cannot replace [endpoint](#communication-endpoint) responsibility. Lower-layer mechanisms can still improve efficiency. The principle concerns function placement, not a requirement for peer-to-peer topology. [Jerome H. Saltzer](computer-science.md#jerry-saltzer), [David P. Reed](computer-science.md#david-p-reed) and [David D. Clark](computer-science.md#david-d-clark) articulated the argument.[Author-hosted reprint, pp. 1–3: the argument and careful file transfer](computer-science-bibliography.md#end-to-end-arguments-in-system-design-by-jerome-h-saltzer-and-others)

##### Application correctness is not determined by a network trace

↑ **Parent:** [End-to-end principle](#end-to-end-principle)

Suppose an application's required property depends on [endpoint](#communication-endpoint) state that is not determined by the network trace. Consider two executions with identical messages and forwarding behaviour: in one the receiver stores the received byte correctly; in the other it corrupts that byte after reception. The network trace is the same, but the required stored-file correctness differs. Any decision based only on that trace must give the same answer in both executions and therefore cannot establish the property for all executions.

This is an indistinguishability argument for that failure model, not a claim that network checks are useless. A link checksum may reduce transmission errors while an application [endpoint](#communication-endpoint) still has to check the property that spans its storage and processing. Specify the [endpoint](#communication-endpoint) boundary before claiming an end-to-end guarantee.

## Communication protocol

↑ **Parent:** [Computer network](computer-network.md)

A [communication protocol](#communication-protocol) specifies the format and meaning of exchanged messages and the permitted behaviour of participants. Compatibility requires agreement about both message syntax and the state changes that messages cause.

### Application-layer acknowledgement

↑ **Parent:** [Communication protocol](#communication-protocol)

An [application-layer acknowledgement](#application-layer-acknowledgement) confirms a condition specified by an application's [communication protocol](#communication-protocol). Receipt, successful processing and durable storage are different conditions. A [Transmission Control Protocol](#transmission-control-protocol) acknowledgement of received bytes does not itself establish any stronger application promise; the relevant [endpoint](#communication-endpoint) must establish that promise.[Printed p. 7: the SWALLOW example distinguishes message delivery from safe storage](computer-science-bibliography.md#end-to-end-arguments-in-system-design-by-jerome-h-saltzer-and-others)

### Communication endpoint

↑ **Parent:** [Communication protocol](#communication-protocol)

A [communication endpoint](#communication-endpoint) is a participant at the boundary of a specified communication function. Always identify the level: a [TLS](computer-science.md#transport-layer-security) peer, a transport [endpoint](#communication-endpoint) and an application [endpoint](#communication-endpoint) need not represent the same boundary of correctness or trust.

### Protocol ossification

↑ **Parent:** [Communication protocol](#communication-protocol)

[Protocol ossification](#protocol-ossification) occurs when deployed implementations or intermediaries make established behaviour difficult to change, for example by rejecting an unfamiliar transport format or assuming fields will never evolve. [Endpoint](#communication-endpoint) support alone may then be insufficient for deployment over real paths.[§§2–5: interface and middlebox constraints on evolution](computer-science-bibliography.md#report-from-the-iab-workshop-on-stack-evolution-in-a-middlebox-internet-rfc-7663)

## ↑ Ancestors (2)

1. [Computer science](computer-science.md)
2. [Codex Wiki](README.md)

## ← Incoming links (5)

- [Computer network](computer-network.md)
- [Flow control](#flow-control)
- [Internet](#internet)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2015/computer-networks.md#3/b/solution)
- [Ring network](#ring-network)
