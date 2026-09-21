# PRIME-MANUFACTURING-ANALYSIS

## Manufacturing Production Analytics

### Introduction

Prime Manufacturing Ltd. manufactures household electrical appliances
across multiple factories and production lines. While the business has
experienced steady growth, management identified four recurring
operational challenges that could affect continued growth:

-   **Inconsistent Output:** Production volumes vary across factories
    and production lines.
-   **Rising Machine Downtime:** Unplanned stoppages reduce available
    production time.
-   **Varying Product Quality:** Defect rates and inspection scores
    differ by product and factory.
-   **Rising Operational Costs:** Maintenance and unit production costs
    are increasing.

### Project Objective

The objective of this project was to analyze a full year of
manufacturing production data and transform the data into actionable
insights that can support operational decision-making, improve
efficiency, reduce downtime, strengthen product quality, and control
costs.

------------------------------------------------------------------------
![python Overview](./python%20Overview.png)>

![Python Mth Trnd](./Python%20Mth%20Trnd.png)>

![Python chaart](./Python%20chaart.png)>

## Dataset & Methodology

The analysis covers **12 months of production activity** from **1
January 2025 to 31 December 2025** across:

  Dataset Component      Count
  -------------------- -------
  Production Records     1,000
  Factories                  3
  Production Lines           4
  Machines                  40
  Operators                100
  Product Categories         5

The dataset includes information on:

-   Planned production
-   Actual production
-   Downtime
-   Energy consumption
-   Maintenance cost
-   Unit cost
-   Environmental conditions
-   Quality inspection scores

### Data Cleaning & Preparation

The data was cleaned and validated using Python before analysis.

1.  Checked dataset structure, data types, and cardinality.
2.  Confirmed that there were no duplicate records.
3.  Filled **15 missing downtime values** using the column median.
4.  Standardized text fields such as factory, line, shift, machine type,
    and product category.
5.  Removed impossible values, including negative quantities and defects
    exceeding actual production.
6.  Validated logical ranges for humidity, quality score, and
    temperature.
7.  Applied IQR-based outlier treatment to energy, maintenance cost, and
    unit cost.

------------------------------------------------------------------------

## Company-Wide Performance

The company achieved an overall production efficiency of **93.4%**,
producing **319,201 units** against **341,586 planned units**.

The overall defect rate was **3.94%**.

The analysis identified **\$1.32M in maintenance spending** and more
than **1,000 hours of downtime** as major areas where operational
improvements could potentially support better margins.

### Headline Metrics

-   **Overall Efficiency:** 93.4%
-   **Actual Production:** 319,201 units
-   **Planned Production:** 341,586 units
-   **Defect Rate:** 3.94%
-   **Maintenance Spend:** \$1.32M
-   **Production Period:** January--December 2025

------------------------------------------------------------------------

## Factory Performance

### Factory Performance

**Factory B** recorded the highest efficiency at **93.2%** without
having a higher defect rate than the other factories.

**Factory A** recorded the lowest factory efficiency at **92.4%**,
highlighting an opportunity for a process review.

The analysis suggests that Factory B's processes and procurement
practices could be examined to identify practices that may be
transferable to other factories.

------------------------------------------------------------------------

## Production Line Performance

The production-line analysis showed a performance gap across the
network.

-   **Top-performing line:** Factory C -- Line D, with **94.2%
    efficiency**
-   **Lowest-performing line:** Factory C -- Line B, with **91.3%
    efficiency**

The approximately **3-percentage-point gap** between these lines
represents an opportunity to improve output through process optimization
without necessarily requiring additional capital investment.

------------------------------------------------------------------------

## Monthly Production Volume vs. Efficiency

Monthly analysis showed that efficiency remained broadly stable even
during higher-volume periods.

This indicates that the current production capacity was able to
accommodate demand increases without a clear deterioration in efficiency
or output quality.

This finding is relevant for future capacity and production planning.

------------------------------------------------------------------------

## Downtime Analysis

### Downtime Hotspot

The most significant downtime hotspot identified was **Factory B's
Morning shift**, with an average downtime of **63.9 minutes**.

This is notable because Factory B also recorded the strongest overall
factory performance.

A focused downtime-reduction initiative on the Morning shift could
therefore provide a targeted opportunity to improve operational
efficiency.

------------------------------------------------------------------------

## Product Quality Analysis

### Product Quality vs. Defect Rate

**Washing Machines** recorded:

-   The highest defect rate: **4.31%**
-   The lowest quality score: **79.5**
-   High production volume

