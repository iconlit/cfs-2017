# Single-Mode Freight Dependence & Risk Exposure

### An analysis of the 2017 Commodity Flow Survey (CFS) Public Use File

## The Question

Freight in the United States moves through a combination of transportation modes — truck, rail, water, pipeline, air, and other modes. But the degree of dependence on those modes varies considerably between regions.

Some regions have a large share of their outbound freight concentrated in a single transportation mode. This raises an important supply-chain risk question:

> **If a region's dominant transportation mode were disrupted, how much of its outbound freight would be exposed to that disruption, and how significant would that exposure be nationally?**

To examine this, this project looks at freight dependence through two different lenses: **economic value** and **physical shipment weight**.

---

## Why Two Metrics?

A single dependence metric can hide important differences between the types of freight being transported.

### Economic Value Dependence

**Economic Value Dependence** measures the percentage of a region's outbound shipment value associated with a particular transportation mode.

It answers:

> **How much economic value is exposed if this mode is disrupted?**

$$
Economic\ Value\ Dependence =
\frac{Weighted\ Value\ by\ Mode}
{Total\ Weighted\ Outbound\ Value}
\times 100
$$

### Operational Dependence

**Operational Dependence** measures the percentage of a region's outbound shipment weight associated with a particular transportation mode.

It answers:

> **How much physical freight movement is exposed if this mode is disrupted?**

$$
Operational\ Dependence =
\frac{Weighted\ Weight\ by\ Mode}
{Total\ Weighted\ Outbound\ Weight}
\times 100
$$

These two measures do not necessarily tell the same story.

A region shipping relatively lightweight, high-value goods may have greater **economic-value dependence** than **operational dependence**.

Conversely, a region shipping heavy, relatively low-value commodities such as bulk agricultural or energy products may have much greater **operational dependence** than **economic-value dependence**.

The difference between the two metrics is therefore an important part of the analysis.

---

## Methodology

The analysis uses the **2017 Commodity Flow Survey (CFS) Public Use File**.

Because the CFS Public Use File is a sample, raw shipment records are expanded using the Census-provided `WGT_FACTOR`.

### Weighted Shipment Value

$$
Weighted\ Shipment\ Value =
SHIPMT\_VALUE \times WGT\_FACTOR
$$

### Weighted Shipment Weight

$$
Weighted\ Shipment\ Weight =
SHIPMT\_WGHT \times WGT\_FACTOR
$$

These weighted values are then aggregated by:

- Origin state
- Origin CFS area
- Transportation mode

The resulting figures represent **estimated population-level freight totals**, rather than simple sums of the sampled records.

### Mode Exposure

For a particular region and transportation mode:

$$
Value\ Exposure =
\sum(SHIPMT\_VALUE \times WGT\_FACTOR)
$$

$$
Weight\ Exposure =
\sum(SHIPMT\_WGHT \times WGT\_FACTOR)
$$

The corresponding percentages are calculated against the region's total weighted outbound freight.

---

# Headline Finding: Wyoming

### Remainder of Wyoming CFS Area — Rail

| Metric                                   |                Result |
| ---------------------------------------- | --------------------: |
| Economic value dependence                |            **24.32%** |
| Operational dependence                   |            **87.12%** |
| Value exposed                            |    **$1.254 billion** |
| Weight exposed                           | **459.35 billion lb** |
| Share of national freight value exposed  |           **0.0086%** |
| Share of national freight weight exposed |           **1.8420%** |

Wyoming provides one of the clearest examples of why both value and weight need to be considered.

**87.12% of the region's outbound freight weight is associated with rail**, while rail accounts for only **24.32% of its outbound shipment value**.

The difference becomes even more significant when viewed nationally.

The rail-dependent freight from this CFS area represents approximately:

- **1.842% of the nation's outbound freight weight**
- **0.0086% of the nation's outbound shipment value**

That means this region has a relatively small national footprint when measured by shipment value, but a substantially larger footprint when measured by physical freight weight.

A risk assessment based only on shipment value would therefore give a very different picture from one based on physical freight movement.

---

# Other High-Dependence Regions

The same analysis reveals a number of regions where trucking accounts for a large share of outbound freight.

| Region                     | Mode                | Economic Value Dependence | Operational Dependence | Value Exposed | Weight Exposed |
| -------------------------- | ------------------- | ------------------------: | ---------------------: | ------------: | -------------: |
| District of Columbia       | Company-owned truck |                    51.10% |                 81.36% |       $599.5M |       3.62B lb |
| Hawaii                     | Company-owned truck |                    77.31% |                 79.96% |        $3.81B |      14.41B lb |
| New Hampshire              | Company-owned truck |                    35.68% |                 75.45% |        $5.39B |      32.72B lb |
| Kentucky / Cincinnati      | For-hire truck      |                    71.41% |                 74.93% |       $15.47B |      21.07B lb |
| Massachusetts / Boston     | Company-owned truck |                    28.40% |                 71.16% |       $18.85B |     106.11B lb |
| North Carolina / Raleigh   | For-hire truck      |                    42.53% |                 70.95% |       $14.58B |      50.00B lb |
| California / San Diego     | For-hire truck      |                    39.40% |                 70.93% |       $15.68B |      36.33B lb |
| Connecticut / Hartford     | Company-owned truck |                    36.69% |                 70.36% |       $12.97B |      33.14B lb |
| Tennessee / Nashville      | For-hire truck      |                    58.38% |                 70.02% |       $37.62B |      72.25B lb |
| Ohio / Cleveland           | For-hire truck      |                    62.69% |                 67.63% |       $53.67B |      82.51B lb |
| Virginia / Washington area | For-hire truck      |                    28.20% |                 67.38% |        $4.48B |      35.89B lb |
| Texas / Laredo             | Company-owned truck |                    60.76% |                 66.61% |        $4.13B |      15.26B lb |
| Maryland                   | For-hire truck      |                    59.03% |                 66.18% |        $8.89B |      33.47B lb |
| Tennessee / Memphis        | For-hire truck      |                    48.98% |                 65.29% |       $23.61B |      29.58B lb |

