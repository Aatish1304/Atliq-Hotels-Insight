# Atliq-Hotels-Insight
Dashboard Link : (https://app.powerbi.com/links/FApgF60kiK?ctid=a3da1a5e-6af9-42be-8ad1-2a9b41101b90&pbi_source=linkShare)
Problem Statement
This dashboard helps hospitality businesses understand their performance better. It provides insights into customer satisfaction, service quality, and operational efficiency. Through different metrics, they can identify areas of improvement and enhance their strategies. It also provides insights into average guest ratings and occupancy trends, helping businesses address challenges and optimize operations.
Since the percentage of neutral or dissatisfied customers (almost 57%) is higher than satisfied customers (around 43%), businesses must work on improving their services and guest experiences.
Additionally, since average occupancy rates in certain locations are lower, businesses should strategize to improve occupancy and revenue in these areas.
Steps Followed
Step 1: Load data into Power BI Desktop, dataset is a CSV file.
Step 2: Open Power Query Editor and, under the "View" tab in the "Data Preview" section, check "Column Distribution," "Column Quality," and "Column Profile" options.
Step 3: Since profiling is by default limited to 1000 rows, select "Column Profiling Based on Entire Dataset."
Step 4: Identify and handle null values. For instance, the "Guest Ratings" column had some missing data, which was excluded from calculations as it comprised less than 1% of the dataset.
Step 5: Select a theme in the "Report View" for consistent design.
Step 6: Add visuals to represent various metrics, such as guest ratings, occupancy trends, and customer demographics, using the visualizations pane.
Step 7: Use slicers for key fields, such as "Location," "Room Type," and "Customer Type."
Step 8: Create card visuals to display key metrics, such as total revenue, average guest rating, and total number of bookings.
Null values were excluded from average calculations using visual-level filters.
Step 9: Add a bar chart to visualize occupancy rates by room type, segmented by location.
Step 10: Create measures and calculated columns to enhance data analysis:
Calculated Column: Segment guests into different satisfaction categories using the following DAX expression:
Satisfaction Category = IF(hospitality_data[Guest Rating] <= 2, "Dissatisfied", IF(hospitality_data[Guest Rating] <= 4, "Neutral", "Satisfied"))
Step 11: Add KPI cards to highlight:
Total Revenue
Occupancy Rate
Average Guest Rating
Step 12: Use stacked bar charts and pie charts for visual representation of:
Booking distribution by location
Room types contributing to revenue
Guest demographics, such as age groups and spending behavior
Step 13: Add text boxes and shapes for dashboard titles, subtitles, and highlighting specific insights.
Step 14: Publish the report to Power BI Service for collaboration and sharing.
Insights
Key takeaways from the Hospitality Insight Dashboard:
Total Revenue: $X (adjusted dynamically with slicers)
Top Performing Location: Location A with $Y in revenue
Underperforming Location: Location B with $Z in revenue
Room Performance:
Best-performing room type: Deluxe
Least-performing room type: Standard
Guest Segments:
Satisfied Guests: 43%
Neutral Guests: 30%
Dissatisfied Guests: 27%
Demographic Trends:
Majority of guests are aged 25-45 years.
High spenders predominantly fall in the 35-45 age group.
Average Guest Rating: 4.2/5
Recommendations
Focus marketing efforts on underperforming locations.
Enhance service quality in neutral or dissatisfied guest categories.
Provide targeted promotions and packages to increase occupancy in low-performing room types.
Analyze guest feedback to address common pain points and improve satisfaction.
Next Steps
Implement advanced analytics, such as predictive modeling, to forecast future occupancy trends.
Integrate real-time data feeds for up-to-date insights.
Enhance the dashboard with more interactive visuals, such as drill-through reports and what-if analyses.
