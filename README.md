What problem does it solve?

Normally, construction costing may involve:

Quantity
×
Rate
=
Amount

For hundreds or thousands of items, manually calculating this can cause errors.

Example

Suppose a project requires:

Item	Quantity	Unit	Rate
Cement	500	Bags	₹400
Steel	2,000	Kg	₹65
Cable	1,500	Meter	₹120

The system calculates:

Cement

500 × ₹400 = ₹2,00,000

Steel

2,000 × ₹65 = ₹1,30,000

Cable

1,500 × ₹120 = ₹1,80,000

Total:

₹2,00,000
+ ₹1,30,000
+ ₹1,80,000
----------------
₹5,10,000

Instead of doing this manually, Excel can automate it.

Possible Excel structure
Input sheet
Item Code
Item Description
Quantity
Unit
Rate
Calculation
=Quantity*Rate
Output
Item       Qty     Rate      Amount
Cement     500     400       200000
Steel      2000     65       130000
Cable      1500    120       180000
                              ------
Total                         510000
Where Alteryx comes in

Suppose data comes from:

Excel 1 → Material
Excel 2 → Labour
Excel 3 → Rates
Excel 4 → Project quantities

Alteryx can combine these:

Material ──┐
Labour ────┤
Rates ─────┼──→ Alteryx Workflow → Clean Dataset
Quantity ──┘

Then the final data can go into Excel/reporting.

Main benefit

The resume describes the system as reducing manual calculation errors and reducing costing turnaround time.
