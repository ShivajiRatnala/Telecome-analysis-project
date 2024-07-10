Formulas:
---------

------>    Total Revenue = Total Revenue = SUM(fact_atliqo_metrics[atliqo_revenue_crores])*10000000

------>    Total active_users = SUM(fact_atliqo_metrics[active_users_lakhs])*100000

------>    Total unsubscribe = SUM(fact_atliqo_metrics[unsubscribed_users_lakhs])*100000

------>    Avg revenue month = AVERAGEX(VALUES(dim_date[month_name]),[Total Revenue])

------>    After 5g = CALCULATE([Total Revenue],dim_date[before/after_5g] = "After 5G")

------>    After 5g = CALCULATE([Total Revenue],dim_date[before/after_5g] = "Before 5G")

------>    Total market shares = SUM(fact_market_share[tmv_city_crores])*10000000

------>    Total plans revenue = SUM(fact_plan_revenue[plan_revenue_crores])*10000000
