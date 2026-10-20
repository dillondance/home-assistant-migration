# Security and privacy considerations

## Applied publication safeguards
- No secrets, tokens, passwords, SSL private keys, database files, or Home Assistant backups committed.
- No identifiable local or public IP addresses, serial numbers, device identifiers, private hostnames, or usernames shared.
- Architecture depicted at a functional level.

## Operational controls worth validating
The following are **recommendations**, not assertions about the current lab:
- Restrict administrative access and require strong authentication.
- Keep Home Assistant OS and NAS firmware updated.
- Maintain protected, tested backups.
- Limit unnecessary network exposure and inspect access paths before enabling remote access.
- Review repository files and screenshots for hidden metadata before publication.
