# Log Analysis Report – SSH Login Activity

## Overview

This analysis reviews SSH login activity to identify suspicious behavior and potential unauthorized access attempts.

## Log Source

* Linux authentication logs (/var/log/auth.log)

## Key Findings

* Multiple failed login attempts from IP: 203.0.113.45
* Attempts targeted user: root
* Activity occurred rapidly over a short time period

## Analysis

The pattern of repeated failed logins suggests a brute-force attempt to gain access via SSH.

## Indicators of Compromise (IOCs)

* IP Address: 203.0.113.45
* Repeated failed authentication attempts

## Recommended Actions

* Disable root SSH login
* Implement fail2ban or account lockout policies
* Block suspicious IP address

## Tools Used

* Log review (Linux)
* Basic command-line analysis

## Conclusion

No successful login detected, but activity indicates an attempted unauthorized access requiring mitigation.
