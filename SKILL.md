---
name: wallet-monitor
description: Monitor NEAR wallet balances, set price alerts, and send automated notifications
version: 1.0
---

# Wallet Monitor Skill

## Purpose
Monitor NEAR wallet balances, track price changes, and send automated alerts when thresholds are met.

## Commands

### check-balance
Check current wallet balances for all tokens.

Example:
check-balance

Output:
Wallet Balance Report
NEAR: 4.171 ($8.59)
USDC: 1.983 ($1.98)
Total: $10.57

### set-alert <token> <condition> <price>
Set a price alert for a token.

Examples:
set-alert NEAR above 4.00
set-alert USDC below 0.99

### list-alerts
List all active price alerts.

### remove-alert <alert_id>
Remove an active alert.

## API Integration
Uses NEAR DCA Agent API for balance checks and token data.