---

# What the Results Show

## 1. Physical and economic dependence can differ substantially

New Hampshire is a particularly clear example.

Its Boston-Worcester-Providence CFS area has:

- **35.68% economic-value dependence**
- **75.45% operational dependence**

The transportation mode therefore accounts for more than twice as much of the region's outbound freight weight as it does shipment value.

This demonstrates why looking only at dollars can understate the amount of physical freight exposed to a transportation disruption.

---

## 2. Trucking dominates many high-dependence regions

Most of the high-dependence regions identified in the results are concentrated around **truck transportation**, including company-owned and for-hire trucking.

Examples include:

- Hawaii
- New Hampshire
- Cincinnati
- Massachusetts
- Raleigh
- San Diego
- Hartford
- Nashville
- Cleveland
- Laredo
- Maryland
- Memphis

The exact nature of the dependence varies substantially between regions, however. Some have relatively high economic-value dependence, while others have a much larger difference between value and weight dependence.

---

## 3. Oklahoma shows a different pattern

Oklahoma's remainder CFS area illustrates the opposite relationship:

| Metric                    | For-hire truck |
| ------------------------- | -------------: |
| Economic value dependence |     **73.31%** |
| Operational dependence    |     **56.35%** |

Truck transportation accounts for a large share of the region's shipment value, but a smaller share of its physical freight weight.

Rail accounts for only **2.69% of shipment value** but **16.92% of shipment weight** in the region.

This demonstrates how a relatively small share of freight value can still represent a substantial amount of physical freight movement.

---

# National Exposure

Regional dependence alone does not tell us how significant that dependence is at the national level.

For this reason, the analysis also calculates each region-mode combination's share of total national outbound freight.

### Example: Wyoming

The Wyoming rail-dependent freight represents:

**1.8420% of national outbound freight weight**

but only:

**0.0086% of national outbound shipment value.**

This creates a major difference between the region's **physical significance** and its **economic-value significance**.

The same approach can be applied to every region:

$$
National\ Weight\ Exposure =
\frac{Regional\ Mode\ Weight}
{National\ Outbound\ Weight}
\times100
$$

$$
National\ Value\ Exposure =
\frac{Regional\ Mode\ Value}
{National\ Outbound\ Value}
\times100
$$

This makes the question of _"how much of the country would feel it?"_ more concrete.

---

# Interpreting "Risk"

The `value_at_risk` and `weight_at_risk` measures should be interpreted as **freight exposure to a hypothetical complete disruption of the transportation mode**, rather than guaranteed economic losses or freight that would permanently stop moving.

For example, if 80% of a region's outbound weight moves by truck, this does **not** necessarily mean 80% of that freight would become impossible to transport.

Some freight could potentially:

- Shift to another transportation mode
- Be rerouted
- Use alternative infrastructure
- Be transported through another region
- Experience delays rather than complete interruption

Therefore, the analysis measures **mode concentration and potential exposure**, not the actual loss caused by a disruption.

---

# Key Takeaway

A single metric is not enough to describe freight dependence.

**Economic value tells us how much shipment value is exposed.**

**Shipment weight tells us how much physical freight movement is exposed.**

These can produce very different results for the same region and transportation mode.

Wyoming demonstrates the importance of this distinction particularly well: its rail dependence represents a relatively small share of national shipment value but a much larger share of national freight weight.

The broader finding is that **freight transportation risk depends not only on how much freight a region moves, but also on what kind of freight it moves and how concentrated its transportation modes are.**

---

# Data Source

**U.S. Census Bureau — 2017 Commodity Flow Survey (CFS) Public Use File**

- **Records:** 5,978,523 shipment records
- **Geographic unit:** CFS areas
- **Analysis:** Outbound freight by origin CFS area and transportation mode
- **Weighting:** `WGT_FACTOR`
- **Freight value:** `SHIPMT_VALUE`
- **Freight weight:** `SHIPMT_WGHT`

All value and weight figures in this analysis are **`WGT_FACTOR`-weighted population estimates**, rather than raw sample sums.

---

---

# Limitations

This analysis measures freight concentration using the transportation mode recorded in the CFS. It does not model the actual consequences of a disruption.

In particular, it does not estimate:

- How quickly freight could switch modes
- Available spare capacity on alternative modes
- Infrastructure redundancy
- Rerouting costs
- Delay duration
- Actual economic losses
- Whether a shipment could be substituted by another transportation route

Therefore, the results should be interpreted as a **freight-dependence and exposure analysis**, rather than a complete disruption simulation.

---

## Conclusion

The analysis shows that transportation dependence can look very different depending on whether it is measured in **dollars or physical freight weight**.

A region can have relatively low economic-value dependence but extremely high operational dependence, as demonstrated by Wyoming. Other regions show strong trucking dependence from both perspectives, while some exhibit much larger exposure in shipment value than in physical weight.

Looking at both measures together provides a more complete picture of where U.S. outbound freight is concentrated and which transportation-mode disruptions could expose substantial amounts of freight movement or shipment value.
