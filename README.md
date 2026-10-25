# The VATA Ledger

A public record of verified security findings.

## Adding a row

Add a new finding object to the `findings` array in `findings.json`. Every field is required. The URL must resolve. Update `lastUpdated` to today's date.

```json
{
  "date": "YYYY-MM-DD",
  "finding": "Description of the vulnerability",
  "target": "Product name, versions affected, fix version",
  "severity": "Critical|High|Moderate",
  "reference": "GHSA-xxxx-xxxx-xxxx or CVE-YYYY-NNNNN",
  "url": "https://github.com/owner/repo/security/advisories/GHSA-xxxx-xxxx-xxxx",
  "probe": "Probe name or declared limit",
  "inReport": "Yes|No"
}
```

Rebuild the HTML table. A row without a resolving link does not go live.
