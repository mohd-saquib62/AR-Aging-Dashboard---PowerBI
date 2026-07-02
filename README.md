# AR-Aging-Dashboard---PowerBI

A Power BI dashboard designed to analyze Accounts Receivable (AR) aging, collection performance, and overdue risk across a simulated dataset of 150 customer invoices.

**Understanding AR Aging**
When a company issues an invoice, the unpaid amount becomes part of its Accounts Receivable. The longer these invoices remain unpaid, the higher the risk of non-collection. AR Aging is the analytical practice of categorizing unpaid invoices by how far past due they are. This allows finance and collections teams to strategically prioritize their efforts on the oldest, highest-risk accounts rather than treating a 5-day overdue invoice with the same urgency as one that is 100 days late.

I built this dashboard to simulate that end-to-end process, transforming raw invoice data into an actionable view for collections management.

Project Scope
**•	Custom Dataset:** A 150-invoice, 25-column dataset created manually to replicate realistic invoice-level data, including customer details, dates, payment modes, collection statuses, and dispute reasons.
**•	Interactive Dashboard:** A two-page Power BI report focusing on AR Overview and Collection Performance.
**•	Custom DAX Measures:** Formulated specifically to calculate Days Sales Outstanding (DSO), Collection Efficiency percentages, and precise overdue amounts.

**Objective**
My goal with this project was to demonstrate the practical reporting responsibilities of an Order-to-Cash (O2C) or Accounts Receivable professional. Rather than simply displaying static numbers, I structured the data to answer the core questions a collections team faces daily: how much capital is at risk, where that exposure is concentrated, and what the root causes are for delayed payments.

**Page 1: AR Overview**
Key Performance Indicators
**•	Total Invoices:** The total volume of invoices raised during the period.
**•	Total Invoice Value:** The gross financial value of all raised invoices, regardless of payment status.
**•	Total Outstanding Amount:** The total capital currently unpaid, encompassing both overdue invoices and those not yet due.
**•	Collection Efficiency:** The percentage of the billed amount that has been successfully collected.
**•	Days Sales Outstanding (DSO):** The average number of days it takes to collect payment after an invoice is raised. A lower DSO indicates healthier cash flow. For example, a DSO of 67 means cash is tied up for roughly 67 days, effectively acting as free credit to customers.
**•	Overdue Invoices:** The volume of invoices that have passed their due date and remain unpaid.

Visual Analytics
**•	Invoices by Collection Status:** A breakdown of invoice volumes into categories like Collected In Time, Collected Late, Partially Collected, and Not Collected. This provides an immediate health check on payment reliability.
**•	Outstanding Amount by Segment:** Highlights unpaid capital divided by customer business size (Enterprise, Mid-Market, SME). Because larger enterprise clients often carry heavier balances, this visual quickly identifies where the most significant financial exposure lies.
**•	Outstanding Amount by Region:** Maps financial exposure across geographic territories to help regional teams assess their specific collection burdens.
**•	Overdue Amount by Aging Bucket:** The core aging visual. It exclusively filters for invoices that are already overdue, categorizing them into 1-30, 31-60, 61-90, and Over 90 Days past due. By deliberately excluding current, not-yet-due invoices, this chart provides an undiluted view of genuine financial risk.

Interactive Slicers
Users can filter the dashboard by Invoice Date, Aging Bucket, Sales Representative, Customer Name, and AR Analyst. This allows for immediate, on-the-fly drill-downs without requiring separate reports.

**Page 2: Collection Performance**

Analytical Tables
**•	Customer Table:** Contrasts the total outstanding amount with the total overdue amount for each customer. Viewing these metrics side-by-side reveals which clients simply have standard open invoices versus those holding genuinely delinquent funds.
**•	AR Analyst Table:** Tracks individual analyst performance by comparing invoice volume, collection efficiency, overdue counts, and disputed accounts. This highlights areas where specific team members might require additional support or process refinement.

Performance Visuals
**•	Collection Efficiency by Sales Rep:** Applies the efficiency metric at the individual representative level to identify which client portfolios yield the most reliable payments.
**•	Amount Received by Payment Mode:** Analyzes successfully collected funds by transaction type (NEFT, Cheque, UPI, RTGS, Letter of Credit) to track customer payment behaviors.
**•	Disputed Invoices by Reason:** Connects collection delays directly to root causes, such as incomplete deliverables or contract mismatches. This crucial view proves that delayed payments are often upstream operational issues rather than a simple refusal to pay.

**Key Takeaways from the Data**
•	The Over 90 Days bucket holds the largest share of overdue capital (₹90.78L), making it the immediate priority for collections.
•	Collection Efficiency varies significantly among analysts (ranging from 74.56% to 90.04%), indicating a clear opportunity for targeted coaching and process alignment.
•	Disputes are heavily concentrated around incomplete deliverables and contract mismatches. Resolving these upstream operational bottlenecks is required to improve downstream cash flow.

**Repository Files**
•	AR_Aging_Dashboard.pbix — The functional Power BI dashboard.
•	AR_Aging_Dataset.xlsx — The underlying 150-invoice dataset.
•	Dashboard screenshots showcasing Page 1 and Page 2.

**Tools Utilized**
Power BI, Power Query (for data cleaning and transformation), Microsoft Excel, and DAX (for calculated measures).

**About the Author**
Built by Mohd Saquib. Drawing on my hands-on background as an Accounts Executive and my MBA in Finance and Marketing, I developed this portfolio project to demonstrate practical expertise in financial reporting, data structuring, and translating complex AR data into actionable business intelligence.

