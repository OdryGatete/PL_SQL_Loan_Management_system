# Data Dictionary – Loan Collateral Management System

## Customers
| Column | Type | Key |
|--------|------|-----|
| customer_id | NUMBER | PK |
| full_name | VARCHAR2(100) |  |
| national_id | VARCHAR2(25) | UNIQUE |
| phone | VARCHAR2(20) |  |
| created_at | DATE |  |

## Loans
| Column | Type | Key |
|--------|------|-----|
| loan_id | NUMBER | PK |
| customer_id | NUMBER | FK → Customers.customer_id |
| loan_amount | NUMBER(12,2) |  |
| loan_status | VARCHAR2(20) |  |
| request_date | DATE |  |

## Collateral
| Column | Type | Key |
|--------|------|-----|
| collateral_id | NUMBER | PK |
| loan_id | NUMBER | FK → Loans.loan_id |
| type_id | NUMBER | FK → Collateral_Types.type_id |
| market_value | NUMBER(12,2) |  |
| manufacture_year | NUMBER |  |
| serial_number | VARCHAR2(50) | UNIQUE |
| condition_status | VARCHAR2(20) |  |

## Collateral_Types
| Column | Type | Key |
|--------|------|-----|
| type_id | NUMBER | PK |
| type_name | VARCHAR2(50) |  |
| depreciation_rate | NUMBER(5,2) |  |

## Collateral_Evaluation
| Column | Type | Key |
|--------|------|-----|
| evaluation_id | NUMBER | PK |
| collateral_id | NUMBER | FK → Collateral.collateral_id |
| evaluated_value | NUMBER(12,2) |  |
| coverage_percentage | NUMBER(5,2) |  |
| risk_level | VARCHAR2(20) |  |
| evaluation_date | DATE |  |

## Collateral_Documents
| Column | Type | Key |
|--------|------|-----|
| document_id | NUMBER | PK |
| collateral_id | NUMBER | FK → Collateral.collateral_id |
| document_type | VARCHAR2(50) |  |
| verification_status | VARCHAR2(20) |  |
| uploaded_at | DATE |  |

## Audit_Log
| Column | Type | Key |
|--------|------|-----|
| audit_id | NUMBER | PK |
| table_name | VARCHAR2(50) |  |
| action_type | VARCHAR2(20) |  |
| user_name | VARCHAR2(50) |  |
| action_time | DATE |  |

