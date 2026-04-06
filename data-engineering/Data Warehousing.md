Data Warehousing is the process of collecting, organizing, and managing data from disparate data sources to provide meaningful business insights and forecasts to respective users. It serves as the foundation for reliable reporting and analysis of large amounts of data across different organizational levels, from customer service to executive decision-making.

## Key Characteristics of Data Warehouses

- **Subject-Oriented** - provides information catered to a specific subject instead of the organization. 
	- Examples: product information, sales data, customer and supplier details, etc.
- **Integrated** - Combine data from multiple sources, i.e. flat files, RDBMS, APIs, etc. 
- **Time-Variant** - Information from a specific point in time.
- **Non-volatile** - All data is immutable. New data shouldn't mutate/update/delete old data.

## Data Warehouse Architectures

- **Single-tier Architecture**: Simplest form, monolithic, data can connect to any other data
- **Two-tier Architecture**: Separates data storage from presentation. Where presentation unidirectionally references the underlying storage layer,
- **Three-tier Architecture aka [[Medallion Architecture | Medallion]]**: Most common, with separate layers for data sources (raw), structured data warehouse, and presentation

## Types of Data Warehouses
| Type                                | Description                                                                                | Use Case                                                                 |
| ----------------------------------- | ------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------ |
| **Enterprise Data Warehouse (EDW)** | Central database for enterprise-wide decisions and complex queries.                        | Executive reporting, cross-departmental analytics, organization-wide BI. |
| **Operational Data Store (ODS)**    | Real-time database serving as staging area between operational systems and data warehouse. | Real-time operational reporting, employee records, feeding data to EDW.  |
| **Data Mart**                       | Department or business unit-specific subset of data warehouse.                             | Department analytics, regional reporting, specialized user group needs.  |
## Data Integration Approaches

- **Query-Driven** - Create custom integrators and wrappers on top of different databases.
- **Update-Driven** - Combine and integrate before storing in a data warehouse.

## Business Benefits

- Improved access to data for end-users
- Better data consistency
- Lower costs for reads on structured data
- Separation of concerns for business intelligence and operational systems.

## Industry Applications

| Industry                     | Description                                                                                              | Use Case                                                                                       |
| ---------------------------- | -------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------- |
| **Investment and Insurance** | Analyze customer and market trends with real-time data streaming for time-sensitive financial decisions. | Market analysis, customer behavior tracking, risk assessment, real-time trading decisions.     |
| **Retail**                   | Support distribution and marketing operations through comprehensive item and customer analytics.         | Inventory tracking, pricing optimization, promotional analysis, customer buying patterns.      |
| **Healthcare**               | Forecast patient outcomes and generate comprehensive treatment reporting for various stakeholders.       | Patient outcome prediction, treatment reports, insurance data sharing, research collaboration. |
|                              |                                                                                                          |                                                                                                |
## The Role of Data Pipelines

A data warehouse is populated using data pipelines. They transport raw data from disparate sources to a centralized data warehouse for reporting and analytics. Along the way, the data is transformed and optimized.

Modern data warehousing emphasizes automation in pipeline creation, with key capabilities including:
- Incremental loading using change data capture
- Job monitoring and scheduling
- Automated transformations
- Real-time or near-real-time data processing

## Modern Considerations

Contemporary data warehousing has evolved to address the challenges of big data, requiring:
- Automated pipeline creation and management
- Cloud-native architectures
- Support for both structured and unstructured data
- Real-time processing capabilities
- Integration with modern analytics and AI/ML platforms`
}


