# AlphaInsight Workflows — Detailed Architecture

This document provides in-depth specifications for each of the 11 workflows in the AlphaInsight system.

---

## WF1: Data Collection — VN100 + HNX30

**Type:** Scheduled  
**Trigger:** Cron (11:31 AM, 3:00 PM Monday-Friday)  
**Runtime:** ~5 seconds  
**Dependencies:** SSH access to VPS, Python scripts (fetch_vn100.py, fetch_hnx30.py)

### Flow Diagram