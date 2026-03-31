### 日期:3/31
### 題目:如何打造台版Edge Impulse TinyML 開發平台
### 演講者:許哲豪 教授
![](https://github.com/yeh119/Seminar-II/blob/main/image/63971_0.jpg)
這場演講主要是在介紹 Edge AI 與 TinyML 的整體概念，以及它們在實際應用中的技術架構與發展方向。一開始先從 AI 技術的演進談起，從早期的 CNN 用於影像辨識、RNN 處理時間序列資料，到後來的 Transformer 成為現代 AI 的核心架構，進一步發展出 LLM（大語言模型）、VLM（圖文模型）以及 VLA（結合感知與行動的模型）。可以看出 AI 正逐漸從單一任務，走向多模態與具備行動能力的系統，甚至發展出 AI Agent 與 Agentic AI 這種可以自主完成任務的型態。
![](https://github.com/yeh119/Seminar-II/blob/main/image/63973_0.jpg)
接著演講重點轉到 Edge AI 與生成式 AI 的差異。Edge AI 的核心概念是在裝置端直接完成 AI 推論，不需要依賴雲端，通常運行在 MCU、手機或 IoT 設備上，因此特別強調低功耗、低延遲與即時性。相對地，生成式 AI 則依賴雲端強大算力，模型規模龐大，適合進行內容生成與複雜推理。這兩者最大的差別在於資源使用與運算位置，一個是「小而即時」，另一個是「大而強大」。
![](https://github.com/yeh119/Seminar-II/blob/main/image/63967_0.jpg)
在應用層面上，演講也提到不同 AI 應用對算力的需求差異，從最基礎的智慧感測，到電腦視覺、自然語言處理，再到生成式 AI 與多模態 AI，所需的算力從 MOPS、GOPS 一直到 TOPS 等級不斷提升。這也說明為什麼 Edge AI 必須依賴模型壓縮與硬體加速，才能在有限資源下運作。
![](https://github.com/yeh119/Seminar-II/blob/main/image/63965_0.jpg)
在硬體架構部分，演講詳細說明了 AI 計算晶片的演進，從 CPU 到 GPU，再到 DSP、NPU、FPGA，最後到 ASIC。這個發展趨勢代表著運算從「通用」走向「專用」，也就是為了提升效率而犧牲彈性。其中 NPU 是專門為神經網路設計的加速器，在 Edge AI 中扮演非常重要的角色。此外，MCU 的架構也被分類為 CISC、RISC、RISC-V、DSP 與 NPU，而 Arm Cortex 系列中的 M 系列則是 TinyML 最常使用的核心。
![](https://github.com/yeh119/Seminar-II/blob/main/image/63959_0.jpg)
教授有解釋到在運算本質上，AI 的核心其實是矩陣運算（Y = AX + B），因此各種硬體加速方法都是圍繞著如何更快完成這類運算，例如提高 CPU 時脈、使用 SIMD 向量化指令、DSP 的乘加運算（MAC）、多核心並行處理，以及 GPU、NPU 等專用加速器。不過這些加速方式同時也會受到限制，包括算力、記憶體、能耗與資料傳輸等瓶頸。
![](https://github.com/yeh119/Seminar-II/blob/main/image/63960_0.jpg)
在軟體與工具方面，演講介紹了不同平台的 AI 開發工具。PC 端主要使用 TensorFlow 與 PyTorch，手機端則使用 TensorFlow Lite 或 PyTorch Mobile，而在 MCU 上則是 TensorFlow Lite for Microcontroller 以及 Edge Impulse。除此之外，各大晶片廠也提供自己的 TinyML 工具，例如 ST 的 CubeAI、NXP 的 eIQ、Renesas 的 Reality AI 等，這些工具的目的是讓模型能更容易部署到嵌入式設備上。
![](https://github.com/yeh119/Seminar-II/blob/main/image/63966_0.jpg)
接著演講也整理了完整的 Edge AI 開發流程，從資料收集開始，經過資料標註、模型建立、訓練與調整參數，再到模型優化（例如量化與壓縮），最後部署到裝置並進行測試。這個流程強調的是反覆迭代，而不是一次完成，尤其在 Edge AI 中，模型大小與效能之間需要不斷取捨。
![](https://github.com/yeh119/Seminar-II/blob/main/image/63970_0.jpg)
另外，演講也透過實際案例（像是龍蝦機器人 OpenClaw）說明同一個應用可以根據不同算力環境，設計成嵌入式版本、主機版本或高階運算版本，這也反映出 Edge AI 系統設計的彈性與層級化概念。
![](https://github.com/yeh119/Seminar-II/blob/main/image/63969_0.jpg)
最後，演講強調 Edge AI 並沒有一個固定的定義，不同公司會根據自身產品定位，將 Edge AI 定義為從穿戴式裝置、手機、單板電腦，到邊緣伺服器等不同層級。整體來說，Edge AI 的本質是在有限的硬體資源下，透過模型優化與硬體加速，讓 AI 能夠真正落地到實際設備中運作。
