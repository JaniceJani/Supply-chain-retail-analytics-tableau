Supply Chain & Retail Analytics Dashboards — EDEN RESTAURATION & VOLTAIRE

Overview
This project delivers interactive Tableau dashboards across two real French companies — a national catering and food service operator and a multi-location bookstore group. Built as part of a Data Visualisation with Tableau course at EDHEC Business School, the work involved end-to-end dashboard development: from raw data ingestion and cleaning, through KPI definition and calculated field construction, to final multi-stakeholder dashboard design.
Each set of dashboards was built as a proof of concept (POC) for data-driven decision-making within the respective organisation, with outputs designed for use by different stakeholder levels — from operational teams to senior management.

View Dashboards Live
Project	Tableau Public Link
EDEN RESTAURATION	View Dashboards →

VOLTAIRE	View Dashboards →

Full Tableau Public Profile	View All Work →



Part 1 — EDEN RESTAURATION (Supply Chain Analytics)
Company Context
EDEN RESTAURATION is a French catering company with a focus on sustainable and ethical sourcing — prioritising local and seasonal ingredients, short supply chains, and responsible procurement practices.

Project Objective
The company's IT department provided a one-month sample dataset and engaged the team to explore the data, design interactive dashboards to track key supply chain metrics, and propose recommendations for optimising logistics, procurement, and inventory management.

Data Sources
Two datasets were used and joined on regional codes:
eMarket_Cmd2019-11.xlsx — Primary dataset covering product deliveries for November 2019. Key fields include site details (SiteCode, SiteName, RegionCode), logistics and supplier information (Plateforme, Fournisseur, DateLivraison, DateEnvoiCmd), and product specifics (Categorie, Famille, SousFamille, ProduitDesignation, QteUC, PrixUC, Marque, Origine).
regions_eden.xlsx — Secondary reference table mapping regional codes to administrative regions of France (RegionCode, RegionName, RegionFrance).
Key Metrics
Metric	Value
Total Revenue	€27.15M
Total Deliveries	726,540
Average Delivery Time	5.13 days
Data Period	November 2019

Dashboards
1. Business Performance Overview – November 2019 - Top-level revenue and operational KPIs for November 2019. Tracks overall business performance, delivery volumes, and period metrics for management reporting. Designed for General Management and strategic decision-making.
2. Supply Chain Performance - Tracks delivery lead times, distribution volumes across platforms (Plateforme), and supplier-level performance. Highlights the 5.13-day average delivery time and identifies logistics bottlenecks across the supply network.
3. Sustainability and Procurement Insights - Analyses local vs. non-local product sourcing by origin (Origine field) across French administrative regions. Tracks procurement cost differentials between local and imported goods, and provides visibility into supplier and product category diversity to support EDEN's sustainability commitments.

Part 2 — VOLTAIRE (Bookstore Analytics)
Company Context
VOLTAIRE is a French multi-location bookstore group operating under two brands — Librairie L'Éclat and Bouquin & Cie — serving both B2C (consumer) and B2B (professional) markets across multiple French regions.

Project Objective
VOLTAIRE engaged the team to develop an interactive analytics application in Tableau to monitor daily store activity across the group. Dashboards were designed for five distinct stakeholder levels: General Management, Regional Management, Store Management, Store Teams (Supervisors), and Management Control.

Data Sources
Six Excel datasets were integrated, cleaned, and joined in Tableau:
Dataset	Contents
SALES.xlsx	Transaction-level sales data — date, item, store, unit cost, selling price (incl. 5.5% VAT), quantity (negative = returns), transaction type (B2C / B2B)
PURCHASES_AND_RETURNS.xlsx	Supplier purchase and return transactions — date, item, store, unit cost, quantity, type (Purchase / Return)
STOCKS.xlsx	Monthly stock snapshots — item, store, weighted average purchase cost, public selling price, quantity in stock
ENTRANCES_AND_EXITS.xlsx	30-minute interval foot traffic data — entrances, exits, tickets sold, sales in euros per interval
STORES.xlsx	Store reference data — store name, postal code, location type, brand, geographic coordinates, regional zone, surface area
ITEMS.xlsx	Product reference data — item label, category, sub-category

Data quality issues (missing values, inconsistent records) were identified and addressed during the cleaning and preprocessing phase.

Key Metrics
Metric	Value
YTD Revenue	€7.77M
Gross Margin	29.11%
Store Conversion Rate	33.63%
Datasets Integrated	6

Dashboards
4. Business Overview - Group-level dashboard for General and Regional Management. Tracks YTD revenue, gross margin, sales trends over time, and performance comparisons across stores, brands (Librairie L'Éclat vs. Bouquin & Cie), and geographic zones (ZONE SUD, ZONE NORD, etc.). Includes B2C vs. B2B revenue breakdown and best-selling article categories.
5. Business Overview – Mobile - A mobile-optimised version of the Business Overview dashboard, condensed to highlight the most critical KPIs for on-the-go decision-making by Store and Regional Management. Designed for narrow-screen display with simplified layout and clear visual hierarchy.
6. Store Operations - Operational dashboard for Store Management and Store Teams. Built on the ENTRANCES_AND_EXITS dataset — tracks foot traffic patterns (entrances, exits, peak 30-minute intervals), tickets sold, and the 33.63% store conversion rate (entrances vs. sales transactions) across store locations.
7. Financial & Inventory Overview - Financial and stock management dashboard for Management Control. Tracks gross margin by store, category, and brand; inventory levels and stock movement from the STOCKS dataset; supplier purchase and return rates from PURCHASES_AND_RETURNS; and average basket value by transaction type (B2C / B2B).

Technical Notes
•	Primary tool: Tableau Desktop (packaged workbooks — .twbx)
•	Data preparation: Excel (data cleaning, field standardisation prior to Tableau ingestion)
•	Dashboard design: Multi-stakeholder architecture with filters, tooltips, drill-down navigation, and mobile-responsive layout for VOLTAIRE
To open: Tableau Desktop or Tableau Public (free) required to view .twbx files interactively.

Files
└── README.md
Note: Both Tableau workbooks are published on Tableau Public — use the links at the top to view all dashboards interactively in your browser without needing Tableau installed. Underlying datasets are not included — data was provided under academic licence and is not publicly shareable.

Context
Course: Data Visualisation with Tableau — MSc Data Analytics & AI 
Institution: EDHEC Business School 
Period: October – November 2025 
Team project

