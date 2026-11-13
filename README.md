# Personal homelab
Ubuntu Server running on an old, unused Lenovo IdeaPad 100S, providing network wide ad blocking for every device on the home network.

---

## Hardware

Lenovo IdeaPad 100S. Low power draw, quiet, & otherwise unused. Repurposing it avoided buying a Raspberry Pi and put already owned hardware to use.

---

## Software

**Ubuntu Server**

- No desktop environment, so almost all of the machine's limited memory goes to services.
- Managed over SSH.

**Pi-hole**

- DNS level ad blocking for the whole network, not per device.
- Every device gets it automatically, including phones and smart TVs that cannot run an ad blocker of their own.
- The router points at the Pi-hole for DNS, so no client configuration is needed.

---

## Why a DNS level blocker?

A browser extension only protects that browser on that device. Blocking at DNS means the request never leaves the network, so it covers every device and every app.

---

## License

MIT. See `LICENSE`.
