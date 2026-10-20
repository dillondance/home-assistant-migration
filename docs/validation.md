# Post-migration validation checklist

This checklist distinguishes checks observed during the migration from recommended repeatable checks.

| Check | Observed during migration | Recommended for repeat tests |
| --- | --- | --- |
| HAOS VM boots to ready state | Yes | Yes |
| Home Assistant UI accessible after restore | Yes | Yes |
| Existing login works | Yes | Yes |
| Attached devices/connectivity restored | Yes | Yes |
| USB/serial passthrough configured | Yes | Yes |
| Memory usage visible in HA and NAS interface | Yes | Yes |
| Full scheduled backup and test restore | Not documented | Yes |
| Recovery-time objective measured | Not documented | Yes |

Avoid uploading screenshots showing automation names, individual devices, hostnames, integrations with account IDs, or server configuration details.
