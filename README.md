log
Failed password for admin from 192.168.1.10
Accepted password for admin from 192.168.1.10

Multiple failed login attempts were detected from the same IP address, followed by a successful login.
This indicates a brute force attack leading to account compromise.

IF failed_login > 5 AND success_login
THEN brute_force_attack

Incident Type: Brute Force Attack

Target: SSH (admin user)

Findings:
- Multiple failed login attempts
- Successful login after failures

Risk: High

Recommendation:
- Enable account lockout
- Use MFA
