# Chore chart app

Tick off each child's jobs, add up their points for the week, and work towards a weekly reward.

Built by MSTR BLDR on **AiRT Official**. For the parent to use, not screen time for the kids.

## What it does

- **Children:** starts with two, "Big kid" and "Little kid". Use nicknames, no full names needed. Add up to four.
- **Today's jobs:** tap a child, then tap a job to tick it (tap again to untick). Each job is worth 1 (quick), 2 (medium) or 3 (big) points.
- **Any day this week:** tap a day from Monday to today to see or fix what was ticked.
- **Points and reward:** points this week, a progress bar to the child's goal, and the reward when the goal is reached. Last week's total is shown underneath.
- **A fresh week every Monday:** the new week starts at 0 points and keeps last week's total.
- **Set up this child:** change the nickname, age group, reward and goal points; load the starter jobs for ages 3 to 5 or 6 to 12; add or remove jobs.
- Saved in this browser only (key `chore-chart-app-data`). Works offline. One file, plain HTML, CSS and JavaScript. No libraries, web fonts, trackers or Ai features.

Pick jobs that suit your child. Help with, and supervise, anything involving heat, knives or cleaning products.

Source for the starter jobs, checked 20 Nov 2026: Raising Children Network, "Household chores for kids" (https://raisingchildren.net.au/preschoolers/family-life/routines-rituals-rules/chores-for-children). The source uses the age groups 2 to 3, 4 to 5, 6 to 11 and 12 to 18; the app's two groups (3 to 5, 6 to 12) and the points are our own grouping and effort rating.

## How it was tested

A sample week (Monday to Thursday) was added up by hand, then checked against the app (`test_app.py` in the studio, 27 checks, all pass).

- Big kid: Mon 4, Tue 7, Wed 6, Thu 5 = 22 points (goal 30, 8 to go). Last week 25.
- Little kid: Mon 3, Tue 4, Wed 2, Thu 5 = 14 points (goal 20). Last week 12.
- Ticking Empty the dishwasher (2), Fold the washing (3) and Vacuum a room (3) on Friday takes Big kid to 30: goal reached.
- On the next Monday, Big kid shows 0 points and "Last week: 30 points".

## How to run

**Use it free:** https://airt-gallery.github.io/chore-chart/

Or run it locally:

1. Download `index.html`.
2. Open it in any modern browser, on your phone or computer.
3. On a phone, use the browser's "Add to Home Screen" so it opens like an app.

## The ASTARR prompt used

PROBLEM: Getting the kids to help around the house turns into nagging, and I lose track of who did what.

ASTARR PROMPT

ACT AS: A parenting educator who builds simple phone apps.

SPECIFIC TOPIC: A weekly chore chart with points for up to four children aged 3 to 12 in an Australian family home. The app is for the parent to tick off jobs, not screen time for the kids.

ACTIONS: Research which household jobs suit each age, from a trusted parenting source. List your sources and flag anything you're unsure of. Give each job points by effort, add a weekly reward goal for each child, and start a fresh week every Monday while keeping last week's total. Test it by ticking a sample week and checking the totals by hand.

RESULT&RULES: I want a mobile app where I tap a child, tick the jobs they did today, and see their points and how close they are to their reward. Starter jobs by age that I can edit, nicknames instead of real names, big buttons, bright friendly colours, saved on this phone only. No connections to the internet or Ai tools.

## Licence

MIT. See [LICENSE](LICENSE).
