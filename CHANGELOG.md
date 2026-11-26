# ArthERP Pro — Changelog & Release Notes

All notable changes, features, and fixes for ArthERP Pro are documented here.

---

## [v2.4.2] — 2026-11-26

### 🦚 UI & Visual Refresh
- **Restored Peacock Feather Theme:** Re-introduced the signature Peacock Teal palette (`#0F766E`, `#0D9488`, `#14B8A6`) for both Dark and Light modes. Completely eliminates eye fatigue during continuous billing shifts.
- **Creative Note Boxes:** Introduced `CreativeNoteBox` callouts with accent left borders and subtle glow across Firm Settings, Document Scheme guides, and GST return dashboards.

### ⚙️ Firm Settings & Validation
- **10-Digit Mobile Number Validation:** Enforced strict 10-digit limit with permanent `+91` prefix badge. Automatically strips leading formatting upon database retrieval.
- **Logo & Signature Upload Limits:** Added strict file size validation (Max 1.0 MB for Firm Logo, Max 500 KB for Authorised Signature) with helpful dimension guidelines (300×120px / 300×150px) to prevent slow invoice rendering and bulky database backups.

### 💳 ArthPay Integration (Laravel 12 UPI Gateway)
- **Midnight Collection Rollover:** Automatic daily reset for multi-account UPI rotation without cron dependency.
- **Zero-Friction Access:** Persistent 1-year device authentication cookie eliminating daily login/PIN friction for counter operators.
- **Redesigned Checkout & Dashboard:** Modern high-conversion UPI checkout with dynamic QR, 1-click UPI ID copy, mobile app deep-links (GPay, PhonePe, Paytm, BHIM), and real-time order filtering.

### 🧪 Test Verification
- All 46 automated unit tests passing 100% (0 errors, 0 failures).

---

## [v2.4.0] — 2026-11-19
- Introduced A5 Portrait Smart Adaptive template (1 page for <=12 items, 2 pages for 13–26 items).
- Added Dual Printing Modes (Full Color & Laser-Safe Pure B&W).
- Implemented FIFO COGS calculation, indirect expenses tracking, and annual FY Closing wizard.
- Integrated draft cart crash recovery and AES-256 encrypted auto-backups.
