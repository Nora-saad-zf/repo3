# 🏭 AdventureWorks Sales Analytics Dashboard (Power BI)

A professional sales performance dashboard built with Power BI using the AdventureWorks dataset. Features interactive visualizations, drill-down capabilities, and time intelligence analysis.

## 📊 Key Features
- **Star Schema Data Model** with optimized relationships
- **Multi-date analysis** (Order Date, Ship Date, Due Date) using `USERELATIONSHIP`
- **Dynamic hierarchies** for Products and Dates
- **Cross-filtering** with synchronized slicers
- **Drill-through** capabilities between report pages

## 🛠️ Technical Implementation

### Data Model
```mermaid
graph TD
    vw_FactOrderDetails -->|Relationships| vw_DimProducts
    vw_FactOrderDetails -->|Relationships| vw_DimSalesPersons
    vw_FactOrderDetails -->|Relationships| vw_DimShipMethods
    vw_FactOrderDetails -->|Relationships| vw_DimStatuses
    vw_FactOrderDetails -->|Relationships| vw_DimTerritories
    vw_FactOrderDetails -->|Multiple Date Relationships| DimDates


📂 Data Sources
AdventureWorks Database: https://docs.microsoft.com/en-us/sql/samples/adventureworks-install-configure?view=sql-server-ver15&tabs=ssms
