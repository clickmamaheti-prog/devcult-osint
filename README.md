# DevCult OSINT Tool v3.0

**Professional Email Intelligence Platform** — by **DevCult XII**

Tool OSINT untuk menganalisis 1 email target secara mendalam. Breach history, DNS analysis, platform footprint, threat intel, risk scoring — all in one shot.

## Fitur

| Fitur | Deskripsi |
|-------|-----------|
| **Breach Intel** | HaveIBeenPwned + LeakCheck |
| **Identity Correlation** | GitHub profile, repos, gists, orgs |
| **Domain Analysis** | DNS / MX / SPF / DKIM / DMARC / BIMI / DNSSEC |
| **WHOIS** | Registrar, creation date, expiry, org |
| **IP & ASN** | Geolocation, ASN, reverse DNS |
| **Shodan** | Open ports, vulnerabilities, banners |
| **Wayback Machine** | Historical domain snapshots |
| **Platform Footprint** | 33+ sites via username correlation |
| **DNSBL Blacklist** | 9 blacklist zones |
| **Threat Intel** | AbuseIPDB reputation score |
| **Risk Scoring** | Automated threat assessment (0-100) |
| **Export** | JSON / CSV |

## Instalasi

```bash
pip install rich requests dnspython python-whois
```

## Penggunaan

```bash
# Interactive mode
python devcult_osint.py

# Single target
python devcult_osint.py -e target@example.com

# Single target + JSON export
python devcult_osint.py -e target@example.com --export json

# Bulk scan from file
python devcult_osint.py --bulk emails.txt --export csv
```

## API Keys (opsional)

| Key | Source | Unlocks |
|-----|--------|---------|
| `HIBP_API_KEY` | haveibeenpwned.com | Breach & paste lookup |
| `SHODAN_API_KEY` | shodan.io | Port/vuln scan |
| `LEAKCHECK_KEY` | leakcheck.io | Additional breach DB |
| `ABUSEIPDB_KEY` | abuseipdb.com | IP reputation |

```bash
export HIBP_API_KEY=your_key_here
export SHODAN_API_KEY=your_key_here
```

---

**Made by DevCult XII**
