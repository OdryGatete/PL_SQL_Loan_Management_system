# Phase III: Assumptions – Loan Collateral Management System

1. One customer can apply for multiple loans.  
2. A single loan may have multiple collaterals attached.  
3. Collateral depreciation is calculated using a fixed rate defined by the bank.  
4. Risk scoring for collateral is configurable in the database.  
5. Customers must provide valid national ID numbers for verification.  
6. Each collateral belongs to exactly one customer.  
7. System users are bank employees with proper access rights.  
8. Collateral valuations are performed before collateral evaluation for a loan.  
9. A single collateral can have multiple valuations over time.  
10. Loan approval itself is outside the scope of Phase III – the system only evaluates collateral suitability.  
11. All dates are stored in `DATE` type fields using the system’s standard format.  
12. Serial numbers for collaterals are unique across the system.  
13. Audit logs record every insert, update, or evaluation action in the system for BI tracking.  
14. Collateral types (e.g., car, land, house) are predefined and stored in `COLLATERAL_TYPES`.  
15. Evaluation results are limited to `Acceptable` or `Insufficient` for simplicity.  


