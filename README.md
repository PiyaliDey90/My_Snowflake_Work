# My_Snowflake_Work


Hands-on Snowflake projects and learning.

## 📦 Retail Orders Analytics Pipeline
An end-to-end **medallion ELT pipeline** built on Snowflake, using TPCH
sample data as a simulated source system.

**Flow:** files → stage → **RAW** (bronze) → **STAGING** (silver) → **ANALYTICS** (gold),
orchestrated with Streams + Tasks.

### Layers
| Layer | Schema | Purpose |
|-------|--------|---------|
| Bronze | `RAW` | Raw data loaded as-is via `COPY INTO` |
| Silver | `STAGING` | Cleaned, conformed, business-friendly columns |
| Gold | `ANALYTICS` | Aggregated marts for reporting |

## 📁 Structure
