# Market-Analysis-in-Dublin-Project
Airbnb: Identify demand-supply gaps using search pattern and acceptance rate analysis. Python, Pandas, Seaborn, NumPy
## Project Overview 
A new Airbnb City Manager in Dublin wants to understand what guests are searching for and which booking inquiries hosts are most likely to accept.

The goal is to analyze guest demand and host supply, identify gaps that may be limiting bookings, and recommend ways to better match supply with demand. The analysis should also highlight any additional data that would help improve understanding of the Dublin market.

##Key Analysis and Findings

Here are the key findings from your Dublin market analysis project:

## Key Findings

**Guest demand vs. supply mismatch**
- **1 guest** is the most commonly *searched-for* group size, but **2 guests** is the most common size that actually gets *booked*. This suggests a shortage of good single-guest/solo accommodation options in Dublin relative to demand.

**Booking funnel drop-off**
- Of all contacts made: ~92% get a reply, ~46% get accepted, and only ~28% turn into an actual booking — meaning most host contacts never convert into a booking.
- Overall acceptance rate across contacts averages **43%**.

**Price doesn't drive rejection**
- Acceptance rates stay roughly similar across all price bands (0–100 up to 600+), meaning guests aren't getting rejected more often just because they filtered for higher prices. Price isn't the main driver of host acceptance.

**Search timing & stay length**
- All searches in the dataset fall within a tight window (Oct 1–14), with no major day-to-day variation.
- Most searches are for short-to-moderate stays (skewed distribution, with the bulk of `n_nights` well under 20).
- Most guests search fairly close to their check-in date (most `length_preparation` values are under 100 days).

**Room type preferences**
- Entire home/apt and private rooms dominate search filters, with shared rooms far less common — though this column has messy/repeated values that would benefit from cleaning (only 4 real Airbnb categories exist: Entire Place, Private Room, Hotel Room, Shared Room).

**Country-level anomaly**
- **India** stands out with a notably low acceptance rate (~15%) — roughly half that of the next-lowest country. Flagged as worth investigating further (could be pricing behavior, listing type preference, host bias, or a data artifact).

**Data quality note**
- All numeric columns are highly right-skewed (skewness > 1), so median-based summaries are more reliable than means throughout this dataset.

---



## Repository Structure
|File/Folder  | Description|
|---------------|-------------------------------|
|assets|There are 2 datasets, searches.tsv - Contains a row for each set of searches that a user does for Dublincontacts.tsv - Contains a row for every time that an assigned visitor makes an inquiry for a stay listing in Dublin|
|Market-Analysis-in-Dublin-Project.ipynb|The main Jupyter Notebook containing all the data cleaning, exploration, and analysis code.|

