Sample Q&A Transcript - PySpark Data Insights Agent
Week 3 Take-Home Project - Google ADK Learning Series
> Generated end-to-end by the agent. Values below come from the reproducible synthetic fallback dataset (60,000 rows, seed=7). When you point `DATA_URL` at a real external CSV, numbers change but the flow is identical - every number is computed by PySpark, never invented by the model.
---
Q1. What are the total sales by region?
Tool params: `{'metric': 'sum', 'measure': 'sales', 'group_by': 'region', 'filters': {}, 'sort': 'desc', 'limit': None}`
Agent answer:
Sum Of Sales by region:
East: 4,612,330.63
West: 4,576,373.21
South: 4,565,506.11
Central: 4,562,980.25
Highest is East at 4,612,330.63.
Chart: bar chart
---
Q2. Show me the top 5 sub-categories by total sales
Memory recall - you previously asked:
What are the total sales by region?
Tool params: `{'metric': 'sum', 'measure': 'sales', 'group_by': 'sub_category', 'filters': {}, 'sort': 'desc', 'limit': 5}`
Agent answer:
Sum Of Sales by sub_category:
Phones: 2,550,722.51
Copiers: 2,542,257.69
Accessories: 2,525,874.47
Machines: 2,480,678.38
Furnishings: 1,778,073.86
Highest is Phones at 2,550,722.51.
Chart: bar chart
---
Q3. What is the average profit by category?
Memory recall - you previously asked:
What are the total sales by region?
Show me the top 5 sub-categories by total sales
Tool params: `{'metric': 'avg', 'measure': 'profit', 'group_by': 'category', 'filters': {}, 'sort': 'desc', 'limit': None}`
Agent answer:
Avg Of Profit by category:
Technology: 19.68
Furniture: 13.82
Office Supplies: 2.31
Highest is Technology at 19.68.
Chart: bar chart
---
Q4. Show the monthly sales trend
Memory recall - you previously asked:
What are the total sales by region?
Show me the top 5 sub-categories by total sales
What is the average profit by category?
Tool params: `{'metric': 'sum', 'measure': 'sales', 'group_by': 'month', 'filters': {}, 'sort': 'desc', 'limit': None}`
Agent answer:
Sum Of Sales by month:
2023-07: 816,530.38
2023-12: 804,482.67
2023-10: 796,342.58
2024-10: 795,511.97
2024-12: 789,011.16
2023-05: 784,719.15
2024-03: 781,326.11
2024-04: 780,520.94
2024-01: 779,762.11
2024-06: 774,944.36
2024-09: 767,923.84
2024-08: 767,494.37
2024-07: 760,788.99
2023-08: 759,753.45
2023-01: 758,792.53
2023-11: 756,441.25
2023-04: 756,042.75
2023-03: 750,609.79
2023-02: 748,740.25
2024-05: 738,188.00
2023-06: 718,943.33
2023-09: 718,813.81
2024-11: 716,230.85
2024-02: 695,275.56
Highest is 2023-07 at 816,530.38.
Chart: line chart (month trend)
---
Q5. What are the total sales in the West region by segment?
Memory recall - you previously asked:
What are the total sales by region?
Show me the top 5 sub-categories by total sales
What is the average profit by category?
Show the monthly sales trend
Tool params: `{'metric': 'sum', 'measure': 'sales', 'group_by': 'segment', 'filters': {'region': 'West'}, 'sort': 'desc', 'limit': None}`
Agent answer:
Sum Of Sales by segment (filtered to region=West):
Consumer: 1,560,246.17
Corporate: 1,524,425.75
Home Office: 1,491,701.29
Highest is Consumer at 1,560,246.17.
Chart: bar chart
---
Q6. Which category has the lowest total profit?
Memory recall - you previously asked:
What are the total sales by region?
Show me the top 5 sub-categories by total sales
What is the average profit by category?
Show the monthly sales trend
What are the total sales in the West region by segment?
Tool params: `{'metric': 'sum', 'measure': 'profit', 'group_by': 'category', 'filters': {}, 'sort': 'asc', 'limit': 1}`
Agent answer:
Sum Of Profit by category:
Office Supplies: 46,510.73
Highest is Office Supplies at 46,510.73.
Chart: bar chart
---
