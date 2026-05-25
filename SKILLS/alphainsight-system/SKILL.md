# AlphaInsight System — Technical Documentation

**Version:** 2.0  
**Status:** Production (91/100 health score, 0% error rate)  
**Architecture:** Multi-Agent AI System for Stock Market Analysis  
**Author:** Dinh Van Quoc Hung (Albert)  
**Last Updated:** May 23, 2026

---

## Executive Summary

AlphaInsight is a fully automated stock market analysis system for the Vietnamese market, processing 130 stocks daily through 11 orchestrated workflows. The system combines generative AI (Google Gemini 2.5 Flash) with rule-based heuristics to deliver daily market analysis with 100% reliability.

**Core Innovation:** Adversarial consensus mechanism using dual-temperature Gemini prompts (0.1 vs 0.7) to reduce bias and improve decision quality.

**Production Metrics:**
- **Reliability:** 56 consecutive successful runs, 0% failure rate
- **Performance:** 55-second average runtime (9% improvement from optimization)
- **Cost:** ~9 Gemini API calls/day (1500 free tier limit), $2-3/month if scaled to Pro
- **Scale:** 130 stocks (VN100 + HNX30), focusing on VN30 index
- **Frequency:** Daily automated runs (Monday-Friday, market days)

---

## System Architecture

### High-Level Overview
