# Plan to build 1000 ICP-qualified companies in one month

The goal is not to create a large raw database, but to build a verified list of 1000 genuinely ICP-qualified companies with evidence-backed qualification. The process should prioritize quality over volume, automation with human verification, and a repeatable sourcing pipeline.

### 1. Build the initial universe
I would start by building a universe of roughly 3,500 to 4,000 companies from multiple overlapping sources: DSIR-recognized R&D units, ABLE and biotech association directories, BSE SME / NSE Emerge, regulator and approval lists, exhibitor directories, and company databases such as The Company Check and BioPharmGuy. These sources are useful because together they capture established manufacturers, regulated companies, and active growth-oriented firms.

### 2. Apply hard pre-filters
Before any AI scoring, I would remove obvious non-fits such as traders, distributors, service-only firms, generic pharma, PE-controlled companies, companies with no meaningful website, revenue above the threshold, and companies with no visible recent activity. This saves both time and API cost and keeps the scoring pipeline focused on plausible ICP candidates.

### 3. Automate qualification
For each company, I would scrape the website, about page, leadership page, products page, news page, and careers page. That text would then be passed into an AI model for structured scoring against the six Federer criteria: manufacturer, India-based, differentiated, technical decision-maker, growing sector, and active growth signals. The output would be forced into a JSON format containing score, evidence, confidence level, and verdict so that the result remains auditable and easy to review.

### 4. Add quality control
Quality control would happen in three layers. First, the hard filters remove obvious junk before scoring. Second, borderline or low-confidence cases would be re-scored using a stronger model or a second-pass prompt. Third, a manual QA layer would review all borderline companies and a sample of strong-pass companies to catch false positives, bad evidence, or hallucinated claims.

### 5. Weekly execution

- Week 1: Build the source universe and create the master database with company name, website, city, segment, and source tag. Expected output: 3,500 to 4,000 raw companies, with most having usable websites or digital footprints.dsir.

- Week 2: Run scraping and first-pass AI scoring on the full universe. Expected output: 2,000 to 2,500 screened companies after automatic disqualification, and around 1,200 to 1,400 first-pass qualified companies.

- Week 3: Re-score borderline companies, manually verify low-confidence results, and clean up obvious false positives and duplicates. Expected output: around 1,000 to 1,200 companies remaining after QA.

- Week 4: Final review, deduplication, and assembly of the final 1,000-company list. Add personalization hooks for the highest-priority companies and prepare the final spreadsheet plus methodology note.

### 6. Final deliverable
The final output would include company name, website, city, segment, revenue band, decision-maker, six criterion scores, evidence points, final verdict, confidence level, and personalization hook. The result should be a clean, evidence-backed list that can directly support outreach and sales research.
