# shadowrocket-config

Shadowrocket split-routing config for personal use. **Rules only — contains no node credentials, subscriptions, or keys.**

## Import

Shadowrocket -> Config -> + -> Import from URL:

```
https://raw.githubusercontent.com/iam-otakun/shadowrocket-config/main/Shadowrocket-Fred.conf
```

Set it as the active config after importing, then pick a node on the home page — all proxy traffic uses that selected node (built-in PROXY policy). To update later, tap the update action on this config in Shadowrocket; it re-fetches the latest version from this repo.

## Design (v2)

- Skeleton: Mini-AntiLeak [General]/DNS + ACL4SSR rule sets (proven in daily use).
- No proxy groups anywhere: v1's regex-built groups stayed empty in Shadowrocket and black-holed all foreign traffic. FINAL points at the built-in PROXY instead.
- Inline lists ported from a mihomo config: Alibaba ecosystem direct (39 domains), AI services (23 domains) to PROXY — every node in the setup is US-based, so AI region requirements are satisfied by any selected node.
- overbridgenet.com hard-rejected at the top.
