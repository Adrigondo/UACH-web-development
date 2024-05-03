For a model `USER`
| CRUD   | HTTP Protocol | URL          | Function |
| ------ | ------------- | ------------ | -------- |
| Create | POST          | /`users`     | create   |
| Read   | GET           | /`users`     | list     |
| Read   | GET           | /`users`/:id | index    |
| Update | PUT           | /`users`/:id | replace  |
| Update | PATCH         | /`users`/:id | update   |
| Delete | DELETE        | /`users`/:id | delete   |

# Cibersecurity
It is the branch of the computational engineering that is dedicated to defend computers and
networks from malicious attacks.

When the hacking has a purpose of commit a crime it is called a ciber-threat:
- Ciber-crime: the attacks that are looking financial benefits.
- Ciber-attacks: search for vulnerabities on the computers, systems, apps, that allow them to take
  control over the devices. Hardening is the technique in computing, practiced to blocking or patching
  the security breaches.
- Ciber-terrorism: commit a crime looking to generate panic or terror.

## OWASP. Open Web Application Security Proyect.
OWASP has a top 10 of the 10 vulnerabilities for a web application.
* A01: Lost of access control.
  The access control implements the permisions for the users.
* A02: Cryptographic flaws
  Manage sensitive information without the correct manage of this information, using weak cryptographic keys, don't rotating the key for jwt, etc.
* A03: Injection
  Bad validation of fields allowing injection of SQL or NoSQL sentences.
* A04: Insecure design
* A05: Wrong security configuration
  If we deploy a server, and we keep the root user with the password 1234.
* A06: Vulnerable and outdated components.
  Aplication range, and system range. When a component in the system, is outdated, it vulnerabilities will affect to all the system.
* A07: Wrong identification and authentication
  - Block the account at the 3 intents.
  - 2FA.
* A08: Software and data integrity failures
  - Placement of malicious code.
  - Process of RQ.
* A09: Registration and monitoring failures.
  Without a correct registry or logs systems, it is not possible to monitore when we are being attacked.
* A10: Server-side request forgery
  It is avoidable using VPN or ACL.