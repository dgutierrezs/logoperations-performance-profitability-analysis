# Logistic Operations Performance Profitability and Analysis

Análisis desarrollado como parte de mi transición hacia data science, aplicando Python y pandas a problemas reales de logística y optimización de rutas. Las bases de datos estan obtenidas en Kaggle.

En este caso, utilizo SQL mediante Python, para que se puedan observar facilmente los resultados con JupyterNotebook. 

Logistics Route Profitability Analysis
This project analyzes route-level profitability and route consistency in a logistics network. The goal is to identify which routes generate the most value, which ones consistently lose money, and which routes show unstable performance.

Objective
Identify which routes generate real profitability after operational costs and which ones are structurally unprofitable.

Key Questions
Are high-demand routes always profitable?
Which routes consistently lose money?
Can we segment routes based on performance?
Key Result
A small number of routes are structurally unprofitable, while most of the network operates efficiently. Profitability is driven by unit economics rather than volume.

Data Overview
The dataset represents a logistics operation over a 3-year period (2022–2024), covering key aspects of fleet management, shipments, and operational performance.

It includes multiple interconnected tables that simulate a real-world relational database, allowing analysis across different dimensions such as routes, drivers, costs, and operational events.

Key Data Entities
Loads: Shipment-level data including revenue, customer, and route information
Trips: Execution-level data capturing actual trip performance (duration, fuel usage, etc.)
Routes: Origin-destination pairs with distance and structural information
Drivers: Driver details and performance-related attributes
Fuel Purchases: Fuel transactions associated with trips
Delivery Events: Operational events such as pickups, deliveries, and delays
Safety Incidents: Records of accidents or operational issues
Maintenance Records: Truck service history and associated costs
Data Relationships
The dataset follows a relational structure where:

Each load is linked to a route and a customer
Each trip represents the execution of a load and is linked to a driver, truck, and trailer
Operational data such as fuel purchases, delivery events, and incidents are tied to individual trips
This structure enables analysis from planned operations (loads/routes) to actual performance (trips and events).

Data Considerations
Some datasets may contain missing or inconsistent values
Aggregated tables (e.g., monthly metrics) are excluded from detailed analysis to maintain granularity
Cost calculations are primarily based on fuel data, as other cost components may not be fully available
