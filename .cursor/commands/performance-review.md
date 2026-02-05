# Performance Review Workflow

Run the automated performance review workflow for a direct report.

## Usage

Type `/performance-review` in Cursor chat, then provide:

1. **Person's name** (must be in Direct Reports Database)
2. **Base directory path** where their files are located
3. **Review period start date** (e.g., 01/01/2025)
4. **Review period end date** (e.g., 12/31/2025)
5. **Review year** (e.g., 2025)

## What It Does

Loads the automation workflow from `prompts/performance-review-workflow-automation.md`, fills in the person's information, and executes all 7 phases automatically with progress tracking.

---

**Implementation:**

Load the performance review workflow automation from: `/Users/emiliano/Library/Mobile Documents/com~apple~CloudDocs/Cursor/Writing/prompts/performance-review-workflow-automation.md`

I will provide the person's information. Once I do, replace the bracketed placeholders in the Master Execution Prompt section with:
- [PERSON'S NAME] → The person's name I provide
- [BASE DIRECTORY PATH] → The base directory path I provide
- [START DATE] → The start date I provide
- [END DATE] → The end date I provide
- [YEAR] → The review year I provide

Then execute the complete workflow automatically, running all 7 phases sequentially with progress tracking.

Please prompt me for:
1. Person's name (must be in Direct Reports Database)
2. Base directory path where their files are located
3. Review period start date (e.g., 01/01/2025)
4. Review period end date (e.g., 12/31/2025)
5. Review year (e.g., 2025)