The combination of relatively high production volume, elevated defects,
and a lower quality score makes Washing Machines an important area for
root-cause quality investigation.

------------------------------------------------------------------------

## Cost Efficiency by Factory

Factory B recorded the highest cost efficiency, producing approximately
**478.7 units per cost unit**.

Its procurement and production practices provide an area for further
investigation to understand which operational practices may be
contributing to its cost performance.

------------------------------------------------------------------------

## Machine Reliability

### Machine Type Performance

**Semi-Automatic machines** recorded both:

-   The highest average maintenance cost: **\$1,367**
-   The highest average downtime: **60.6 minutes**

The results indicate that maintenance spending on this machine type is
not currently translating into lower downtime.

This creates an opportunity to review maintenance strategies and
consider a more preventive approach.

------------------------------------------------------------------------

## Key Findings

### 1. Strong Operational Baseline

The company recorded **93.4% overall efficiency** and a **3.94% defect
rate**, providing a solid operational baseline.

### 2. Uneven Production-Line Performance

There is an approximately **3-percentage-point efficiency gap** between
the strongest and weakest production lines.

### 3. Downtime Concentration

Factory B's Morning shift represents the most significant downtime
hotspot despite Factory B having the strongest overall factory
performance.

### 4. Concentrated Quality Risk

Washing Machines combine the highest defect rate with the lowest quality
score while maintaining high production volume.

### 5. Maintenance Efficiency Challenge

Semi-Automatic machines have the highest average maintenance cost and
highest average downtime, suggesting that current maintenance activity
is not sufficiently improving reliability.

### 6. Energy Use vs. Production

Energy consumption shows almost no correlation with production volume,
indicating a potential opportunity to investigate avoidable energy
usage.

------------------------------------------------------------------------

## Recommendations

### 1. Standardize Factory B's Practices

Document and evaluate Factory B's process and procurement practices and
identify practices that can be adapted across Factories A and C.

### 2. Target the Weakest Production Line

Conduct a focused process review of **Factory C -- Line B**, the
lowest-efficiency production line.

### 3. Address Morning-Shift Downtime

Pilot a targeted downtime-reduction program on **Factory B's Morning
shift** before considering broader implementation.

### 4. Investigate Washing Machine Quality

Conduct a root-cause analysis into the elevated defect rate and lower
quality score associated with Washing Machines.

### 5. Strengthen Semi-Automatic Machine Maintenance

Review the current maintenance strategy for Semi-Automatic machines and
consider scheduled preventive maintenance to reduce downtime and improve
reliability.

### 6. Audit Energy Consumption

Investigate energy consumption independently of production volume to
identify potential sources of avoidable energy waste.

------------------------------------------------------------------------

## Tools & Technologies

-   **Python**
-   **Pandas**
-   **NumPy**
-   **Matplotlib / Seaborn**
-   **Data Cleaning**
-   **Exploratory Data Analysis (EDA)**
-   **Data Aggregation**
-   **Data Visualization**
-   **Operational Analytics**

------------------------------------------------------------------------

## Project Workflow

``` text
Raw Production Data
        ↓
Data Cleaning & Validation
        ↓
Exploratory Data Analysis
        ↓
Aggregation & KPI Analysis
        ↓
Factory / Line / Machine Analysis
        ↓
Downtime & Quality Analysis
        ↓
Cost & Energy Analysis
        ↓
Key Findings
        ↓
Business Recommendations
```

------------------------------------------------------------------------

## Business Impact

This analysis demonstrates how manufacturing data can be transformed
into operational insights by identifying:

-   Efficiency gaps across factories and production lines
-   Major downtime hotspots
-   Product quality risks
-   Machine reliability challenges
-   Cost-efficiency differences
-   Potential energy-use inefficiencies

The findings provide management with specific areas to investigate and
prioritize for continuous improvement.

------------------------------------------------------------------------

## Conclusion

The analysis shows that Prime Manufacturing Ltd. has a strong overall
operational baseline, but performance is not evenly distributed across
factories, production lines, shifts, products, and machine types.

The largest opportunities identified are concentrated around
**production-line efficiency, downtime reduction, product quality,
machine maintenance, cost efficiency, and energy usage**.

By applying targeted process improvements and monitoring the identified
KPIs, management can use production data more effectively to support
continuous operational improvement.

------------------------------------------------------------------------

## Project Deliverables

-   Manufacturing production analysis
-   Data cleaning and validation
-   Exploratory data analysis
-   Factory and production-line performance analysis
-   Downtime hotspot analysis
-   Product quality analysis
-   Cost-efficiency analysis 
-   Machine reliability analysis
-   Business recommendations
