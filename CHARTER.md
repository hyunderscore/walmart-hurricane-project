# Team Charter: Andrew and Anh

DS2002 Midterm Project, Walmart Hurricane Analytics, Fall 2026

## Roster

| Name | GitHub | Role |
|---|---|---|
| Andrew | [@hyunderscore](https://github.com/hyunderscore) | Cleaning + decision log |
| Anh | [@anhnbach](https://github.com/anhnbach) | Weather API + joins |

- **Main repo:** https://github.com/hyunderscore/walmart-hurricane-project
- **Repo owner:** Andrew

## Part 1: Goals

**What a good result looks like**
- A notebook that runs clean from Restart and Run All
- All five questions answered with code, a number, a chart, and a written finding
- Delivering a good presentation and answering any questions

**What we want to learn**
- Practice building a cleaning pipeline
- Learn how to pull and join API data

**What limits our time**
- Andrew: Other classes
- Anh: Other classes

**What to avoid**
- Starting analysis before the data is clean. We will work on Q1 to Q5 when data cleaning is done.
- Two versions of the notebook. Only the notebook owner commits to `team_notebook.ipynb`.
- Bad communication and division of work.

## Part 2: Who does what

| Job | Owner | Backup | Done when |
|---|---|---|---|
| Cleaning + decision log | Andrew | Anh | One function turns the raw files into clean tables. The log lists every decision and the rows it affected. |
| Weather API + join | Anh | Andrew | One function returns daily weather with retries and a `source` column. The join passes a row-count check. Base URL cited. |
| Analysis Q1 to Q5 | Split (see Part 3) | The other person | Every question has code, a number, and a paragraph. |
| Charts + presentation | Both | Both | At least six labeled plots. The six-minute presentation has been practiced once. |
| README | Both | Both | README explains the project and how to run the notebook. |

**Notebook owner:** rotates weekly. Only the owner commits to `team_notebook.ipynb` and runs Restart and Run All before pushing. Everyone else works in `notebooks/scratch/` and notebook owner commits to main notebook.

| Week | Notebook owner |
|---|---|
| Week 1 (Oct 19 to 23) | Andrew |
| Week 2 (Oct 26 to 30) | Anh |
| Week 3 (Nov 2 to 6) | Andrew |

## Part 3: Question owners

| Question | Owner | Reviewer | Waits on |
|---|---|---|---|
| Q1 Demand surge | Andrew | Anh | Date cleaning |
| Q2 SKU consolidation | Andrew | Anh | SKU mapping table |
| Q3 Weather correlation | Anh | Andrew | Weather API working |
| Q4 Stores and geography | Anh | Andrew | Store ID cleaning |
| Q5 Signal or artifact | Anh | Andrew | SKU and category cleanup |

Q1 and Q3 are worked on first because the other questions depend on clean dates and the weather data.

## Part 4: How we work

- **Where we talk:** text. We reply within a day.
- **When we meet:** Wednesdays at 5 PM, outside class.
- **How we decide:** look at the data first. If we still disagree, the owner of that part decides, and the decision goes in the decision log with the reason.
- **If someone goes quiet:** check in after one day. After two days, check in again. If we have no response, email the professor or TAs.
- **Git:** pull before you start, push before you stop. No keys or tokens in the repo.