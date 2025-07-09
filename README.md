Blinkit Sales Dashboard
Step-by-Step Process Using Power BI Tools
🔹 Step 1: Data Loading

Tool Used: Power BI Desktop – Power Query Editor

    Comment: Data was imported from sources such as Excel, SQL, or CSV.

    Steps:

        Use “Get Data” to load Blinkit sales data.

        Clean nulls, rename columns, and ensure correct data types (e.g., dates, currency, integers).

🔹 Step 2: Data Transformation

Tool Used: Power Query Editor

    Comment: Necessary fields like Total Sales, Fat Content, Avg Ratings were cleaned and calculated.

    Steps:

        Add calculated columns for metrics like Total Sales, Avg Sales.

        Apply filters for relevant years or item types.

        Split columns if needed (e.g., separating "Outlet Location" into tier types).

🔹 Step 3: Data Modeling

Tool Used: Data Model (Manage Relationships)

    Comment: Relationships between tables like Outlet, Item Types, and Sales were built.

    Steps:

        Create relationships using primary/foreign keys.

        Ensure correct one-to-many relationships for dimension tables (e.g., Item Types to Sales).

        Set default summarizations (SUM, AVERAGE).

🔹 Step 4: Creating Measures

Tool Used: DAX (Data Analysis Expressions)

    Comment: Custom measures like Average Sales, Total Sales, No of Items, and Average Ratings were created.

    Examples:

    Avg_Sales = AVERAGE(Sales[SalesAmount])
    Total_Sales = SUM(Sales[SalesAmount])
    No_of_Items = SUM(Sales[ItemCount])
    Avg_Rating = AVERAGE(Sales[Rating])

🔹 Step 5: Visualization

Tool Used: Report View

    Comment: Multiple charts and cards were used to display data insights.

    Visuals Used:

        Cards: For Total Sales, Avg Sales, Avg Ratings.

        Bar Charts: Sales by Item Type, Outlet Type, Fat Content.

        Column Charts: Outlet Establishment Year vs. Sales.

        Pie Charts/Donut Charts: Distribution by Outlet Location (Tier 1, 2, 3).

        Slicers: For filtering data by Item Type, Location.

🔹 Step 6: Filter Panel and Interactivity

Tool Used: Slicers & Filters Pane

    Comment: Slicers allow dynamic filtering for better insights.

    Steps:

        Add slicers for Location, Item Type, and Outlet Type.

        Enable cross-filtering between visuals.

🔹 Step 7: Formatting & Layout

Tool Used: Format Pane

    Comment: Uniform font, color themes, and layout were applied for a professional look.

    Steps:

        Adjust colors to represent performance (green for high sales, red for low).

        Align visuals, apply labels and tooltips.

        Add titles and subtitles for clarity.

🔹 Step 8: Dashboard Publishing

Tool Used: Power BI Service

    Comment: The final dashboard was likely published to Power BI Service for sharing.

    Steps:

        Click “Publish” to upload the report.

        Set up dashboard views, add collaborators, and enable scheduled refreshes if needed.

 Summary Comments on Tools Used
        | Feature       | Tool             | Use Case                                   |
| ------------- | ---------------- | ------------------------------------------ |
| Data Import   | Power Query      | Load and clean sales and outlet data       |
| Relationships | Model View       | Link sales, item types, outlet info        |
| Metrics       | DAX              | Create custom KPIs like Avg Sales, Ratings |
| Charts        | Visualizations   | Bar, Column, Card, Slicer, Filter          |
| Layout        | Format Panel     | Font, alignment, background colors         |
| Interaction   | Slicers          | Dynamic filtering by type or location      |
| Sharing       | Power BI Service | Publishing and distribution                |
