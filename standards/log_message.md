# Log Message Standard

The key words “MUST”, “MUST NOT”, “REQUIRED”, “SHALL”, “SHALL NOT”, “SHOULD”, “SHOULD NOT”, “RECOMMENDED”, “MAY”, and “OPTIONAL” in this document are to be interpreted as described in [RFC 2119](http://www.ietf.org/rfc/rfc2119.txt).

The message format MUST be JSON.

The message MUST contain the following top-level keys: `level`, `message`:
- `level` MUST be a **string** of of one of the following values (case-sensitive) and MUST follow this order of severity (from least to greatest): `DEBUG`, `INFO`, `NOTICE`, `WARNING`, `ERROR`, `CRITICAL`, `ALERT`, or `EMERGENCY`.
- `message` MUST be a **string** and SHOULD contain a message useful for debugging/error reporting.

Additional key/values of any type MAY be included and MUST NOT break functionality.