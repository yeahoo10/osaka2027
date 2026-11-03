# 2027 日本大阪京都家族旅行專案規範 (GEMINI.md)

本專案核心行為準則與引擎分工規則已統一定義於 [AGENTS.md](file:///c:/Users/yeaho/OneDrive/文件/claudeuse/2027日本大阪行/AGENTS.md)。

---

## 核心規則精要速覽

1. **成員與步調守則**：
   - 2027/2/24～3/3 關西 8 天 7 夜（京都 2 晚 + 大阪 5 晚）。
   - 6 大 + 2 幼（3歲/5歲）+ 1 嬰（第4天加入）。
   - 每日大景點最多 2 個，無障礙電梯動線第一，嚴禁急行軍拉車。

2. **引擎調用優先層級（嚴格遵守零費用）**：
   - **第一優先（無消耗）**：`travel-themeparks`（USJ / 樂高排隊與維護）、`travel-weather`（即時天氣）。
   - **第二優先（AI 攻略）**：`travel-tavily`（每月 1,000 次，專搜 PTT / Dcard 親子避坑、長輩推車心得）。
   - **第三優先（精確地圖）**：`travel-planner` / Google Maps API（點對點轉乘、官方營業時間）。
   - **第四優先（戰略比價）**：`travel-flights` & `travel-hotels`（SerpAPI，每月 250 次，嚴格限制「僅查機票與飯店即時含稅價」）。

3. **路書維護原則**：
   - 更新每日行程時，同步維護 [index.html](file:///c:/Users/yeaho/OneDrive/文件/claudeuse/2027日本大阪行/index.html)。
   - 確保手機端與電腦端 RWD 閱讀體驗。
   - 線上即時路書：`https://yeahoo10.github.io/osaka2027/`。
