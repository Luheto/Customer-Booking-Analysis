# Customer-Booking-Analysis
A reproducible analysis of customer flight booking behaviour — data cleaning, exploratory analysis, feature engineering, modeling, and business recommendations.
___
## Summary

This project analyses customer booking behaviour to identify the strongest drivers of completed bookings and produce actionable recommendations for sales and marketing teams.

High-level findings (see <a href=>Executive Summary.pdf<a/> for the one-page summary):

<img width="1136" height="639" alt="Screenshot 2025-10-17 234012" src="https://github.com/user-attachments/assets/17f192a7-cdc6-4498-a082-719a1ec0f093" />

- Sales leads are the primary driver of bookings. 

- Most bookings cluster around ~80 days before travel — prioritize outreach and campaigns in that lead window.
   
<img width="1189" height="590" alt="Leads by booking status" src="https://github.com/user-attachments/assets/f9844628-c657-4f7b-8bc5-4af9c824b478" />

- Low completion rate (~15% of ~7.4k customers) — significant opportunity to increase conversions.
  
<img width="989" height="590" alt="Booking" src="https://github.com/user-attachments/assets/7ddf63a0-a628-41b1-8d0a-12e4e417bcf5" />

- Top predictive features: purchase_leads, flight_hours, length_of_days, flight_duration.
  
<img width="977" height="547" alt="Important Features" src="https://github.com/user-attachments/assets/ec6d36c1-701d-4302-b1f7-fb25d26adf8b" />

___
## Goals

- Reproduce the full analysis and modeling pipeline.
- Quantify behavioural drivers of booking decisions.
- Build a predictive model for booking likelihood.
- Produce business recommendations and next steps for implementation.
___
## Notebook overview (Customer Booking.ipynb)

The notebook is organized to be reproducible and easy to follow:

- Data loading & cleaning — consistent preprocessing steps and notes on missing data handling.
- Exploratory Data Analysis — distributions, time-series patterns (including the ~80-day lead window), and correlation heatmaps.
- Feature engineering — lead-time features, behavioral aggregates, and categorical encodings.
- Modeling — baseline classifiers, evaluation (precision/recall/F1), and feature importance.
- Business conclusions — clear, actionable recommendations and suggested next steps.
___
## Key business recommendations

- Prioritize outreach around the ~80-day lead window. Concentrate paid acquisition and sales follow-up during this period to capture the highest conversion probability. 
- Target low-conversion segments with tests. With an overall completion rate around ~15%, run A/B tests for messaging, incentives, and follow-up cadences on segments with high drop-off.
- Use top predictive features in scoring. Incorporate purchase_leads, flight_hours, length_of_days, and flight_duration into a daily scoring pipeline to prioritise high-propensity customers. 
- Measure, iterate, and instrument. Deploy lightweight tracking to measure lift from targeted campaigns and feed results back into the modeling pipeline.
___
## Suggested next steps / extensions

- Productionize a scoring pipeline (daily or real-time) to surface high-propensity customers.
- Run randomized experiments (A/B tests) on offers and messaging in the ~80-day window.
- Add external signals (pricing, competitor activity) and richer behavioral features (clickstreams, session data).
- Build a stakeholder dashboard showing booking funnel KPIs and model-backed recommendations.
___
## Notes & attribution

The short executive summary is available in the repo as Executive Summary.pdf. 

___
## License

This project is released under the MIT License.
___
## Contact

**Luheto Vunda** — Data Analyst & Economist  
Lusaka, Zambia

- GitHub: https://github.com/Luheto  
- Portfolio / selected projects:
  - https://github.com/Luheto/Economic-Workforce-Analysis
  - https://github.com/Luheto/Data-Analysis-Dashboard-Call-Center
  - https://github.com/Luheto/PATUMBA-FEBRUARY-SOCIAL-MEDIA-INSIGHTS
  - https://github.com/Luheto/Optimizing-Big-Data-for-Social-Buzz-s-IPO
  - https://github.com/Luheto/Retail-Store-Expansion-Stratergy
  - https://github.com/Luheto/Data-Analysis-Dashboard-Insurance-Claims

- Email: `<luhetovda@gmail.com>`  
- LinkedIn: `<linkedin.com/in/luhetovunda>` 
- Phone: `<+260 973 026 923>`

Prefer updates or collaboration? Open an issue or a pull request on this repo — I’ll respond there.
