# 🧠 Hardware Adaptation Bridge

Trinity Engine is designed to be **Hardware-Agnostic**. It doesn't use the same logic for every PC. Instead, it "Adapts" its soul to your hardware.

## 📊 Logic Tiers

| Tier | Requirement | Behavior |
|------|-------------|----------|
| **Light** | < 8GB RAM | Focuses on extreme junk cleaning and clearing standby lists. |
| **Balanced** | 8-16GB RAM | Balances RAM purging with background service optimization. |
| **Power** | 16-32GB RAM | Aggressive CPU priority boosting and network latency reduction. |
| **Extreme** | 32GB+ RAM | Sustained high-performance mode, kernel-level UI acceleration. |

## 🛠️ How it works
The `hardware_bridge.py` uses WMI queries to detect:
1. **Core Count:** Determines the number of parallel C++ agents for XEngine.
2. **Disk Type:** Detects SSD vs HDD to decide if 'Defrag' or 'TRIM' should be used.
3. **Thermal State:** Monitors CPU load to prevent overheating during aggressive optimization.
