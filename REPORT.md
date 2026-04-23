# Day 16 Submission — Team 4

## Members
- Xói (Nguyễn Bình Thành) - 2A202600138 — Product Manager (Team Lead)
- Phạm Hoàng Kim Liên - 2A202600260 — User Researcher
- Lê Đức Thanh - 2A202600093 — System Architect / AI Engineer
- Lê Nguyễn Thanh Bình - 2A202600447 — Go-to-Market Strategist
- Huy Hoàng - 2A202600486 — Data & Moat Analyst

---
## 1. Idea reframed
Original idea:
> Cung cấp các AI chatbot chuyên biệt theo môn học cho sinh viên Y khoa, giúp giải đáp thắc mắc và tóm tắt kiến thức một cách tự động.

Reframed as a product opportunity:
> Sinh viên Y khoa gặp khó khăn trong việc hệ thống hóa khối lượng kiến thức chuyên ngành khổng lồ từ nhiều nguồn tài liệu rời rạc, dẫn đến lãng phí thời gian và giảm hiệu quả ôn luyện. AI có khả năng hiểu và xử lý ngữ cảnh chuyên môn sâu, tạo điều kiện cho việc tự động chuyển đổi tài liệu cá nhân lộn xộn thành bài học có cấu trúc chuẩn và tóm tắt thông tin tức thì—điều mà các công cụ Note-taking hay Search hiện tại không thể làm trọn vẹn.

---
## 2. Customer / Segment Card
- **Segment name:** Sinh viên Y khoa (Tập trung vào nhóm năm 1-4 đang học khối kiến thức cơ sở và thi chuyển giai đoạn).
- **Operational context:** Phải nạp và tiêu hóa một khối lượng kiến thức lâm sàng / cận lâm sàng khổng lồ trong thời gian cực kỳ giới hạn.
- **Recurring workflow:** Ghi chép tay (handnote) thủ công, chụp slide mờ, gõ máy rời rạc; hoàn toàn thiếu một hệ thống tự động để cấu trúc lại các mảnh thông tin phân tán này thành một lộ trình bài học có tính hệ thống.
- **Pain moment:** Giai đoạn "nước rút" sát lịch thi. Áp lực chồng chéo từ nhiều môn học tạo ra cảm giác hoảng loạn (panic), mất kiểm soát tiến độ.
- **Why now:** Sự trưởng thành của Agentic AI trong việc đọc hiểu ngữ cảnh sâu (Deep Contextual Understanding) giúp máy móc lần đầu tiên có thể làm nhiệm vụ "nhặt rác và xếp vào đúng ngăn kéo chuyên môn" thay cho con người.
- **Access path:** Các cộng đồng sinh viên Y khoa (Group Facebook trường, các Drive chia sẻ tài liệu tiền mùa thi, các nhóm chat Zalo nội bộ khóa).

One-sentence description:
> Sinh viên Y khoa cần công cụ AI giúp tự động hệ thống hóa kiến thức chuyên môn từ mớ tài liệu rời rạc để lấy lại quyền kiểm soát lộ trình ôn thi áp lực cao.

---
## 3. Need Map (2 needs)

### Need #1: Tự động hóa cấu trúc lộ trình học tập
- **Statement:** Sinh viên Y khoa cần một cách để nhìn thấy ngay lập tức bức tranh tổng thể và logic của môn học từ mớ tài liệu hỗn độn, để họ có thể bắt tay vào học ngay thay vì tốn hàng giờ sắp xếp thủ công.
- **Current workaround:** Người học dành hàng giờ để đọc lại sổ tay, sau đó tự gõ lại nội dung vào máy tính hoặc vẽ sơ đồ tư duy (mindmap) bằng tay một cách cảm tính.
- **Pain signal:** Cảm giác quá tải và mất phương hướng khi khối lượng kiến thức chuyên ngành quá lớn nhưng tài liệu lại nằm rải rác ở nhiều nguồn khác nhau.
- **Evidence / proxy evidence:** Sự xuất hiện dày đặc của các folder Google Drive chứa hàng chục file PDF, ảnh chụp vở ghi, và mindmap chằng chịt được sinh viên chia sẻ (share/request access) liên tục trên các group Facebook khóa/trường trong vòng 1 tháng trước kỳ thi.
- **Why underserved:** Các ứng dụng ghi chú phổ biến chỉ đóng vai trò lưu trữ tĩnh (storage) chứ chưa có khả năng đọc hiểu (understanding) thuật ngữ chuyên môn để tự sắp xếp kiến thức thành bài học hoàn chỉnh.

