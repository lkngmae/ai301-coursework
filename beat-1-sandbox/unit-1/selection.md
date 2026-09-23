# Unit 1 — Issue Selection

Path: `beat-1-sandbox/unit-1/selection.md`

Record of the issue carried into Unit 2, and of the evaluation runs that produced
`eval-run.txt`. This file is graded at the path above; a copy kept anywhere else in
the repository is not read.

Complete every labelled field below. Each is graded on its own; content placed under the
wrong label is not graded.

---

## Selected issue

**Issue link**

https://github.com/codepath/pathreview-ai301-fa26-s1/issues/61

**Verdict output**

[Your skill's live-mode output for this issue, pasted verbatim and ending with the
fenced JSON verdict block. A summary does not satisfy this field.]

**The verdict must record `accept` for this issue.** Choose an issue your own skill
accepts. If your skill rejects every candidate you try, that is a signal about your
rubric rather than about the issues: revise it and re-run — retries are unlimited and a
partial re-run costs about $0.20 — or run the skill on different candidates. Output
recording `reject` for the issue you chose earns no credit for this field.

```
1. #61 — Health check DB probe passes a raw SQL string — accept
The only candidate that passes the preferred Clear specification check: the body carries an explicit **Steps to reproduce:** heading and the literal error text (ArgumentError: Textual SQL expression 'SELECT 1' should be explicitly declared as text('SELECT 1')). Zero comments, zero cross-references, one file (api/routes/health.py), a one-line sqlalchemy.text() wrap. Cleanest of the three.

  {
    "item": "https://github.com/codepath/pathreview-ai301-fa26-s1/issues/61",
    "checks": [
      {"name": "Maintainer is alive", "grade": "pass", "evidence": "Aburke225 (COLLABORATOR) committed to main 2026-09-16, 7 days before the 2026-09-23 grading date."},
      {"name": "Repo is in use", "grade": "pass", "evidence": "repo pushed_at 2026-09-16T21:48:27Z; archived: false."},
      {"name": "Issue is not taken", "grade": "pass", "evidence": "assignees: []; 0 comments; timeline shows only 4 label events, no cross-references or linked PRs."},
      {"name": "Policy allows contribution", "grade": "pass", "evidence": "docs/CONTRIBUTING.md states 'Fork the repository... Comment on the issue to let others know you're working on it' — no AI ban, no assignment requirement, repo not archived."},
      {"name": "Scope fits newcomer", "grade": "pass", "evidence": "Labeled 'good first issue' and 'tier-1'; fix is wrapping a literal 'SELECT 1' in sqlalchemy.text() in api/routes/health.py."},
      {"name": "Clear specification", "grade": "pass", "evidence": "Body has an explicit '**Steps to reproduce:**' heading plus the concrete ArgumentError message."}
    ],
    "verdict": "accept"
  },

```

---

## Eval iterations

Quote source text directly in each field below. Paraphrase does not satisfy them.

**Run history**

[The agreement score of each run you did, in order. A single run is a complete answer if
only one run occurred. **The last score in your list must match the agreement line in the
`eval-run.txt` you committed** — that file is the record of your final run.]

**Issue analysis**

[One scored issue, identified by id (`issue-01` through `issue-20`; the `calib-`
issues are not scored). State your rubric's decision, the gold label, and the
reasoning that produced your rubric's result.]

**Check rationale**

[One check from the `rubric.md` uploaded to `tools/issue-select/`, quoted as it is
currently written, with the reasoning behind its current form.]

**Trade-offs**

[What the quoted check gives up. Any one of these is a complete answer: an issue whose
result it changes, a canary you re-ran with `--only`, a case you accept it will miss, or a
stated reason nothing changed elsewhere. "Nothing changed, and here is how I know" earns
the point in full when the reason follows.]

---

## Selection rationale

Graded on whether all three are answered, in your own words. Not on how good the
reasoning is, and not on length — a short honest answer to each earns the full marks.
This is also the basis for the claim comment you write in Unit 2.

**Selection rationale**

[Answer all three:

1. The issue's fit to your interests and to the time available.
2. What the verdict identified correctly, and what you weighed that the rubric could
   not.
3. The anticipated difficulty in claiming it.]

---

Related paths: `eval-run.txt` in this directory; your skill's files in
`tools/issue-select/`.
