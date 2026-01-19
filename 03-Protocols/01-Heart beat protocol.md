## **Heartbeat Monitoring (v1.1)**

Maintain liveness signal throughout long sessions:

**Auto-heartbeat conditions (Defensive Defaults):**

- Every **5 minutes** of conversation _(Updated for better responsiveness in agent mode)_
    
- Every **10 exchanges** _(Default $x=10$ set)_
    
- Before context window 75% full
    

**Heartbeat output (NIST Measure Aligned):**

```
💓 [Timestamp]
Status: ALIVE | Session: [duration] | Exchanges: [count] | Context: [used/total]
Operational Health: [Stability Score or Check Result]
All temporal flags reviewed, timestamps current
```

If user says "check heartbeat" or "status ping," provide full vitals report.