### Need #2: Định lượng và theo dõi tiến độ ôn tập
- **Statement:** Người học cần một hệ thống có khả năng đánh giá xem họ đã cover được bao nhiêu phần trăm chương trình để giải tỏa áp lực hoang mang trước kỳ thi.
- **Current workaround:** Sinh viên lật từng trang ghi chú hoặc dùng bút dạ highlight mục lục giáo trình để ước lượng thô sơ xem mình còn bao nhiêu bài chưa học.
- **Pain signal:** Sự hoảng loạn (panic) khi không biết mình đang ở đâu trong ma trận kiến thức, dẫn đến học vẹt hoặc bỏ sót phần trọng tâm.
- **Evidence / proxy evidence:** Các bài post ẩn danh (confession) than thở về sự bất lực, "học trước quên sau", hoặc xin "tài liệu tóm tắt cấp tốc" bùng nổ trên các diễn đàn trường Y mỗi kỳ thi.
- **Why underserved:** Các AI Note-taking (như NotebookLM) rất giỏi tóm tắt tài liệu lẻ, nhưng chúng bị "mù" về mặt bối cảnh chuyên môn (Domain Ignorance). Chúng không có sẵn bộ khung giáo trình chuẩn để đối chiếu, nên không thể tạo ra một thanh tiến độ học tập.

---
## 4. Strategy Statement
For **[sinh viên Y khoa đang đối mặt với kỳ thi có khối lượng kiến thức khổng lồ]**,
who struggle with **[sự hoang mang và mất kiểm soát khi không biết mình đã hoàn thành bao nhiêu phần trăm chương trình ôn luyện]**,
our product helps them **[chuyển hóa kho tài liệu cá nhân rời rạc thành các khóa học có lộ trình bài bản và thanh tiến độ trực quan]**
through **[kiến trúc AI Agent tự động đối chiếu và ánh xạ (map) ghi chú cá nhân vào khung giáo trình y khoa chuẩn đã được pre-cache]**,
unlike **[các công cụ AI note-taking chung chung chỉ có khả năng tóm tắt tài liệu lẻ tẻ]**,
because we can leverage **[bánh đà dữ liệu chuyên môn giúp định lượng hóa quá trình học tập một cách chính xác tuyệt đối.]**

---
## 5. Moat Hypothesis
**Moat mechanism:** Data Compounding & Domain-Specific Mapping Flywheel (Bánh đà dữ liệu & Ánh xạ chuyên môn).

If we deploy 50 times in the same vertical (ví dụ: xử lý tài liệu cho 50 khóa sinh viên Y tại các trường khác nhau), the following improve:
1. Độ chính xác khi AI Agent nhận diện và phân loại các ghi chú "nháp", viết tắt tiếng lóng (ví dụ: HF = suy tim), hoặc slide lộn xộn của sinh viên vào đúng ngăn kéo (Medical Ontology) đạt mức gần tuyệt đối.
2. Kho dữ liệu tĩnh (Cold Cache) tự động mở rộng bao phủ được các format tài liệu đặc thù của từng trường Đại học (Y Hà Nội vs. Y Dược TP.HCM).
3. Thời gian xử lý (Latency) để tạo ra lộ trình học tập giảm xuống gần bằng 0, vì hệ thống đã "nhẵn mặt" với hầu hết các pattern tài liệu cá nhân.

