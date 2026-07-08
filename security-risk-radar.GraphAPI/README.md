
Goal: Detect risky Microsoft 365 activity and produce a security report.

Example detections:

Detection	Graph data source	Why it matters
High-risk sign-ins	/auditLogs/signIns	Finds suspicious login behavior
Risky users	/identityProtection/riskyUsers	Shows compromised or suspicious accounts
Defender incidents	/security/incidents	Pulls active security incidents from Microsoft 365 Defender
Conditional Access gaps	/identity/conditionalAccess/policies	Checks whether MFA/block policies exist
Weak MFA posture	/users/{id}/authentication/methods	Finds users without strong auth methods
Risky OAuth apps	oauth2PermissionGrants, appRoleAssignments	Finds over-permissioned enterprise apps
