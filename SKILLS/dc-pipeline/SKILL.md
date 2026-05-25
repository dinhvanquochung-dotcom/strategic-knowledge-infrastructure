# DC-PIPE Series — Data Pipeline Documentation

**System:** Second Brain Universe  
**Purpose:** Automated data flows between layers and external systems  
**Author:** Dinh Van Quoc Hung (Albert)  
**Last Updated:** May 14, 2026

---

## Overview

DC-PIPE (Data Center Pipeline) series represents the **nervous system** of Second Brain Universe — automated workflows that move data between:
- Input channels (Telegram, voice, web)
- Notion databases (TASKS, PROJECT HUB, KNOWLEDGE BASE)
- External systems (TTCK Universe)
- Output layers (Family Portal, Public Garden)

**Core Principle:** Every pipeline has **error handler first** (Principle P4). No silent failures.

---

## Pipeline Registry

| ID | Name | Status | Trigger | Purpose |
|----|------|--------|---------|---------|
| **DC-PIPE-001** | Capture & Classify | ✅ Live | Telegram commands | Route input to correct DB via Gemini |
| **DC-PIPE-002** | Knowledge Health | 🔵 Planned | Weekly Sunday | Score Confidence/Decay across KB |
| **DC-PIPE-005** | Smart Router | ✅ Live | Webhook | Route processed ideas to KB/Projects |
| **DC-PIPE-008** | Weekly Review | 🟡 Design | Sunday 8pm | Digest + cleanup Inbox >7 days |
| **DC-PIPE-009** | TTCK Bridge | 🔴 Disabled | (was daily) | Real-time trading data → SB (REMOVED) |
| **DC-PIPE-010** | Wisdom Feed | 🟡 Design | Saturday | TTCK lessons → KB Seedling (1-way) |
| **DC-PIPE-011** | Legacy Formatter | 🔵 Planned | Manual | Cornerstone → Family Portal format |
| **DC-PIPE-012** | Public Filter | 🔵 Planned | Manual | CHÂN-THIỆN-MỸ filter → Public Garden |
| **DC-PIPE-013** | PAIOS Extractor | 🟡 Next | Sunday 9pm | Mine lessons from completed work |

---

## DC-PIPE-001: Capture & Classify

**Status:** ✅ Production  
**Trigger:** Telegram `/capture`, `/task`, `/project`, `/ask`  
**Runtime:** ~3 seconds  
**AI:** Gemini 2.5 Flash (classification)

### Architecture
