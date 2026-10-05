# My lab evidence / 我的實作紀錄

- Group code / 組別：Not provided
- Tool / 工具：Codex agent, GitHub CLI (`gh`), Git, PowerShell, Node.js
- Route / 路線：Individual, agent-assisted local execution; this is not a student classroom run
- Tasks completed / 完成題目：A, B v1, B revision (v2), D
- Material / 素材：NDHU classroom tasks 東華課堂版
- For original-pack work / 原版實作：Not applicable
- My role and what I checked / 我的角色與實際檢查：The Codex agent created and checked the files in this repository. No personal student observations are claimed.

## Scope and plan / 範圍與計畫

Allowed input and output folders / 可讀取與輸出的資料夾：`practice/01-club-files/input/` → `practice/01-club-files/output/`; `practice/02-campus-picker/activities.json` → `practice/02-campus-picker/output/index.html`; `practice/04-review/bad-plan.txt` was read to write `practice/04-review/my-rejection.md`. Git metadata and GitHub CLI were used only to publish this practice repository.

What I asked for / 原始需求：Complete the practice repository using GitHub CLI, following its README and classroom handout.

What I checked before execution / 動手前我檢查了什麼：Confirmed Git and GitHub CLI were available, checked the authenticated GitHub account, read the repository instructions and task handout, inspected the supplied fictional input files, and confirmed the task output folders did not already exist.

## Tests actually performed / 我真的做過的測試

| Test / 測試 | Expected / 預期 | Observed / 實際 | Evidence / 證據 |
|---|---|---|---|
| A: inventory, manifest and copy integrity | 12 input files, 12 manifest entries, one exact copy per source, all originals preserved | 12 entries and copies found; SHA-256 matched for every source/copy pair. Identical announcement and equipment files were copied separately; both differing proposal versions remain. | Local PowerShell count, manifest path checks and SHA-256 comparison |
| B: picker behavior | Filters all apply; outdoor/15/medium has no match; outdoor/30/medium yields A09; history caps at five; reset keeps history; language and clear controls work | All checks passed using a Node.js VM harness with a minimal DOM stub. The page has no external script or stylesheet references. | Temporary local harness (not included in the submission); implementation is `practice/02-campus-picker/output/index.html` |

## One revision / 一次修改

Before / 原來的情況：In B v1, switching language updated the controls and history, but the currently displayed picked activity kept its previous language.

Request / 我提出的修改：After a successful pick, switch the interface language and confirm the currently displayed activity name and details update too.

After and retest / 修改後與重測結果：B v2 stores the current pick and redraws it after language changes. The Node.js behavior harness confirmed that the displayed activity uses the selected language and the five-item history remains intact.

New requirement or defect? / 新需求還是原規格未做到？：Revision to meet the original bilingual activity-name requirement consistently.

## One rejection / 一次退回

Which action I reject and why / 退回哪個動作、為什麼：Rejected the plan in `practice/04-review/bad-plan.txt` because it expands to all Downloads, deletes files, infers approval from a filename, guesses missing values, and publishes automatically.

An acceptable alternative / 可以怎麼改：Stay inside the selected fictional task folder, propose changes before executing, preserve originals and all differing versions, flag uncertainty for human review, and do not publish.

## Still unverified / 還沒驗證

What I cannot claim is complete / 哪些事不能說已完成：No browser-based visual/mobile inspection or screenshot of the running page was captured. The learning record is an agent execution record, not a student's personal reflection or classroom observation. No group code was supplied.
