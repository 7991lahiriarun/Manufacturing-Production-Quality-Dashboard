# Manufacturing-Production-Quality-Dashboard

MANUFACTURING
Production & Quality Dashboard — Analysis Report
Source: 06_manufacturing_production.csv · 3,608,207 units across 4 lines, 3 shifts
Prepared by: Arunabha Lahiri
Report type: Dashboard analysis & insights summary
Companion to: Power BI portfolio dashboard build
Executive Summary
The plant produced 3,608,207 units in the period at a defect rate of 3.47% and estimated OEE of 90.6% (availability 93.8% × quality 96.53%). Total downtime across all lines was 1,479 hours. Defect rates are broadly consistent across the four production lines (a spread of well under 1 percentage point), and supplier quality score shows essentially no correlation with defect rate (r = 0.003) in this dataset — meaning defects here are not explained by incoming material quality and are more likely driven by machine- or process-level factors.
Detailed Analysis
1. Output & OEE
Overall Equipment Effectiveness is estimated at 90.6%, calculated as Availability (93.8%) × Performance (proxy) × Quality (96.53%). Industry benchmark 'world class' OEE is typically cited around 85%, so the plant is performing at or above that reference band on the availability and quality components specifically.
Total downtime of 1,479 hours across the period is the main lever for further OEE improvement, since quality loss is already low.
2. Defect Rate by Line
Defect rate by line: Line-B: 3.55%, Line-C: 3.52%, Line-D: 3.44%, Line-A: 3.37%. Line-B runs highest at 3.55%, only marginally above Line-A at 3.37% — the gap between best and worst line is small enough that it likely reflects normal process variation rather than a systemic issue on any one line.
3. Downtime by Machine
MC-011 recorded the highest cumulative downtime in the period at 3,772 minutes, followed closely by the next several machines in the ranking — downtime is concentrated in a top group of machines rather than spread evenly across all 30, which is the classic Pareto pattern for maintenance prioritization.
Recommendation: schedule preventive maintenance for MC-011 and the next 2-3 highest-downtime machines first; this small group is disproportionately responsible for total lost production time.
4. Shift & Supplier Quality Patterns
Defect rate by shift is nearly flat: Afternoon: 3.53%, Morning: 3.53%, Night: 3.35%, with Afternoon marginally highest. This is not a meaningful operational difference.
Supplier Quality Score shows no meaningful correlation with defect rate in this data (r = 0.003), which — if this pattern held in a real plant — would suggest defects are driven by internal process/machine factors rather than incoming material quality, and quality-improvement investment should be directed at the production line rather than supplier audits.
Key Recommendations
1. Target preventive maintenance at MC-011 and the next few highest-downtime machines — downtime, not defect rate, is the larger OEE lever here.
2. Downtime reduction will move OEE more than defect-rate reduction, since quality loss is already low relative to availability loss.
3. Since defect rate doesn't correlate with supplier quality score in this data, investigate machine calibration and process parameters as the more likely defect driver.
4. Line and shift differences are small enough to deprioritize as improvement targets in favor of machine-level maintenance.
Data & Methodology Notes
This dataset is synthetically generated for portfolio purposes; the Performance component of OEE uses a simplified proxy (no true ideal-cycle-time field exists in the raw data), and the lack of correlation between supplier quality and defects reflects the synthetic generation process rather than a real causal finding. A production analysis would also track defect type/root cause codes, not just defect count.
Methodology: figures in this report are computed directly from the underlying row-level dataset (not estimated), using the same aggregation logic as the DAX measures defined for the companion Power BI dashboard, so the numbers here should reconcile with the dashboard's KPI cards and charts.
