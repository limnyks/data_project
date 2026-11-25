# data_project


Executive summary of task 



The database supports how a state archive handles a **property request**,
from registering the application to issuing an archival certificate.
Based on scenario 09, "State archive: archival evidence request", from the course catalogue.

## Scope
- Request type: **property requests**, limited to **civil-law transactions**
  (sale, gift, inheritance, etc.) involving real estate.
- Out of scope: decisions of public authorities, movable property, OCR and digitisation,
  legal assessment of the applicant's entitlement.
- All data is synthetic.



## Data model (9 tables)
| Table | Purpose |
|---|---|
| `requests` | Requests, their status, who registered them and who is handling them |
| `findings` | Search log: documents examined and which ones were used in the response |
| `responses` | Response versions, result, reviewer, issue date |
| `employees` | Archive staff: intake workers, archivists, reviewers |
| `documents` | Document catalogue with archival reference (fond, inventory, file, sheet) |
| `events` | Property events (transactions) with type, date and price |
| `objects` | Real-estate objects: address, type, area |
| `people` | Applicants, transaction participants, document signatories |
| `event_participants` | Event participants and their roles (seller, buyer, …) |


