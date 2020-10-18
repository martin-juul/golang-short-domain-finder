# Golang Short Domain Finder

This Golang program will attempt to find available short domains based on a few input parameters such as domain extension and maximum length of domain name

This is useful is you're trying to find short and unique domains.
Particularly for url shortening websites or finding a free subdomain with few letters.

This was originally created to find a short `.me` domain as a student since namecheap offers those.

See [TODO.md](/TODO.md) for a better way to do this

## Requirements

Uses the [whois.go](https://github.com/likexian/whois-go) module.

To install:

`go get -u github.com/likexian/whois-go`

## Usage

```
Usage of ./short-domain-finder:
  -exts string
        List of domain extensions (ie. .com, .io) (default "pw,xyz,dk,es")
  -len int
        Maximum length of domain name (default 3)
  -sep string
        Char used to separate the list of domain extensions (default ",")
  -workers int
        Number of worker to query whois in parallel. Too many may overwhelm the service and get you blocked (default 10)
```

Errors are piped to STDERR, so it's safe to pipe output to a file like so:

```bash
./short-domain-finder > output.txt
```

## Credits

- [https://github.com/fyxme/golang-short-domain-finder](https://github.com/fyxme/golang-short-domain-finder)
- [https://github.com/likexian/whois-go](https://github.com/likexian/whois-go)