### 日期:3/17
### 題目:The Development and Applications of BioImpedance Technology
### 演講者:Kuo-Sheng Cheng, Ph.D.
![](https://github.com/yeh119/Seminar-II/blob/main/image/20260317_133115.jpg)
今天在講 Bioimpedance（生物阻抗），主要是在用電的方法去量人體的生理狀態。老師一開始先講這個技術可以做什麼，像是可以量體積變化（例如血流）、做 impedance plethysmography、impedance cardiography、甚至肺部的 impedance pneumography，也可以用來分析身體組成（body composition）、組織分類、組織監測，甚至到細胞層級的量測。
![](https://github.com/yeh119/Seminar-II/blob/main/image/20260317_133926.jpg)
接著進到 bioimpedance 的方法，本質上就是在人體上加一個高頻小電流（大概 100 kHz），然後去量電壓變化來推阻抗。實驗配置是用電極貼在胸腔，會量到像 Z₀、ΔZ，還會搭配 ECG 跟心音（phonocardiogram）一起看，所以其實是多訊號同步分析。量測的訊號會包含 dZ/dt、ΔZ、ECG、心音、還有主動脈壓力跟血流，這些波形之間是有時間對應關係的。

老師有特別畫一張圖在講訊號，像 dZ/dt 的 peak（最大變化率）會對應到血液射出速度，然後可以抓出 LVET（left ventricle ejection time），也就是左心室射血時間，這在後面算 cardiac output 很重要。

然後進到數學模型，本質其實就是從歐姆定律來的，R = ρL/A，阻抗 Z 也是類似概念。人體可以當作一個導體，血流改變會讓截面積 A 改變 → 阻抗改變 ΔZ。最後可以推到 stroke volume（SV）跟 dZ/dt 的最大值有關，公式大概是
SV ≈ (ρb × L² / Z₀²) × LVET × (dZ/dt)_max
所以其實就是用阻抗變化去間接估血液流量。
![](https://github.com/yeh119/Seminar-II/blob/main/image/20260317_133627.jpg)
接著講循環系統的部分，cardiac output（CO）就是
CO = SV × HR（心跳率）
傳統方法像是 Fick method 或 indicator dilution，但 bioimpedance 是非侵入式的方法，比較方便。

再來講呼吸相關的應用，像呼吸量測會用 spirometer、rotating vane、ultrasonic 或 differential pressure flow meter，流量基本上跟壓差 ΔP 成正比。呼吸的生理參數有 tidal volume（TV）、IRV、ERV、RV，還有 IC、FRC、VC、TLC 這些肺容量的概念，圖上有畫出整個肺容量的分布。
![](https://github.com/yeh119/Seminar-II/blob/main/image/20260317_133137.jpg)
最後回到最基本的觀念，就是歐姆定律，J = σE（電流密度跟電場），V = IR，這整個 bioimpedance 的核心就是「電流 → 電壓 → 阻抗 → 推回生理資訊」。

整體來說這堂課重點就是：用電的方式（阻抗變化）去量人體的血流、呼吸等生理參數，而且是非侵入式，未來也可以搭配影像（像 EIT）或甚至 deep learning 做更進一步分析。
