# tlsref.org-data

Static data files served at [data.tlsref.org](https://data.tlsref.org), used by [tlsref.org](https://tlsref.org).

## Files

**DH Parameters** — pre-built PEM files for configuring Diffie-Hellman key exchange:

- [`/static/ffdhe2048.txt`](https://data.tlsref.org/static/ffdhe2048.txt) — 2048-bit FFDHE params (RFC 7919)
- [`/static/ffdhe4096.txt`](https://data.tlsref.org/static/ffdhe4096.txt) — 4096-bit FFDHE params (RFC 7919)

**TLSRef Guidelines** — JSON snapshots of the TLSRef guidelines, one file per version (4.0 through 6.0):

- [`/static/guidelines/6.0.json`](https://data.tlsref.org/static/guidelines/6.0.json) — latest
- [`/static/guidelines/CHANGELOG.md`](https://data.tlsref.org/static/guidelines/CHANGELOG.md) — version history

## Tools

`tools/rfc-to-der/` contains a Python script used to generate and validate the DH parameter files from RFC hex values.

```
pip install asn1tools
python tools/rfc-to-der/rfc-to-der.py
```
