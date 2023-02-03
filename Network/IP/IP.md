# IP

## Message Structure

- **Version**: 4 (IPv4) and 6 (IPv6).
- **Differentiate services**: To obtain better services, not generally used.
- **Total length**: Including the head length and the length of the data part.
- **Survival time**: Prevent undelivered(无法交付) data from constantly circled on the Internet.
- **Protocol**: Indicates which protocol the carrying data should be handed over for processing, such as ICMP, TCP, UDP, etc.

## Address Types

- A：(`1.0.0.0`-`126.0.0.0`)
- B：(`128.0.0.0`-`191.255.0.0`)
- C：(`192.0.0.0`-`223.255.255.0`)
- D
- E

## Special IP Address

- `0.0.0.0`：All unclear host and destination networks.
- `255.255.255.255`： Restrict broadcast address. Refers to all hosts in the same broadcast domain and cannot be forwarded by the router.
- `127.0.0.1`：The local address and cannot be sent to the network interface.