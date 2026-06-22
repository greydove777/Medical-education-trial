# 教學解答與專家回顧 (Answer Key & Expert Debriefing)

> ⚠️ 建議先完成 `case.md` 中的任務後再閱讀本檔案。

<style>
.dx-flip-grid {
  display: flex;
  flex-wrap: wrap;
  gap: 18px;
  margin: 20px 0;
}
.dx-flip-card {
  width: 220px;
  height: 210px;
  perspective: 1200px;
}
.dx-flip-card input[type="checkbox"] {
  display: none;
}
.dx-flip-inner {
  position: relative;
  display: block;
  width: 100%;
  height: 100%;
  cursor: pointer;
  transition: transform 0.6s;
  transform-style: preserve-3d;
}
.dx-flip-card input:checked ~ .dx-flip-inner {
  transform: rotateY(180deg);
}
.dx-flip-front, .dx-flip-back {
  position: absolute;
  top: 0; left: 0;
  width: 100%;
  height: 100%;
  backface-visibility: hidden;
  border-radius: 14px;
  box-sizing: border-box;
  padding: 14px;
  overflow-y: auto;
}
.dx-flip-front {
  background: linear-gradient(135deg, #eef2ff, #e0e7ff);
  border: 2px solid #6366f1;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  text-align: center;
}
.dx-flip-front .dx-rank {
  font-size: 0.8em;
  color: #6366f1;
  font-weight: bold;
  margin-bottom: 6px;
}
.dx-flip-front .dx-name {
  font-weight: bold;
  font-size: 1em;
  line-height: 1.4;
}
.dx-flip-front .dx-hint {
  margin-top: 10px;
  font-size: 0.78em;
  color: #6b7280;
}
.dx-flip-back {
  background: #fffbeb;
  border: 2px solid #f59e0b;
  transform: rotateY(180deg);
  font-size: 0.82em;
  line-height: 1.5;
}
.dx-flip-back b {
  color: #92400e;
}
</style>

---

## 0️⃣ 生命徵象判讀 (Vital Signs Interpretation)

> 💡 點擊卡片翻面，看看每個數值背後隱藏的臨床意義。

<div class="dx-flip-grid">

<div class="dx-flip-card">
  <input type="checkbox" id="vs-card-1">
  <label for="vs-card-1" class="dx-flip-inner">
    <div class="dx-flip-front">
      <div class="dx-rank">血壓</div>
      <div class="dx-name">178/96 mmHg</div>
      <div class="dx-hint">👆 點擊翻面看意義</div>
    </div>
    <div class="dx-flip-back">
      <b>判讀：</b>未超過 rt-PA 給藥門檻 (<185/110 mmHg)，<b>不需要</b>額外降壓即可準備給藥；需留意是否為長期未規律服藥的慢性高血壓所致
    </div>
  </label>
</div>

<div class="dx-flip-card">
  <input type="checkbox" id="vs-card-2">
  <label for="vs-card-2" class="dx-flip-inner">
    <div class="dx-flip-front">
      <div class="dx-rank">心率 / 心律</div>
      <div class="dx-name">92 bpm<br>節律不規則</div>
      <div class="dx-hint">👆 點擊翻面看意義</div>
    </div>
    <div class="dx-flip-back">
      <b>判讀：</b>不規則心律提示心房顫動 (Atrial Fibrillation) 可能，須安排 12-lead ECG 確認；亦提示可能病因為<b>心源性栓塞 (cardioembolic stroke)</b>
    </div>
  </label>
</div>

<div class="dx-flip-card">
  <input type="checkbox" id="vs-card-3">
  <label for="vs-card-3" class="dx-flip-inner">
    <div class="dx-flip-front">
      <div class="dx-rank">血氧</div>
      <div class="dx-name">SpO2 98%<br>(room air)</div>
      <div class="dx-hint">👆 點擊翻面看意義</div>
    </div>
    <div class="dx-flip-back">
      <b>判讀：</b>正常，無明顯低氧，暫無立即呼吸道處置或氧氣治療需求
    </div>
  </label>
</div>

<div class="dx-flip-card">
  <input type="checkbox" id="vs-card-4">
  <label for="vs-card-4" class="dx-flip-inner">
    <div class="dx-flip-front">
      <div class="dx-rank">體溫</div>
      <div class="dx-name">36.8°C</div>
      <div class="dx-hint">👆 點擊翻面看意義</div>
    </div>
    <div class="dx-flip-back">
      <b>判讀：</b>正常，無發燒徵象，降低中樞神經感染或敗血症相關腦病的可能性
    </div>
  </label>
</div>

<div class="dx-flip-card">
  <input type="checkbox" id="vs-card-5">
  <label for="vs-card-5" class="dx-flip-inner">
    <div class="dx-flip-front">
      <div class="dx-rank">指尖血糖</div>
      <div class="dx-name">142 mg/dL</div>
      <div class="dx-hint">👆 點擊翻面看意義</div>
    </div>
    <div class="dx-flip-back">
      <b>判讀：</b>可初步排除低血糖這個 stroke mimic；血糖過高（通常 >185 mg/dL）才會是 rt-PA 相對禁忌考量之一，本案數值不構成顧慮
    </div>
  </label>
</div>

</div>

---

## 1️⃣ NIHSS 逐項計分

> 💡 點擊每張卡片翻面，核對你的評分是否正確。

<div class="dx-flip-grid">

<div class="dx-flip-card">
  <input type="checkbox" id="ns-card-1">
  <label for="ns-card-1" class="dx-flip-inner">
    <div class="dx-flip-front">
      <div class="dx-rank">1a. 意識水平 (LOC)</div>
      <div class="dx-name">清醒，可自發睜眼</div>
      <div class="dx-hint">👆 你給幾分？</div>
    </div>
    <div class="dx-flip-back">
      <b>給分：0</b><br>清醒、可自發反應，無意識障礙
    </div>
  </label>
</div>

<div class="dx-flip-card">
  <input type="checkbox" id="ns-card-2">
  <label for="ns-card-2" class="dx-flip-inner">
    <div class="dx-flip-front">
      <div class="dx-rank">1b. LOC 問題</div>
      <div class="dx-name">回答含糊但內容正確</div>
      <div class="dx-hint">👆 你給幾分？</div>
    </div>
    <div class="dx-flip-back">
      <b>給分：1</b><br>答對但因構音/語言受影響而不清楚，非完全答錯
    </div>
  </label>
</div>

<div class="dx-flip-card">
  <input type="checkbox" id="ns-card-3">
  <label for="ns-card-3" class="dx-flip-inner">
    <div class="dx-flip-front">
      <div class="dx-rank">1c. LOC 指令</div>
      <div class="dx-name">正確完成兩項指令</div>
      <div class="dx-hint">👆 你給幾分？</div>
    </div>
    <div class="dx-flip-back">
      <b>給分：0</b><br>兩項指令皆正確完成
    </div>
  </label>
</div>

<div class="dx-flip-card">
  <input type="checkbox" id="ns-card-4">
  <label for="ns-card-4" class="dx-flip-inner">
    <div class="dx-flip-front">
      <div class="dx-rank">2. 凝視</div>
      <div class="dx-name">雙眼水平活動正常</div>
      <div class="dx-hint">👆 你給幾分？</div>
    </div>
    <div class="dx-flip-back">
      <b>給分：0</b><br>無凝視偏移
    </div>
  </label>
</div>

<div class="dx-flip-card">
  <input type="checkbox" id="ns-card-5">
  <label for="ns-card-5" class="dx-flip-inner">
    <div class="dx-flip-front">
      <div class="dx-rank">3. 視野</div>
      <div class="dx-name">粗略測試無缺損</div>
      <div class="dx-hint">👆 你給幾分？</div>
    </div>
    <div class="dx-flip-back">
      <b>給分：0</b><br>未發現偏盲或視野缺損
    </div>
  </label>
</div>

<div class="dx-flip-card">
  <input type="checkbox" id="ns-card-6">
  <label for="ns-card-6" class="dx-flip-inner">
    <div class="dx-flip-front">
      <div class="dx-rank">4. 顏面麻痺</div>
      <div class="dx-name">右側鼻唇溝變淺<br>口角下垂但可閉眼</div>
      <div class="dx-hint">👆 你給幾分？</div>
    </div>
    <div class="dx-flip-back">
      <b>給分：1</b><br>屬於輕度（minor）顏面無力
    </div>
  </label>
</div>

<div class="dx-flip-card">
  <input type="checkbox" id="ns-card-7">
  <label for="ns-card-7" class="dx-flip-inner">
    <div class="dx-flip-front">
      <div class="dx-rank">5a. 右上肢</div>
      <div class="dx-name">10秒內下垂<br>未完全落床</div>
      <div class="dx-hint">👆 你給幾分？</div>
    </div>
    <div class="dx-flip-back">
      <b>給分：2</b><br>有 drift 但尚未完全落床，屬中度無力
    </div>
  </label>
</div>

<div class="dx-flip-card">
  <input type="checkbox" id="ns-card-8">
  <label for="ns-card-8" class="dx-flip-inner">
    <div class="dx-flip-front">
      <div class="dx-rank">5b. 左上肢</div>
      <div class="dx-name">正常維持90度10秒</div>
      <div class="dx-hint">👆 你給幾分？</div>
    </div>
    <div class="dx-flip-back">
      <b>給分：0</b><br>無下垂，力量正常
    </div>
  </label>
</div>

<div class="dx-flip-card">
  <input type="checkbox" id="ns-card-9">
  <label for="ns-card-9" class="dx-flip-inner">
    <div class="dx-flip-front">
      <div class="dx-rank">6a. 右下肢</div>
      <div class="dx-name">力量稍弱<br>可抗阻力</div>
      <div class="dx-hint">👆 你給幾分？</div>
    </div>
    <div class="dx-flip-back">
      <b>給分：1</b><br>輕微力量下降，仍可對抗阻力
    </div>
  </label>
</div>

<div class="dx-flip-card">
  <input type="checkbox" id="ns-card-10">
  <label for="ns-card-10" class="dx-flip-inner">
    <div class="dx-flip-front">
      <div class="dx-rank">6b. 左下肢</div>
      <div class="dx-name">正常</div>
      <div class="dx-hint">👆 你給幾分？</div>
    </div>
    <div class="dx-flip-back">
      <b>給分：0</b><br>力量正常
    </div>
  </label>
</div>

<div class="dx-flip-card">
  <input type="checkbox" id="ns-card-11">
  <label for="ns-card-11" class="dx-flip-inner">
    <div class="dx-flip-front">
      <div class="dx-rank">7. 肢體共濟失調</div>
      <div class="dx-name">因無力無法可靠評估</div>
      <div class="dx-hint">👆 你給幾分？</div>
    </div>
    <div class="dx-flip-back">
      <b>給分：0</b><br>因無力而無法評估時計 0 分，並非共濟失調本身的問題
    </div>
  </label>
</div>

<div class="dx-flip-card">
  <input type="checkbox" id="ns-card-12">
  <label for="ns-card-12" class="dx-flip-inner">
    <div class="dx-flip-front">
      <div class="dx-rank">8. 感覺</div>
      <div class="dx-name">針刺反應正常對稱</div>
      <div class="dx-hint">👆 你給幾分？</div>
    </div>
    <div class="dx-flip-back">
      <b>給分：0</b><br>雙側對稱，無感覺缺損
    </div>
  </label>
</div>

<div class="dx-flip-card">
  <input type="checkbox" id="ns-card-13">
  <label for="ns-card-13" class="dx-flip-inner">
    <div class="dx-flip-front">
      <div class="dx-rank">9. 語言</div>
      <div class="dx-name">找詞困難、不流暢<br>理解力保留</div>
      <div class="dx-hint">👆 你給幾分？</div>
    </div>
    <div class="dx-flip-back">
      <b>給分：1</b><br>輕度~中度失語（mild-moderate aphasia）
    </div>
  </label>
</div>

<div class="dx-flip-card">
  <input type="checkbox" id="ns-card-14">
  <label for="ns-card-14" class="dx-flip-inner">
    <div class="dx-flip-front">
      <div class="dx-rank">10. 構音障礙</div>
      <div class="dx-name">說話明顯含糊<br>仍可被理解</div>
      <div class="dx-hint">👆 你給幾分？</div>
    </div>
    <div class="dx-flip-back">
      <b>給分：1</b><br>明顯但可理解，屬中等程度構音障礙
    </div>
  </label>
</div>

<div class="dx-flip-card">
  <input type="checkbox" id="ns-card-15">
  <label for="ns-card-15" class="dx-flip-inner">
    <div class="dx-flip-front">
      <div class="dx-rank">11. 忽略症</div>
      <div class="dx-name">雙側同時刺激無忽略</div>
      <div class="dx-hint">👆 你給幾分？</div>
    </div>
    <div class="dx-flip-back">
      <b>給分：0</b><br>無 extinction/inattention 現象
    </div>
  </label>
</div>

</div>

**總分 = 1+1+2+1+1+1 = 約 7 分**（屬於輕度至中度中風，mild-moderate stroke）

> 📌 教學提醒：NIHSS 評分常見爭議點在於 **1b（LOC questions）與失語症的交互影響**——若患者因構音障礙導致答案聽不清楚但內容正確，通常給 1 分而非 2 分；需與失語症（9 分項目）區分評估，避免重複扣分邏輯混淆。

---

## 2️⃣ 血管供應區域定位 (Vascular Territory Localization)

<details>
<summary>點擊展開定位推論</summary>

**關鍵徵候組合**：
- 右側顏面 + 右上肢無力為主（leg 較輕）
- 構音障礙 + 找詞困難（語言障礙，但理解力保留）
- **無**視野缺損、**無**忽略症（neglect）、**無**凝視偏移

**推論**：
- 此型態（面部+上肢 > 下肢的無力分布）符合 **左側大腦中動脈 (Left Middle Cerebral Artery, MCA)** 供應區域中的 **上分支 (superior division)** 受損
- 語言障礙（找詞困難但理解保留）較符合 **表達性/運動性失語 (Broca-type aphasia)** 的部分表現，支持左側額葉下部（優勢側語言區）受累
- **無**忽略症與**無**視野缺損，使較大範圍的左側 MCA 主幹或合併下分支病灶可能性降低（但不能完全排除，仍須影像確認）
- 心律不整觸診不規則 → 高度懷疑潛在 **心房顫動 (Atrial Fibrillation)**，提示可能病因為**心源性栓塞 (cardioembolic stroke)**

> 📌 臨床珍珠：右利手患者中，語言中樞絕大多數位於**左側**，因此「右側肢體無力 + 語言障礙」幾乎可直接定位於**左側大腦半球**病灶，這是臨床上快速定位的重要捷徑。

</details>

---

## 3️⃣ 鑑別診斷 (Top 3 Differential Diagnosis)

> 💡 點擊下方卡片翻面查看支持點與需排除點。建議先自己猜猜看排序，再翻開核對。

<div class="dx-flip-grid">

<div class="dx-flip-card">
  <input type="checkbox" id="dx-card-1">
  <label for="dx-card-1" class="dx-flip-inner">
    <div class="dx-flip-front">
      <div class="dx-rank">排序 1</div>
      <div class="dx-name">急性缺血性腦中風<br>(Acute Ischemic Stroke)<br>左側 MCA 供應區</div>
      <div class="dx-hint">👆 點擊翻面看理由</div>
    </div>
    <div class="dx-flip-back">
      <b>✅ 支持點：</b>急性局部神經學缺損、時間軸明確、心律不整提示心源性栓塞風險<br><br>
      <b>⚠️ 需排除：</b>須影像排除出血才能確立此診斷並啟動治療
    </div>
  </label>
</div>

<div class="dx-flip-card">
  <input type="checkbox" id="dx-card-2">
  <label for="dx-card-2" class="dx-flip-inner">
    <div class="dx-flip-front">
      <div class="dx-rank">排序 2</div>
      <div class="dx-name">腦出血<br>(Intracerebral Hemorrhage)</div>
      <div class="dx-hint">👆 點擊翻面看理由</div>
    </div>
    <div class="dx-flip-back">
      <b>✅ 支持點：</b>急性局部神經學症狀亦可見於出血，且患者血壓偏高<br><br>
      <b>⚠️ 需排除：</b>須以 <b>非顯影電腦斷層 (Non-contrast CT Brain)</b> 立即排除——這是治療決策（是否給予 rt-PA）的關鍵性第一步
    </div>
  </label>
</div>

<div class="dx-flip-card">
  <input type="checkbox" id="dx-card-3">
  <label for="dx-card-3" class="dx-flip-inner">
    <div class="dx-flip-front">
      <div class="dx-rank">排序 3</div>
      <div class="dx-name">Stroke Mimics<br>低血糖 / Todd's paralysis /<br>偏頭痛先兆</div>
      <div class="dx-hint">👆 點擊翻面看理由</div>
    </div>
    <div class="dx-flip-back">
      <b>✅ 支持點：</b>此類為常見的 stroke mimics，須以病史與血糖值排除<br><br>
      <b>⚠️ 已排除：</b>本案血糖 142 mg/dL，已可初步排除低血糖；無癲癇病史、無頭痛病史
    </div>
  </label>
</div>

</div>

> 📌 教學提醒：臨床上常見陷阱是**過早鎖定「中風」診斷**而忽略 stroke mimics（如低血糖、癲癇後狀態、複雜性偏頭痛、轉換症等），務必先用基本檢驗（血糖）與影像排除立即危險的鑑別診斷。

---

## 4️⃣ 影像學與檢驗安排

<details>
<summary>點擊展開建議檢查項目</summary>

**立即（Door-to-imaging 目標 <25 分鐘）：**
- **非顯影腦部電腦斷層 (Non-contrast CT Brain)** — 首要排除出血，是否給予 rt-PA 的關鍵依據
- 視機構能力可同時安排 **CT Angiography (CTA)** 評估大血管阻塞（是否符合機械取栓條件）

**抽血（不應延遲 CT 與 rt-PA 評估）：**
- 隨機/指尖血糖（已測得 142 mg/dL，正常範圍）
- 全血球計數 (CBC)、凝血功能 (PT/INR, aPTT) — 評估是否有凝血異常或抗凝血劑使用史
- 腎功能、電解質
- 心電圖 (12-lead ECG) — 評估心房顫動

> 📌 重要原則：**等待凝血功能報告不應延誤 rt-PA 給藥**，除非患者有抗凝血劑使用史或出血傾向之臨床懷疑（依 AHA/ASA 指引）。

</details>

---

## 5️⃣ 治療決策 (Management Decision)

<details>
<summary>點擊展開治療邏輯</summary>

**時間窗判斷**：
- Last known well = **07:30**
- 抵達急診 = **10:10**
- 距離 LKW 已 **2 小時 40 分**，仍在 **rt-PA 4.5 小時治療時間窗內**

**若 CT 排除出血、無其他禁忌症：**
- 考慮 **靜脈注射血栓溶解劑 (IV Alteplase / rt-PA)**
  - 劑量：**0.9 mg/kg**（最大總劑量 90mg），其中 10% 於 1 分鐘內靜脈推注，剩餘 90% 於 60 分鐘輸注
  - 給藥前須確認：血壓 <185/110 mmHg（若過高需先降壓）、無近期手術/出血史、INR/aPTT 正常或未使用抗凝血劑

**若 CTA 顯示大血管阻塞（如左側 MCA M1 段）：**
- 評估是否符合 **機械取栓 (Mechanical Thrombectomy)** 條件（依 AHA/ASA 指引，部分病人時間窗可延長至 24 小時，需配合灌注影像評估）

**心房顫動處置（次要但重要）**：
- 急性期**不立即**啟動口服抗凝血劑（需待出血風險穩定、評估出血轉化風險後，通常急性中風後數天至數週才考慮啟動，依梗塞嚴重度分層）
- 此為**未定論之臨床議題**：抗凝起始時機目前各指引建議略有差異，需依個案梗塞範圍與出血風險評估

> ⚠️ **目前醫學實證有限/具爭議處**：心房顫動相關中風之抗凝起始確切時間點，仍依各家機構與最新研究（如 ELAN trial）持續調整，建議查閱最新指引。

</details>

---

## 6️⃣ 專家回顧 (Expert Debriefing)

### ✅ Take-home Messages
1. **時間軸是急性中風處置的核心**：Last known well 而非「被發現異常的時間」才是治療時間窗計算的起點
2. **面臂腿無力分布** + **語言障礙**的組合，可快速定位至優勢側（通常為左側）大腦中動脈供應區
3. **NIHSS 不只是評分工具**，更是治療決策（rt-PA 適應症、取栓評估）與預後溝通的共同語言
4. **CT 排除出血永遠優先於一切治療決策**，這是急性中風流程中不可省略的步驟
5. Stroke mimics（低血糖、Todd's paralysis、偏頭痛先兆）需在診斷流程中主動排除，避免誤判

### ⚠️ 常見臨床陷阱 (Pitfalls)
- 將「家屬發現異常的時間」誤當作症狀發生時間，導致時間窗誤判
- 因患者構音障礙而誤判為意識不清或不合作，影響 NIHSS 評分準確性
- 忽略心律不整的觸診/聽診線索，延誤對心房顫動相關心源性栓塞的懷疑
- 過度聚焦於「是否符合 rt-PA」而忽略同時評估是否符合機械取栓條件（兩者並非互斥）

---

## 📚 延伸閱讀建議方向
- AHA/ASA Guidelines for the Early Management of Patients With Acute Ischemic Stroke（建議查閱最新版本）
- NIHSS 標準化教學影片（用於評分一致性訓練）
- ELAN trial（心房顫動相關中風後抗凝起始時機之隨機對照試驗）

> 本檔案內容依公開臨床指引原則整理，旨在教學演練使用。實際臨床決策應以當下最新版官方指引與個別病人情況為準。
