# TODO

- Some domains don't seem to be supported such as gq with current whois server
    - A potential fix: use a list of whois servers such as `https://github.com/whois-server-list/whois-server-list`
- Add file input
- A potentially better way to do this: do a dns lookup. If the name does not resolve to an ip, do a whois lookup
- Let users specify whois servers `--servers server1,server2,server3`