**Why competitors cannot easily replicate this:** > Các công cụ AI Note-taking (như NotebookLM, Notion) thiếu lớp Database y khoa tĩnh (Medical Ontology), trong khi các thư viện Y khoa khổng lồ (như AMBOSS) lại đóng kín và thiếu Engine linh hoạt để nhai nuốt dữ liệu rác cá nhân của người dùng. Để bắt chước, đối thủ phải xây lại cả hai hệ thống này và luồng agentic workflow kết nối chúng.

---
## 6. Initial TAM / SAM / SOM view
| Layer | Estimate | Key assumptions | Confidence |
|---|---|---|---|
| TAM | ~100 tỷ VNĐ/năm ($4M) | 100.000 SV Y khoa (toàn VN) x Giá giả định 1.000.000 VNĐ/user/năm | High |
| SAM | ~40 tỷ VNĐ/năm ($1.6M) | 40% của TAM (Tập trung nhóm SV dùng thiết bị thông minh, sẵn sàng chi trả ở các TP lớn) | Med |
| SOM | 2 - 4 tỷ VNĐ/năm ($80K-$160K) | Mức thâm nhập 5-10% của SAM trong 12-24 tháng đầu thông qua Viral Loop chia sẻ tài liệu mùa thi | Med |

**Top 3 unknowns requiring further research:**
1. **Unit Economics:** Chi phí API cho LLM/Vector DB trên mỗi user có làm biên lợi nhuận (margin) bị âm so với mức giá 1.000.000 VNĐ/năm hay không?
2. **Willingness to Pay (WTP):** Văn hóa sinh viên VN quen dùng "Drive Share" miễn phí. Tỷ lệ chuyển đổi (Conversion Rate) từ việc bấm link xem ké sang tài khoản trả phí là bao nhiêu?
3. **Zero-Tolerance for Hallucination:** Làm sao để kiểm soát và định lượng rủi ro AI map sai kiến thức lâm sàng trong giai đoạn MVP?

**Judgment:**
- [x] Worth pursuing now (Làm bàn đạp Testbed ở VN để tối ưu hệ thống, sau đó scale ra các chứng chỉ quốc tế như USMLE để mở rộng TAM).
- [ ] Worth pursuing but not now (need to validate [...] first)
- [ ] Not worth pursuing as currently framed

---
## 7. Positioning Note (2 sentences)
**What we are:**
> Course4ALL là một Lớp màng lọc điều phối (Orchestration Layer) sử dụng AI Agent để tự động ráp nối tài liệu cá nhân hỗn loạn của sinh viên Y khoa vào một lộ trình ôn thi chuẩn xác.

**What we are not / not yet:**
> Chúng tôi không phải là một nhà xuất bản tạo sẵn thư viện nội dung học thuật tĩnh, và tuyệt đối không phải là một công cụ AI tạo chữ chung chung có nguy cơ sinh ra kiến thức sai lệch.

---
## 8. Self-assessment before Day 17
Trong 6 mắt xích (Idea - Customer - Need - Strategy - Moat - Market Size)
> Mắt xích cứng cáp nhất hiện tại là **Customer & Need** (pain point cực kỳ sắc nét và có tính khẩn cấp cao) và **Moat** (kiến trúc Hybrid rất khó bị copy bởi Big Tech). Mắt xích yếu nhất cần rà soát là **Market Size**, vì TAM thị trường VN khá nhỏ, đòi hỏi phải chứng minh được tiềm năng scale up ra global (như các kỳ thi USMLE) trong tương lai.

Open questions chúng tôi muốn khám phá thêm ở Day 17:
1. Cơ chế Growth/Viral Loop cụ thể nào để biến 1 sinh viên dùng thử thành 10 sinh viên mua gói trả phí trong cùng một lớp học?
2. Bài toán cân bằng giữa chi phí (Token cost) và Trải nghiệm người dùng (Latency) ở góc độ System Design cho bản MVP?
3. Các metric (chỉ số) quan trọng nhất để đánh giá Product-Market Fit cho sản phẩm này trong 3 tháng đầu ra mắt là gì?
