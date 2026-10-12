<div align="center">

# `> whoami`

**Security Engineering · Identity · Detection · Automatisierung**

</div>

```console
$ nmap -Pn -p- i3iker
Starting Nmap 7.95 ( https://nmap.org ) at 2026-10-12 13:37 CEST
Nmap scan report for i3iker
All 65535 scanned ports on i3iker are in ignored states.
Not shown: 65535 filtered tcp ports (no-response)

Nmap done: 1 IP address (1 host up) scanned in 1337.42 seconds
```

```kql
I3iker
| where Focus has_any ("Entra ID", "Defender XDR", "Sentinel", "KQL", "Proxmox")
| extend Motto = "Was nicht als Code existiert, driftet."
| project-away Kunden, Tenants, IPs, Details
```

```yaml
# /etc/i3iker.conf
clickops: disabled
gates: fail-closed       # grün ohne Prüfung = Exit 1
rollout: report-only     # erst messen, dann scharf
homelab: rebuilding      # wie immer
coffee: required
```

<div align="center">
<sub>Repos: privat · Details: auf Anfrage · Alles andere: <code>403 Forbidden</code></sub>
</div>

<!-- nice try. -->
