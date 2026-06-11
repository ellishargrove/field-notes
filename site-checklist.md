# TRACE Site Assessment Checklist
Revision 4 — updated 2019-01-15
e.hargrove

Use this before and during every initial site visit. Not a substitute for the full assessment
methodology — this is the field checklist, not the deliverable template.

---

## Pre-Visit

- [ ] Confirm site contact and access arrangements 48 hours before visit
- [ ] Review any prior assessment documents or client-provided network diagrams
- [ ] Charge all equipment (laptop, tablet, cable tester, tone generator)
- [ ] Pack: console cables (RJ45 + USB adapter), ethernet tester, label maker, measuring tape
- [ ] Confirm NDA / engagement agreement is signed before any documentation is collected
- [ ] Key question to answer at the start: *What does the client think their network looks like?*
      The gap between their mental model and reality is usually where the problems are.

---

## On-Site — Physical

- [ ] Photograph MDF and all IDFs before touching anything
- [ ] Document rack layout (top to bottom, left to right)
- [ ] Note physical security: Is the MDF locked? Who has access?
- [ ] Note environmental conditions: temperature, humidity, UPS present?
- [ ] Check cable management: labeled? traceable?
- [ ] Identify all active vs. inactive ports (tape over unused ports if none already)
- [ ] Note cable runs that exceed 90m (copper limit) — flag for testing

---

## On-Site — Network Discovery

- [ ] Identify core/distribution/access layer devices
- [ ] Confirm managed vs. unmanaged switches
- [ ] Pull running config from all managed devices (with permission)
- [ ] Document VLAN assignments — staff, student, guest, management
- [ ] Identify wireless infrastructure: controller, APs, SSID count
- [ ] Confirm internet edge: ISP CPE, firewall make/model, NAT configuration
- [ ] Identify any out-of-band management (console servers, IPMI, etc.)
- [ ] Note any shadow IT: unmanaged APs, personal hotspots, unauthorized switches

---

## On-Site — Security Posture (Observation Only)

- [ ] Is there a firewall appliance separate from the ISP CPE?
- [ ] Is student traffic segmented from staff traffic?
- [ ] Is there a guest network? Is it isolated?
- [ ] Are default passwords in use on any visible devices? (check login prompts if accessible)
- [ ] Is there any network monitoring in place? (SNMP, syslog, SIEM)
- [ ] Are wireless networks using WPA2-Enterprise or PSK?
      Key observation: PSK networks where the key hasn't changed in 2+ years are effectively open.

---

## Post-Visit — Documentation

- [ ] Upload all photos to client folder (labeled by location)
- [ ] Draft physical inventory within 48 hours while memory is fresh
- [ ] Flag any critical findings for immediate client notification (don't wait for the report)
- [ ] Log visit in field-notes repo
- [ ] Update site-specific assessment document with revision number

---

## Notes on Scope

This checklist covers initial assessment visits. Penetration testing, wireless surveys,
and firewall rule reviews each have their own checklists — don't use this one for those.

If something doesn't fit a checkbox, write it down anyway. The most important findings
are usually the ones that don't fit any template.

---

*TRACE internal document — not for client distribution*
