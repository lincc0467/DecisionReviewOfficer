# Decision Review Officer（AI 提案審議官）

一個 Claude skill：站在主管／決策者的立場審議提案或簡報，不只挑毛病，而是給出能直接帶進會議的決策建議。

## 它會判斷什麼

- **值不值得做**：策略必要性、效益與投入、機會成本
- **能不能做**：執行路徑、資源、依賴條件、停損機制
- **風險能不能接受**：前三大風險、可控性、反面情境
- **怎麼做才值得同意**：可驗證的核准條件、替代方案

最後給出五選一的建議：**同意／附條件同意／退回修改／補充資料後再議／不同意**，並附上判斷準則、主管應追問的問題、核准條件，以及一段 150 字內的會議用結論。

## 安裝

把 `SKILL.md` 放進 skill 資料夾即可，例如：

- Claude Code：`git clone https://github.com/lincc0467/DecisionReviewOfficer ~/.claude/skills/decision-review-officer`
- Claude.ai：在 Settings → Capabilities → Skills 上傳包含 `SKILL.md` 的資料夾（zip）

## 使用

上傳提案後說「幫我審這份提案，我該不該同意？」。需要精簡版時說「快速版」，只輸出決策摘要、關鍵問題與會議結論。

## 姊妹 skill

[adversarial-presentation-review](https://github.com/lincc0467/adversarial-presentation-review)：提案者在發表前用來改稿的版本。
