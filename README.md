# targeted-dirbusting-wordlist-read-me
10,631 targeted paths for Gobuster, ffuf &amp; directory busting built for bug bountys, food delivery APIs, sensitive files, config leaks &amp; more.

## Recon Wordlist

10,631 targeted paths for directory busting, API fuzzing, and endpoint discovery.

Works with Gobuster, ffuf, or any tool that takes a wordlist.

## Coverage

This isn't just a generic dirbusting list. It covers common web directories, admin panels, Ruby on Rails internals (Sidekiq, ActiveStorage, Blazer), Go debug endpoints (pprof, metrics), food delivery and e-commerce paths (orders, carts, menus, restaurants, delivery tracking), sensitive file discovery (.env, .git, backups, configs, credentials), API versioned routes across v1 through v4, cloud and AWS paths, CI/CD tooling, Spring Boot Actuator, Elasticsearch, Grafana, Kibana, auth flows (OAuth, SAML, OIDC), and over 600 compound path variations.

## Usage

```
gobuster dir -u https://TARGET -w eternal_wordlist.txt --threads 1 --delay 1000ms
```

```
ffuf -u https://TARGET/FUZZ -w eternal_wordlist.txt -rate 1 -t 1
```

Rate limit your tools. One request per second is plenty and keeps you out of trouble.

## Disclaimer

This wordlist is provided strictly for authorized security research and educational purposes only.

Do not use this against any target without explicit authorization. The author takes no responsibility for misuse, damage, or illegal activity resulting from the use of this wordlist. Always follow responsible disclosure guidelines and all applicable laws in your jurisdiction. Unauthorized access to computer systems is illegal and may violate the Computer Fraud and Abuse Act (CFAA) or equivalent laws where you live.

By downloading or using this wordlist, you accept full responsibility for your actions.

## License

MIT
