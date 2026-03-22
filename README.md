# 🛠️ HP EliteBook 845 G7 — Keyboard Replacement & RAM Upgrade

**Category:** IT Hardware Repair & Upgrade  
**Device:** HP EliteBook 845 G7  
**Date:** March 2026  
**Outcome:** ✅ Fully functional — keyboard replaced, RAM upgraded to 16 GB dual-channel, Windows 11 verified

📄 **[View Full Visual Lab Report](https://arturskaufmanis.github.io/Hardware-repair-and-upgrade-project/)**

---

## Overview

This lab documents the complete lifecycle of an IT hardware repair and upgrade project — from fault diagnosis and research through to component sourcing, disassembly, repair, upgrade, reassembly, and post-repair verification.

The device was purchased with a known keyboard fault. Rather than simply replacing the part, the project began with structured research: identifying the root cause of the fault, determining the correct replacement part, assessing the upgrade potential of the platform, and studying the disassembly procedure before touching the hardware. This approach reflects how hardware work should be done in a professional IT environment — methodically, with decisions grounded in research rather than assumption.

---

## Device Specifications

| Component | Specification |
|-----------|--------------|
| **Model** | HP EliteBook 845 G7 |
| **CPU** | AMD Ryzen 5 PRO 4650U with Radeon Graphics @ 2.10 GHz |
| **RAM (original)** | 8 GB DDR4 3200 MHz SODIMM — single channel, one slot occupied |
| **RAM (upgraded)** | 16 GB DDR4 3200 MHz SODIMM — dual channel, 2 × 8 GB matched pair |
| **Storage** | 238 GB NVMe SSD |
| **GPU** | AMD Radeon™ Integrated Graphics (496 MB) |
| **OS** | Windows 11 |

---

## Fault Diagnosis

On receipt of the device, a full inspection was carried out before any disassembly. The goal was to understand the actual failure mode rather than assume.

**Symptoms:** Three keys — R, T, and Y — were non-functional.

**Finding:** Physical inspection revealed the previous owner had attempted a DIY repair. The aluminium stabiliser hinges on all three keycaps were broken and could not be reseated or repaired. The damage pattern was consistent with improper keycap removal technique — lifting at an angle rather than straight up, shearing the hinge clips.

**Decision:** Individual key hinge repair was ruled out as non-viable. A full keyboard replacement was the correct resolution. All other components — display, ports, trackpad, storage, and system board — were verified as functional prior to proceeding.

---

## Research Phase

Before ordering parts or starting disassembly, the following research was completed:

**Keyboard replacement:**
- Identified the correct HP spare part number for the EliteBook 845 G7 keyboard (UK layout)
- Confirmed the keyboard is riveted to the palmrest — not screwed — requiring a heat-based separation method
- Reviewed the HP service manual disassembly sequence to understand the correct order of operations and identify any fragile connectors or cables requiring care

**RAM upgrade:**
- Confirmed the 845 G7 has two SODIMM slots, with one occupied by a single 8 GB DDR4 3200 MHz module
- Verified the platform supports dual-channel operation when both slots are populated with matched modules
- Identified maximum supported capacity (32 GB) and confirmed DDR4 3200 MHz SO-DIMM as the correct specification
- Sourced a matched 8 GB DDR4 3200 MHz module to enable dual-channel operation, improving memory bandwidth — particularly relevant for the AMD integrated GPU which shares system memory

This research phase ensured the correct parts were ordered before disassembly, and that no steps were improvised during the repair.

---

## Tools & Materials

| Item | Purpose |
|------|---------|
| Electric screwdriver | Chassis screw removal and reinstallation |
| Plastic case opening picks | Panel separation without marking or cracking the chassis |
| Plastic tweezers | Safe handling of ribbon cables and ZIF connectors |
| Watchmaker magnification glasses | Inspection of hinges, connectors, and rivet points |
| Heat gun (DeWalt) | Softening keyboard rivet adhesive for non-destructive removal |
| Glue gun | Re-securing replacement keyboard at rivet contact points |
| Compressed air duster | Dust removal from internals during disassembly |
| Coffee | Essential consumable ☕ |

---

## Procedure

### Phase 1 — Pre-Disassembly Preparation

- Device disconnected from mains and visually inspected
- Service manual reviewed; disassembly sequence confirmed
- All tools and replacement parts prepared in advance
- ESD precautions observed throughout

### Phase 2 — Disassembly

- Bottom panel removed using plastic picks and screwdriver
- Battery connector disconnected immediately upon opening — standard practice to eliminate short-circuit risk before handling internal components
- All components identified, inspected, and placed in disassembly order for controlled reassembly:
  - Motherboard, CPU fan and heatsink, WLAN card, RAM (single slot occupied confirmed), M.2 SSD, display assembly with hinges and antenna cables, speakers, battery

### Phase 3 — Keyboard Replacement

- Palmrest assembly removed from chassis
- Heat gun applied to the reverse side of the palmrest to soften the factory rivet adhesive — controlled application to avoid heat damage to the PCB or ribbon cables
- Damaged keyboard separated cleanly from the palmrest
- Replacement keyboard fitted and aligned
- **Glue gun used at original rivet contact points** — a deliberate technique choice. The glue creates a secure bond while remaining reversible: future keyboard replacement can be done by reheating the glue, without needing to replace or damage the palmrest. This makes the repair more maintainable than standard rivet reinstatement
- Keyboard ribbon cable and backlight connector reseated and verified

### Phase 4 — RAM Upgrade

- Second SODIMM slot located on the motherboard
- New 8 GB DDR4 3200 MHz module installed in the empty slot
- Both modules seated and latched; dual-channel configuration confirmed

### Phase 5 — Reassembly

- All components reinstalled in reverse disassembly sequence
- All ribbon cables, antenna cables, and board connectors reseated
- Battery reconnected; bottom panel refitted and all screws secured

---

## Post-Repair Verification

All functionality tested systematically after reassembly:

| Test | Result |
|------|--------|
| Device powers on cleanly | ✅ Pass |
| All keys functional — including R, T, Y | ✅ Pass |
| RAM detected: 16.0 GB @ 3200 MT/s | ✅ Pass |
| Dual-channel operation confirmed in System Info | ✅ Pass |
| Windows 11 OOBE completed successfully | ✅ Pass |
| Wi-Fi adapter detected; networks visible | ✅ Pass |
| Display — no artefacts or dead pixels | ✅ Pass |
| Trackpad and fingerprint reader functional | ✅ Pass |
| All USB and I/O ports functional | ✅ Pass |
| Fan spin-up and thermal management normal | ✅ Pass |

**System > About confirmed post-repair:** AMD Ryzen 5 PRO 4650U | 16.0 GB RAM @ 3200 MT/s | 238 GB SSD

---

---

## Skills Demonstrated

- Hardware fault diagnosis — identifying root cause rather than symptom
- Pre-repair research: part identification, compatibility verification, upgrade assessment
- Service manual interpretation and disassembly planning
- Full laptop disassembly and reassembly
- Keyboard replacement using heat gun separation and glue reinstatement
- RAM upgrade and dual-channel configuration
- ESD awareness and safe component handling
- Systematic post-repair functional verification
- Technical documentation

---

## Repository Structure

```
hp-elitebook-845g7-repair-lab/
├── README.md
└── images/
    ├── IMG20260312120343.jpg
    ├── IMG20260312121105.jpg
    ├── ... (all 20 lab images)
    └── IMG20260312190822.jpg
```

---

*Part of a general IT portfolio demonstrating hardware support, diagnosis, and upgrade competency.*
