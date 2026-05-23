<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0d1117,100:00b4d8&height=180&section=header&text=Dental%20Clinic%20Management%20System&fontSize=32&fontColor=ffffff&fontAlignY=38&desc=Secure%20Full-Stack%20Web%20Application&descAlignY=58&descColor=90e0ef" width="100%"/>

[![Live Demo](https://img.shields.io/badge/Live%20Demo-Online-28a745?style=for-the-badge&logo=googlechrome&logoColor=white)](https://dentalclinicpro.rf.gd/dental_clinic/index.php)
[![PHP](https://img.shields.io/badge/PHP-777BB4?style=for-the-badge&logo=php&logoColor=white)]()
[![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)]()
[![OWASP](https://img.shields.io/badge/OWASP-Hardened-red?style=for-the-badge)]()
[![Status](https://img.shields.io/badge/Status-Active-brightgreen?style=for-the-badge)]()

</div>

---

## Overview

A web-based dental clinic management system built with **security-first architecture** — threat modeling and secure design were part of the process from day one, not an afterthought.

> Used both as a **production clinic tool** and a **personal AppSec research sandbox** — intentionally building and auditing authentication and access control layers.

---

## Features

| Module | Description |
|--------|-------------|
| Patient Management | Add, edit, delete, search patient records |
| Visit Tracking | Log dental visits with detailed notes |
| Billing & Payments | Daily and monthly reports with export |
| File Uploads | Secure upload and download per patient |
| Authentication | Login system with restricted access control |
| Reports | Export patient and payment data to CSV |

---

## Security Architecture

### Authentication & Access Control
- Session-based authentication with restricted route access
- RBAC to prevent privilege escalation
- No sensitive data stored client-side

### Injection Prevention
- Parameterized queries (PDO) — eliminates SQLi vectors
- Input sanitization on all user-supplied data
- File type validation and upload path isolation

### OWASP Top 10 Coverage### Manual Security Testing
- SQLi — tested via Burp Suite on all input fields
- Auth bypass — direct URL access without session
- IDOR — patient ID manipulation in URLs
- File upload abuse — non-image extensions and double-extension payloads

---

## Project Structure
---

## Getting Started

```bash
# 1. Clone the repo
git clone https://github.com/AhmedAshrafShaban/Code-Dental-clinic.git

# 2. Import database
# Create MySQL database and import .sql from /includes

# 3. Configure connection in includes/db.php
# $host = 'localhost';
# $db   = 'dental_clinic';
# $user = 'root';
# $pass = 'your_password';

# 4. Set permissions
chmod 755 uploads/

# 5. Run
# http://localhost/Code-Dental-clinic/index.php
```

---

## Tech Stack

![PHP](https://img.shields.io/badge/PHP-777BB4?style=flat-square&logo=php&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white)
![Bootstrap](https://img.shields.io/badge/Bootstrap-7952B3?style=flat-square&logo=bootstrap&logoColor=white)
![Burp Suite](https://img.shields.io/badge/Burp%20Suite-FF6633?style=flat-square&logo=burpsuite&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)

---

## Author

**Ahmed Ashraf Shaban** — Junior Penetration Tester | AppSec Enthusiast

[![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/AhmedAshrafShaban)
[![Email](https://img.shields.io/badge/Email-D14836?style=flat-square&logo=gmail&logoColor=white)](mailto:ahmedelkodary292@gmail.com)

---

<div align="center">
<img src="https://capsule-render.vercel.app/api?type=waving&color=0:00b4d8,100:0d1117&height=100&section=footer" width="100%"/>

*"Built secure. Tested harder."*
</div>