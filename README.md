# securityonion-filters-rules
Custom filters.rules file used by the so-suricata metadata engine
## Improvements
- If you read the article referenced in most of the ESET rules, it specifies the appliance needs to resolve the hostnames. If you can add that variable and modify the rule you can make the whitelist more exact.
- All of the rules use case-insensitive pcre (/i), but perhaps some rules could be case sensitive because official applications should be using the exact domain/uri
- Rules that are mutually exclusive (ex. one for a different version of a product) have the same sid. If that is not best practice that can be changed
# ESET Detections
- sid: 1200001 - 065
# Benign WIndows Network Behavior
- sid: 12000101 - 103
# Kaspersky Detections
- sid: 12000201 - 203