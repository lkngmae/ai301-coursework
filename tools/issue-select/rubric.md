# Rubric: is this a good first issue?

<!--
THIS IS THE PART YOU WRITE. The skill in SKILL.md executes whatever checks
you define here. It ships empty on purpose: the judgment is your work.

A filled rubric must contain:

1. At least one row in the checks table. Each row needs all four columns:
   - Check: a short name (used in the output JSON).s
   - Evidence: exactly what to look at, and where. Name the source
     (repo-facts block, issue body, comment thread, or the locations in
     references/evidence-guide.md). "The repo" is not a source; "the last
     5 default-branch commit dates" is.
   - Pass condition: a condition someone else could apply and get your
     answer. Prefer thresholds with numbers ("a maintainer commented
     within 30 days") over adjectives ("maintainer is responsive").
   - Weight: `required` (a fail here rejects the issue) or `preferred`
     (never changes the verdict; a nice-to-have that helps rank the
     issues you accept).

2. A verdict rule below the table: how the check grades combine into
   accept or reject, including how `unclear` is treated. The verdict
   space is binary. If you write no rule for `unclear`, the skill treats
   it as fail.

Cover what actually kills first contributions. The lecture named four
families: the maintainer is alive, the repo is in use, the scope fits a
newcomer, and nobody else is already on it. A rubric that ignores a family
will fail eval issues designed around that family.
-->

## Checks

| Check | Evidence | Pass condition | Weight |
|---|---|---|---|
| Maintainer is alive | Issue comment thread, repo-facts block (recent commit/PR merge dates) | A maintainer has commented on an issue, merged a PR, or committed to the default branch within the last 60 days. | required |
| Repo is in use | repo-facts block (default-branch commit dates or releases) | The last default-branch commit or release date is no more than 60 days old. | required |
| Scope fits newcomer | Issue labels and issue body | Has a label indicating beginner friendliness (e.g., "good first issue", "help wanted", "beginner") OR It MUST NOT involve major architectural changes, unbounded new feature development, or affect a large number of files. | required |
| Issue is not taken | Issue sidebar (assignees, linked PRs) and issue comment thread | No assignees, no linked open/approved PRs, and no comments from anyone claiming they are working on it from within the past 60 days (unless a maintainer explicitly released/unassigned them). | required |
| Policy allows contribution | repo-facts block (CONTRIBUTING.md, repo status) and issue comment thread | The repo is NOT archived. The rules do NOT pause community PRs, do NOT forbid this specific type of change (like typos), and do NOT contain rules requiring you to be assigned by a maintainer before opening a PR. | required |
| Clear specification | Issue body | The description contains explicit headings like "Steps to reproduce", "Expected behavior", or a concrete code snippet demonstrating the error.| preferred |


## Verdict rule

Accept if every check passes and rank as highest; reject if any required check is not passed (unsure and failed both will fail the issue overall); preferred checks never change the verdict, but passing more preferred checks ranks the issue higher in the outcome; For each check, Pass is ranked highest, followed by unsure, and fail is the lowest.
