# Learning.md

## Day 3 – Data Management

### Topics Learned

#### 1. Data Management in Salesforce

* Data management is the process of importing, exporting, updating, deleting, and maintaining data in Salesforce.
* It ensures data remains accurate, consistent, and useful for business operations.
* Good data management improves reporting, dashboards, and decision-making.

#### 2. Data Import Wizard

* Used to import data into Salesforce through a simple web-based interface.
* Supports standard objects such as Accounts, Contacts, Leads, and custom objects.
* Allows field mapping between CSV columns and Salesforce fields.
* Suitable for administrators who need an easy way to import data.

#### 3. Data Loader

* Data Loader is a client application used for bulk data operations.
* Supports Insert, Update, Upsert, Delete, and Export operations.
* Can handle large volumes of records.
* Uses CSV files for data processing.
* Provides error and success logs after execution.

#### 4. Import Wizard vs Data Loader

| Feature        | Import Wizard        | Data Loader         |
| -------------- | -------------------- | ------------------- |
| User Interface | Web-based            | Desktop Application |
| Record Limit   | Smaller Data Volumes | Large Data Volumes  |
| Delete Support | No                   | Yes                 |
| Export Support | No                   | Yes                 |
| Upsert Support | Limited              | Yes                 |
| Ease of Use    | Easy                 | Moderate            |

#### 5. Data Migration

* Data migration is the process of moving data from one system to another.
* Common migration sources include Excel files, databases, and legacy applications.
* Planning and data cleaning are essential before migration.
* Validation and testing help ensure successful migration.

#### 6. Data Quality

* Data quality refers to the accuracy, completeness, consistency, and reliability of data.
* Poor-quality data leads to incorrect reports and business decisions.
* Data validation rules help maintain quality.

#### 7. Duplicate Management

* Duplicate records create confusion and reduce productivity.
* Salesforce provides Matching Rules and Duplicate Rules to identify and prevent duplicates.
* Duplicate Management helps maintain a single source of truth.

#### 8. Common Data Quality Problems

* Missing email addresses
* Incorrect phone numbers
* Duplicate records
* Invalid status values
* Inconsistent naming conventions
* Blank mandatory fields
* Incorrect addresses
* Outdated information
* Data entry mistakes
* Formatting inconsistencies

#### 9. Enterprise Impact of Poor Data

* Incorrect reports
* Inaccurate dashboards
* Wrong business decisions
* Duplicate communications
* Failed notifications
* Reduced customer satisfaction
* Lower sales productivity
* Compliance risks
* Data migration failures
* Loss of management trust in reports

### Practical Understanding

* Learned how to import records using Data Import Wizard.
* Learned how to update records using Dataloader.io.
* Understood field mapping during imports.
* Practiced creating matching rules for duplicate detection.
* Learned how organizations maintain clean and reliable data.

### Key Takeaway

Clean and accurate data is essential because every report, dashboard, automation, and business decision depends on the quality of the underlying data. Effective data management improves productivity, customer relationships, and overall organizational success.
