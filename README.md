# Maven-Sales-Challenge


## MavenTech Sales Snapshot: CRM-driven Performance Dashboard
### Visualise Team and Individual Performance: 2017 Quarterly Insights with Power BI

### Data
This dataset, available on [Maven Analytics](https://mavenanalytics.io/data-playground), contains B2B sales opportunities from a CRM database for a fictitious company (MavenTech) that sells computer hardware, including information on accounts (customers), products sold, sales teams, and sales opportunities (sales pipeline data).

The data model was simple, and the dataset did not need much cleaning except for a couple of things:
- In the sales pipeline table, I changed the product name from "GTXPro" to "GTX Pro" to ensure consistency when merging the sales pipeline and product tables. A simple find and replace value within Power Query was sufficient. 
- I did a basic merge of the sales pipeline and product tables using the related "product" column to align the data.
- Furthermore, I merged the sales teams with the sales pipeline table based on the sales agent column to integrate relevant information on managers.

I used Power BI to build the report. Find it [here](https://github.com/umasreeakula/Maven-Sales-Challenge/blob/main/MavenTech%20-%20Quarterly%20Sales%20Team%20Performance.pbix).

### Business Scenario:
MavenTech is a company based in the United States that sells computer hardware to large businesses. Recently, MavenTech implemented a new CRM system to manage its sales opportunities. However, the company faces a challenge: limited visibility of the sales data beyond the CRM platform.
As a BI Developer for MavenTech, I have developed an interactive dashboard to enable sales managers to track their team's quarterly performance effectively. MavenTech can now extract valuable insights from sales data from the CRM system, making it easier to make data-driven decisions.

#### Assumptions:
- The dashboard prioritises detailed performance insights at an individual level, reflecting the assumption that sales managers are primarily concerned with assessing the performance of team members. This approach allows for benchmarking individuals against each other. Teams can access each other's performance data, enabling comparative analysis to assess relative performance across teams.
- The dashboard allows managers to retrospectively analyse performance over the year, organised by quarters, to track and evaluate long-term progress effectively.

The dashboard is user-friendly and includes help tooltips and text for interpreting the graphs, metrics and how to access information from them.

### What information is available to managers in the dashboard?
- Quarterly Performance Overview: The dashboard provides a comprehensive overview of a team's performance for each quarter, including the performance of each sales agent, which, when compared with team performance metrics, will enable managers to identify top performers, areas for improvement, and coaching opportunities.
- Individual Sales Rep Performance: Sales managers can evaluate the performance of individual sales agents through a variety of metrics, including:
	- Total sales
	- Number of deals closed (won and lost)
	- Win rates
	- Average deal size
	- Average time taken to win and close deals
 
The report also offers an overview of the percentage of discounted opportunities by each individual, followed by the average discount percentage they have given away, providing insights into which individuals give away a higher proportion of sales in discounts. Understanding the discounts offered can demonstrate their impact on the average opportunity size.

- Deal Pipeline Analysis: Managers can explore the overall sales pipeline to understand the distribution of deals across various stages (e.g., prospecting, engaging, closed-won, closed-lost), helping them prioritise efforts and allocate resources efficiently.
- Product Sales: Managers can obtain a comprehensive overview of product sales for each quarter, including insights into the number of products sold within their opportunities.
- Performance by Sales Teams: Managers can view where they stand relative to other teams in performance in each metric.
- Quarter-over-Quarter Performance Summary: Managers can gain insights into the overall team's performance changes quarter-over-quarter. They can also delve into each sales agent's quarter-over-quarter performance, examining total sales, deals won, win rates, average deal size, and the time taken to close winning deals. 

The report also highlights the number of deals lost by the team and individual members, alongside the wins. It also includes the potential sales of each team to give an overview of the impact the engaging deals have.

### Key Metrics:
Based on the available data, I selected the following sales metrics for performance comparison:
- Sales: Income received from the sales of the hardware products.
- Wins: These are deals that result in a purchase of the product. How many deals do they need to land to meet targets?
- Win-Rate: How well can the agents in the team conclude negotiations and make a sale? This metric is calculated by dividing the number of wins by the total of closed (both won and lost) deals.
- Average Deal/Opportunity Size: Calculated by dividing the total value of every deal by the number of deals won within the quarter. It measures the size of incoming sales opportunities.
- Average Time to Close (successful deals only): The time taken to close a winning deal from initial contact. Faster closures mean more time is available to pursue additional deals.

These metrics enable managers to gauge the effectiveness of their team's and agents' sales strategy and process in successfully closing deals and identifying particular strengths and opportunities on the team.

### The Dashboard:
The report's first page is a detailed summary of the team's and the sales reps' performances for the selected quarter. Managers can utilise two drop-down menus—one for choosing their name and the other for choosing a quarter. Upon selecting/hovering over a visual, managers can hover over it to find a tooltip (represented by a question mark) for assistance in interpreting the visual.
The cards at the top represent the team's averages for the key metrics, serving as benchmarks to evaluate individual team members' performance. The table and accompanying graphs summarise the sales agents' quarter performance. To view their specific results, clicking on a sales agent's name in the table will update the graphs accordingly.
The graph depicting pipeline stages offers an overview of the pipeline at the end of the year, along with potential closing sales. 
Explore the graph representing the team's closed-won and closed-lost deals in more detail to analyse the breakdown for each sales representative. The tooltip provides additional assistance.

![MavenTech - Selected Quarter Performance](https://github.com/umasreeakula/Maven-Sales-Challenge/assets/163797397/7398ea83-cf19-4639-91a9-a15b1a706251)

The second page provides an overview of performance by every team in each metric. Managers can observe where their team ranks relative to others in performance by the metric for every quarter if they'd like to know. They can utilise the drop-down menu to select a specific quarter for analysis.

![MavenTech - Selected Quarter Team Performance Ranking](https://github.com/umasreeakula/Maven-Sales-Challenge/assets/163797397/ddad30dc-4a51-4254-88b9-823e5ef46705)

The third page offers a quarter-over-quarter performance summary for managers to analyse how the team and individual sales agents have performed in the current quarter (selected from the drop-down menu) compared to the previous quarter. Clicking on a bar in any of the graphs can highlight the specific results for the individual, including the sales results from the table.

![MavenTech - QoQ Performance Summary](https://github.com/umasreeakula/Maven-Sales-Challenge/assets/163797397/a12949a7-955d-4d07-a51a-5a51686713cf)

Graphs on the second and third pages also feature tooltips for additional assistance, similar to the first page of the report. These tooltips become available upon selecting or hovering over the visuals, providing helpful information to managers as needed.
