# UBER TRIP ANALYSIS

![Page 1](https://github.com/user-attachments/assets/e2589b05-6f06-43e2-8f1b-faddcf043655)

## BUSINESS REQUIREMENT

### Page 1: OVERVIEW ANALYSIS

Analyse Uber trip data using Power BI to gain insights into booking trends, revenue, and trip efficiency, helping stakeholders make data-driven decisions.

#### KPI’s:

      1.	Total Bookings – How many trips were booked over a given period?
      2.	Total Booking Value – What is the total revenue generated from all bookings?
      3.	Average Booking Value – What is the average revenue per booking?
      4.	Total Trip Distance – What is the total distance covered by all trips?
      5.	Average Trip Distance – How far are customers traveling on average per trip?
      6.	Average Trip Time – What is the average duration of trips?

#### Expected Outcomes:
      ✔ Identify trends in ride bookings and revenue generation.
      ✔ Analyse trip efficiency in terms of distance and duration.
      ✔ Compare booking values and trip patterns across different time periods.
      ✔ Provide insights to optimize pricing models and improve customer satisfaction.

#### CHART’s:
      Create a Measure Selector using a Disconnected Table with the following values:
         •	Total Bookings
         •	Total Booking Value
         •	Total Trip Distance
      Then, use a measure to dynamically update the visualizations based on user selection.
      By Payment Type (Card, Cash, Wallet, etc.)
      By Trip Type (Day/Night)

##### Additional Enhancements:
      	Dynamic Title – Update the chart title based on the selected measure.
      	Slicers – Add filters for Date, City, and other interactive filters for deeper analysis.
      	Tooltips – Show  additional details like Average Booking Value or Trip Distance.

Vehicle Type Analysis - Grid View in Power BI
Create a grid table (matrix or table visual) to analyse key performance indicators like Total Bookings, Total Booking Value, Avg Booking Value, Total Trip Distance across different Vehicle Types in Uber trips.

##### Power BI Implementation:
      	Use a Table or Matrix Visual to display Vehicle Type with the KPIs.
      	Apply Conditional Formatting to highlight high and low values.
      	Enable Sorting & Filtering for user interaction.

###### Total Bookings by Day:
      	Detecting trends and fluctuations in daily trip volumes.
      	Identifying peak and off-peak booking days.
      	Understanding the impact of external factors (holidays, events, weather) on ride demand.
      	Supporting strategic planning for resource allocation and pricing adjustments.

###### Location Analysis:
      Understanding trip locations is crucial for optimizing ride distribution, demand forecasting, and operational efficiency. This analysis focuses on:
             Most Frequent Pickup Point
                  • Identify the most common starting locations for trips.
                  •	Helps in optimizing driver availability and dynamic pricing strategies.
             Most Frequent Drop-off Point
                  •	Find the most common drop-off locations.
                  •	Requires activating an inactive relationship in Power BI between Pickup Location and Drop-off Location in the data model.
             Farthest Trip
                  •	Determine the longest trip based on distance travelled.
                  •	Useful for analysing outlier trips, long-distance demand, and fare optimization.
             Total Bookings by Location (Top 5)
                  •	Identify the top 5 locations with the highest trip bookings.
                  •	Helps in demand forecasting and optimizing driver availability in high-traffic areas.
             Most Preferred Vehicle for Location Pickup
                  •	Determine the most frequently booked vehicle type at each pickup location.
                  •	Supports strategic vehicle distribution based on customer preferences and location demand.
### Page 2: TIME ANALYSIS

![Page 2](https://github.com/user-attachments/assets/f66a128a-419c-4c19-85ac-f17678b95add)

To understand trip patterns based on time, Uber needs to analyse ride demand and trends across different time intervals. This dashboard will help in optimizing operations, pricing, and driver availability.
Global Dynamic Measure (Filters All Charts)

            A measure selector will be created for:
                  ✔ Total Bookings
                  ✔ Total Booking Value
                  ✔ Total Trip Distance
            This dynamic measure will update all visuals based on user selection.

#### Visualizations:
      By Pickup Time (10-Minute Intervals) - Area Chart
            • Groups trip bookings into 10-minute intervals throughout the day.
            • Helps in identifying peak and off-peak demand periods.
      By Day Name - Line Chart
            • Shows booking trends across Monday to Sunday.
            • Useful for analysing weekday vs. weekend demand.
      By Hour and Time - Heatmap (Matrix Grid)
            • Rows: Hours of the Day (0–23)
            • Columns: Days of the Week (Mon-Sun)
            • Values: Selected Dynamic Measure (e.g., Total Bookings)
            • Highlights peak booking hours across different days.

### Page 3: DETAILS TAB:

![Page 3](https://github.com/user-attachments/assets/97c2776d-32b8-424e-815e-ccb778bd4183)

To provide in-depth insights and allow users to explore granular data, a Grid Tab will be created. This tab will enable drill-through functionality, allowing users to access detailed records based on selections made in other dashboards.
Features of the Grid Tab:

      	Grid Table with Key Fields:
            • Displays essential trip details
      	Drill-Through Functionality:
            • Users can right-click on a data point from other visuals (e.g., charts, heatmaps) and drill through to this Grid Tab.
            • Displays detailed records related to the selected data point.
      	Bookmark for Full Data View:
            • A "View Full Data" bookmark to toggle between filtered drill-through data and the complete dataset.
            • Allows users to reset filters and see all records easily.
