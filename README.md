# Tactile Deep Learning: Part B (Group XX)

![Module](https://img.shields.io/badge/ELEC70129-Deep%20Learning-1f4e79)
![Direction](https://img.shields.io/badge/direction-to%20decide%2027%20Nov-lightgrey)
![Next deadline](https://img.shields.io/badge/next%20deadline-charter%2029%20Nov-orange)
![Part B due](https://img.shields.io/badge/Part%20B%20due-20%20Dec%202026-b31b1b)

Our group workspace for the ELEC70129 Part B project: a tactile perception problem for a real stakeholder, a working proof of concept, and a video of at most 5:00. Everything we write or code lives here. Video footage and large files live in our Teams/OneDrive folder.

> **Start here:** read [the brief on one page](docs/01_brief.md), then [how we are marked](docs/02_marking.md), then [the directions](docs/03_directions.md) before the meeting.

## Status

| Item | State |
|---|---|
| Direction | Not chosen yet (meeting on Fri 27 Nov) |
| Paper(s) we build on | To decide |
| Dataset | To decide |
| Stakeholder | To decide |
| Next deadline | Charter and direction paragraph, **Sun 29 Nov, 23:59** |
| Final deadline | Video, code zip and contributions form, **Sun 20 Dec, 23:59** |

## Key dates

| Date (2026) | What | Owner |
|---|---|---|
| Fri 27 Nov | First meeting: direction, roles, charter | Everyone |
| **Sun 29 Nov, 23:59** | Signed charter + one-paragraph direction on Canvas ([charter](admin/CHARTER.md), [paragraph](admin/DIRECTION.md)) | Coordinator |
| 30 Nov to 4 Dec | Progress check with the TA (Week 4) | Everyone |
| Mon 7 Dec | Last sensible day to escalate an unresolved group problem to the TA | Coordinator |
| Sun 13 Dec, 23:59 | **Part A due** (individual, never shared here) | Each of us |
| **Sun 20 Dec, 23:59** | **Part B due**: video, code zip, contributions form, then email to the TA | Coordinator |
| Wed 23 Dec, 23:59 | Peer assessment closes (everyone rates everyone) | Each of us |

Our internal plan is in [docs/05_timeline.md](docs/05_timeline.md).

## The team

| Name | GitHub | Lead role | Also helps with |
|---|---|---|---|
| | | Coordinator and stakeholder lead | |
| | | Research and novelty lead | |
| | | Data lead | |
| | | Modelling lead | |
| | | Evaluation and demo lead | |
| | | Video producer | |

What each role owns: [docs/04_roles.md](docs/04_roles.md).

## How we work

1. **Actions are GitHub Issues.** One issue per action, assigned to one person, with the due date in the title, for example `Download Touch and Go subset (due 1 Dec)`. Close it with a link to the evidence. This doubles as our contribution record for peer assessment.
2. **Minutes go in [minutes/](minutes/)** within 24 hours of each meeting, one file per meeting, from the [template](minutes/TEMPLATE.md).
3. **Decisions go in [admin/DECISIONS.md](admin/DECISIONS.md)**, one line each, so nobody has to scroll a group chat.
4. **Each of us keeps a contribution log** in [admin/contribution_logs/](admin/contribution_logs/). Five minutes a week; it protects your peer factor.
5. **Notebooks:** the modelling lead owns [notebooks/poc_starter.ipynb](notebooks/poc_starter.ipynb). Everyone else experiments in `notebooks/scratch/<yourname>_<topic>.ipynb` and the modelling lead merges what works. Two people editing one notebook in git creates conflicts that are painful to fix.
6. **Training runs in Colab.** Open a notebook from GitHub in Colab, save checkpoints to Google Drive, and save the notebook back with *File > Save a copy in GitHub*.
7. **Never commit data, weights or video.** The [.gitignore](.gitignore) blocks the usual file types. Data stays where you downloaded it; large shared files go in Teams/OneDrive.

## Repository map

```
.
├── README.md                  this page: status, dates, team, how we work
├── docs/
│   ├── 01_brief.md            Part B on one page
│   ├── 02_marking.md          the 40 marks and what earns them
│   ├── 03_directions.md       directions A to G, and how we choose
│   ├── 04_roles.md            the six roles
│   ├── 05_timeline.md         internal plan with a Gantt chart
│   ├── 06_reading_list.md     papers and datasets, with links
│   └── 07_rules_and_checklist.md   rules that protect our marks, final checklist
├── admin/
│   ├── CHARTER.md             draft charter (sign and upload by 29 Nov)
│   ├── DIRECTION.md           direction paragraph (upload by 29 Nov)
│   ├── DECISIONS.md           decisions log
│   ├── RISKS.md               risk register
│   └── contribution_logs/     one log per member
├── minutes/                   one file per meeting
├── notebooks/
│   └── poc_starter.ipynb      proof-of-concept skeleton (runs in demo mode now)
├── video/
│   └── STORYBOARD.md          5-minute storyboard mapped to the marks
└── .github/ISSUE_TEMPLATE/    templates for actions and decisions
```

## Rules we never break

- **Part A stays out of this repo.** No Part A code, weights, results or report text, ever. Part A is individual.
- **No Part A data and no GelSight subsets of TacVerse** in Part B.
- **Choose models on the validation set only.** The test set is used once, for the final numbers.
- **Cite everything we did not make**: papers, datasets, pretrained weights, adapted code, figures, music.
- **Declare AI use.** Any AI-tool use goes in our contribution logs and in the group's AI-use declaration.

Full list: [docs/07_rules_and_checklist.md](docs/07_rules_and_checklist.md).

## Contacts

- Lecturer: Dr Dandan Zhang, d.zhang17@imperial.ac.uk
- Teaching assistant: Ms Lan Wei, l.wei24@imperial.ac.uk
- Email subject for every inquiry: `[2026-Deep-Learning-Inquiry]-[Your Name]`
- Handbook, announcements, group registration and submissions: Canvas.
