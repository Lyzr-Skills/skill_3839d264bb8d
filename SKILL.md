---
name: report-parser
description: Use this to turn a raw report email into clean structured text with the employee, date and the items inside it.
---

# Report Parser

## Purpose
Convert one raw report email into clean, structured content that the other skills can compare.

## Steps
1. Remove greetings, signatures, legal disclaimers, auto-footers and quoted earlier replies.
2. Set the report date. Use the date the report states for itself (for example "Report for 14 Oct"). If none is stated, use the date the email was sent.
3. If one employee sent several emails for the same day, combine them into one report for that day.
4. If there is an attachment and its text is readable, include it. If it is not readable, note "attachment not readable" and do not guess its content.
5. Split the content into these groups: work completed, work pending, issues or blockers, requests made to the leader, payments or money items, and next steps.
6. Keep the employee's original wording for each item. Do not rewrite or improve it, because later skills compare exact wording.
7. Record the length: number of lines and whether the report is a single line.

## Output
- Employee
- Report date
- Completed items
- Pending items
- Issues or blockers
- Requests
- Payments
- Next steps
- Line count
- Notes (for example "attachment not readable")
