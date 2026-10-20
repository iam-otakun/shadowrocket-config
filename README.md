# shadowrocket-config

Shadowrocket split-routing config for personal use. **Rules only — contains no node credentials, subscriptions, or keys.**

## Import

Shadowrocket -> Config -> + -> Import from URL:

```
https://raw.githubusercontent.com/iam-otakun/shadowrocket-config/main/Shadowrocket-Fred.conf
```

Set it as the active config after importing. To update later, tap the update/download action on this config in Shadowrocket — it re-fetches the latest version from this repo.

## Contents

- Split rules ported from a mihomo (Clash Meta) config: domestic/Alibaba direct, AI services via US group, everything else via proxy, GEOIP CN direct fallback.
- DNS anti-leak: IP-form DoH only (1.1.1.1 / 8.8.8.8), no system resolver, hijack-dns for hardcoded DNS, IPv6 off.
- Nodes are NOT in this file: proxy groups collect imported nodes by name pattern automatically.
