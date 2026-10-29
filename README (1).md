# HR Attrition Analysis: Power BI

A three-page Power BI report exploring employee attrition in a fictional IBM HR dataset (1,470 employees). Built in Power BI Desktop as a local .pbix file; no Power BI Service tenant was used.

## Key findings
- Company attrition: **16.12%** (237 leavers out of 1,470 employees)
- Attrition by department: Sales **20.63%**, HR **19.05%**, R&D **13.84%**
- Average tenure: **7.0 years** overall
- Stayers vs. leavers: $6.8K vs. $4.8K average monthly income (~30% pay gap); 7.4 vs. 5.1 years average tenure

## Report pages
1. **Overview**: headline KPIs against the 16.12% company benchmark
2. **Deep-Dive**: attrition drivers, including the stayers-vs-leavers comparison
3. **Demographics**: attrition patterns across employee groups

Full-page images are in the `screenshots/` folder, and the full report export is `IBM_HR_Attrition.pdf` in this repository.

## How to read the colors
Dark blue = above the 16.12% company average. Light blue = at or below the company average.

## Techniques used
- Slicer-proof benchmark measure built with `ALL`, so the 16.12% company average stays fixed while visuals filter
- Key Insights panel to surface the headline takeaways on each page

## Case study conclusion

This report analyzed attrition for 1,470 employees in a fictional IBM HR dataset. The overall attrition rate was 16.12 percent, with 237 employees leaving. Three findings stand out.

First, attrition is concentrated in specific roles rather than spread evenly across departments. Sales had the highest department rate at 20.63 percent, but the pattern inside Sales is role-specific. Sales Representatives left at 39.76 percent and earned the lowest average monthly income in the company at $2,626, while Sales Executives left at 17.48 percent. The same pattern appears in Research and Development, the lowest-attrition department at 13.84 percent, where Laboratory Technicians still left at 23.94 percent. Managers and Research Directors had the lowest rates, at 4.90 percent and 2.50 percent.

Second, employees who left earned less and had shorter tenure than employees who stayed. Leavers averaged $4.8K in monthly income and 5.1 years of tenure, compared with $6.8K and 7.4 years for stayers. That is a pay gap of about 30 percent, and leavers left about two years earlier on average.

Third, attrition was highest early in working life. Employees aged 18 to 24 left at 39.18 percent, more than twice the company rate, and attrition dropped sharply after age 35. Single employees left at 25.53 percent, about twice the rate of married employees at 12.48 percent and divorced employees at 10.09 percent.

Two explanations are consistent with these patterns. The first is that pay at the entry level may not be keeping pace with the demands of those roles. The roles with the highest attrition, Sales Representatives and Laboratory Technicians, are also among the lowest paid, while the highest-paid senior roles barely lose anyone. The second is that the first years of employment are the most fragile period. Younger employees and employees with shorter tenure have had less time to build seniority, internal networks, and a clear promotion path, so leaving carries a lower cost for them than it does for established employees.

Two follow-up actions would test these explanations. First, review the starting pay bands and the first two years of pay progression for Sales Representatives and Laboratory Technicians against market rates, and track whether any adjustment changes those roles' attrition in the following period. Second, add structured support for employees in their first two years, including scheduled check-ins and a written promotion timeline, then re-measure attrition by age band and tenure band each quarter to see whether the early-career rates move.

These findings describe patterns in one fictional dataset. They show where attrition concentrates, but they do not by themselves prove why any individual employee left.

## Data source
IBM HR Analytics Employee Attrition dataset via Kaggle (fictional data).
