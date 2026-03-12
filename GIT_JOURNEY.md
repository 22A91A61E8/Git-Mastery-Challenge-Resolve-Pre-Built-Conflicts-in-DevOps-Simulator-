&#x20;# Git Mastery Challenge Journey



\## Student Information

\- \*\*Name:\*\* Srikanth

\- \*\*Student ID:\*\* 22A91A61E8

\- \*\*GitHub Repository:\*\* \[GitHub Repo](https://github.com/22A91A61E8/Git-Mastery-Challenge-Resolve-Pre-Built-Conflicts-in-DevOps-Simulator-.git)

\- \*\*Date Started:\*\* 12 Mar 2026

\- \*\*Date Completed:\*\* 12 Mar 2026



\---



\## Task Summary

Cloned the instructor's repository with pre-built conflicts and successfully resolved all merge conflicts across multiple branches using proper Git workflows. Configured personal GitHub repository for submission.



\---



\## Commands Used



| Command | Times Used | Purpose |

|---------|------------|---------|

| git clone | 1 | Cloned instructor's repository |

| git checkout | 20+ | Switch between branches |

| git branch | 10+ | View and manage branches |

| git merge | 2 | Merge `dev` and `conflict-simulator` into `main` |

| git add | 30+ | Stage resolved conflicts |

| git commit | 15+ | Commit resolved changes |

| git push | 10+ | Push changes to personal repository |

| git fetch | 2 | Fetch updates from instructor |

| git pull | 1 | Pull updates from instructor |

| git stash | 2 | Save temporary work |

| git cherry-pick | 1 | Apply a specific commit |

| git rebase | 1 | Rebase a feature branch |

| git reset | 3 | Undo commits (soft/mixed/hard) |

| git revert | 1 | Safe undo |

| git tag | 2 | Create annotated release tags |

| git status | 50+ | Check repository state |

| git log | 30+ | View commit history |

| git diff | 20+ | Compare changes |



\---



\## Conflicts Resolved



\### Merge 1: `main` + `dev` (6 files)



1\. \*\*config/app-config.yaml\*\*  

&#x20;  - Issue: Production used port 8080, development used 3000  

&#x20;  - Resolution: Unified config using environment variables  

&#x20;  - Strategy: Keep production defaults, dev optional  

&#x20;  - Difficulty: Medium  

&#x20;  - Time: 15 mins  



2\. \*\*config/database-config.json\*\*  

&#x20;  - Issue: Different hosts, SSL modes, pool sizes  

&#x20;  - Resolution: Added separate profiles for production and development  

&#x20;  - Strategy: JSON structure supports multiple environments  

&#x20;  - Difficulty: Medium  

&#x20;  - Time: 10 mins  



3\. \*\*scripts/deploy.sh\*\*  

&#x20;  - Issue: Production vs Docker Compose logic  

&#x20;  - Resolution: Conditional deployment based on `DEPLOY\_ENV`  

&#x20;  - Strategy: Single script handles both environments  

&#x20;  - Difficulty: Hard  

&#x20;  - Time: 20 mins  



4\. \*\*scripts/monitor.js\*\*  

&#x20;  - Issue: Different intervals and logging formats  

&#x20;  - Resolution: Environment-based config object  

&#x20;  - Strategy: `process.env.NODE\_ENV` determines behavior  

&#x20;  - Difficulty: Medium  

&#x20;  - Time: 15 mins  



5\. \*\*docs/architecture.md\*\*  

&#x20;  - Issue: Different architectural descriptions  

&#x20;  - Resolution: Combined into a comprehensive doc  

&#x20;  - Strategy: Added sections per environment  

&#x20;  - Difficulty: Easy  

&#x20;  - Time: 10 mins  



6\. \*\*README.md\*\*  

&#x20;  - Issue: Different feature lists and versions  

&#x20;  - Resolution: Merged features, clearly labeled per environment  

&#x20;  - Difficulty: Easy  

&#x20;  - Time: 10 mins  



\---



\### Merge 2: `main` + `conflict-simulator` (6 files)



\- Fetched remote branch first (`instructor/conflict-simulator`)  

\- Merged into `main` successfully  

\- Resolved conflicts in similar files as above  

\- Committed and pushed to `origin/main`  



> All merge conflicts resolved, working tree clean.



\---



\## Challenges / Warnings



\- Initially missing local `conflict-simulator` branch (solved by fetching and creating local branch tracking instructor)  

\- Python AI analyzer script missing: `scripts/ai-analyzer.py`  

&#x20; - Fix: Documented placeholder; monitoring still functional  

\- Understanding `<<<<<<< HEAD`, `=======`, `>>>>>>> dev` markers took careful reading  



\---



\## Testing \& Verification



\- Ran `scripts/deploy.sh` for production and development environments  

\- Verified monitoring (`monitor.js`) works for AWS, Azure, GCP  

\- AI optimization and predictions functioning (some warnings due to missing script)  

\- No errors after merge resolution  



\---



\## Git Workflow Insights



\- Conflicts are normal; careful review is key  

\- `git fetch` + `git merge instructor/<branch>` is safer than merging missing local branch  

\- `git status` and `git log` are crucial for tracking changes  

\- Cherry-pick, rebase, reset, and revert help manage complex histories  

\- Keep calm and test frequently after merges  



\---



\## Key Learnings



1\. Mastered resolving merge conflicts across multiple environments  

2\. Learned best practices for environment-based scripts and configuration  

3\. Practiced advanced Git commands (`rebase`, `cherry-pick`, `reset`, `revert`)  

4\. Learned to document workflow for reproducibility  



\---



\## Repository Snapshot



\### Branches



```text

main

dev

conflict-simulator

