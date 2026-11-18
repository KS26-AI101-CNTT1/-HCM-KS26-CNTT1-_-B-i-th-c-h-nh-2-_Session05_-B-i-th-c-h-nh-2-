Đề bài / Yêu cầu

Xây dựng chuỗi Prompt viết bài PR sản phẩm công nghệ

1. Mục tiêu

Thành thạo kỹ thuật Prompt Chaining để giải quyết tác vụ phức tạp đòi hỏi nhiều công đoạn.

Biết cách thiết lập và truyền ngữ cảnh (Context) liên tiếp giữa các prompt thành phần.

Nắm vững kỹ năng xử lý đứt gãy ngữ cảnh và duy trì tính nhất quán khi viết bài dài.

2. Bối cảnh bài toán

Phòng Marketing cần sản xuất một bài PR chuyên sâu (khoảng 1000 - 1500 từ) giới thiệu giải pháp AI Chatbot mới cho doanh nghiệp. Việc sử dụng một prompt đơn lẻ để AI viết toàn bộ bài thường dẫn đến nội dung hời hợt, lặp ý và thiếu chiều sâu.

Bạn cần xây dựng một chuỗi prompt (Prompt Chain) gồm 3 bước để tạo ra bài viết chất lượng cao.

3. Yêu cầu

Thiết lập quy trình Prompt Chaining gồm 3 bước rõ ràng:

Prompt 1: Nghiên cứu đối tượng khách hàng mục tiêu và xây dựng danh sách các nỗi đau (pain points) mà sản phẩm giải quyết.

Prompt 2: Dựa trên output của Prompt 1, thiết lập dàn ý chi tiết (Outline) cho bài viết PR.

Prompt 3: Dựa trên dàn ý ở Prompt 2, triển khai viết chi tiết từng phần của bài viết và tối ưu hóa từ khóa SEO.

4. Quy tắc xử lý

Thiết kế các prompt thành phần sao cho kết quả của prompt trước là đầu vào bắt buộc của prompt sau.

Quy định rõ cấu trúc dữ liệu truyền giữa các bước để đảm bảo tính nhất quán.

Thiết lập quy tắc xử lý khi AI viết bài dài bị ngắt quãng giữa chừng (đạt max token): cung cấp câu lệnh điều khiển tiếp tục tạo chính xác.

5. Yêu cầu xử lý dữ liệu

Bài viết PR đầu ra cuối cùng cần đạt cấu trúc chuẩn SEO bao gồm:

Tiêu đề thu hút (Headline).

Đoạn mở đầu (Lead) hấp dẫn giải quyết pain points.

Các tiệu đề con (H2, H3) tương ứng với dàn ý.

Lời kêu gọi hành động (CTA) rõ ràng ở cuối bài.

Kiến trúc luồng dữ liệu (Data Flow)

Để đảm bảo tính nhất quán và tránh mất ngữ cảnh, dữ liệu giữa các bước sẽ được đóng gói theo cấu trúc định sẵn:

Đầu ra Prompt 1 ([OUTPUT_1]): Bảng phân tích Chân dung khách hàng & Pain Points.

Đầu ra Prompt 2 ([OUTPUT_2]): Dàn ý chi tiết (H1, H2, H3) kèm phân bổ từ khóa SEO và định hướng giọng điệu.

Đầu ra Prompt 3 ([OUTPUT_3]): Nội dung bài PR hoàn chỉnh (1000 – 1500 từ) được viết cuốn chiếu từng phần.

Prompt 1: Nghiên cứu đối tượng & Khai thác nỗi đau (Pain Points)

Mục tiêu: Xác định đúng tệp khách hàng B2B và các vấn đề cốt lõi để làm chất liệu cho bài PR. [1]

text

Bạn là một Chuyên gia Nghiên cứu Thị trường và Chiến lược Nội dung B2B. 

Nhiệm vụ của bạn là phân tích khách hàng mục tiêu cho một bài viết PR giới thiệu giải pháp "AI Chatbot thế hệ mới dành cho doanh nghiệp" (tự động hóa chăm sóc khách hàng, chốt đơn và tích hợp CRM).

Hãy xuất kết quả theo đúng cấu trúc dữ liệu dưới đây để làm đầu vào cho bước lập dàn ý:

1. CHÂN DUNG KHÁCH HÀNG MỤC TIÊU (TARGET AUDIENCE):

- Nhóm đối tượng chính (Chức danh, quy mô doanh nghiệp):

- Mục tiêu kinh doanh hàng đầu của họ:

2. DANH SÁCH 4 NỖI ĐAU CỐT LÕI (PAIN POINTS) & GIẢI PHÁP:

Với mỗi nỗi đau, hãy trình bày theo mẫu:

- Nỗi đau [Số thứ tự]: [Tên nỗi đau cụ thể trong vận hành/CSKH]

- Hệ quả thực tế: [Tác động tiêu cực đến doanh thu hoặc chi phí]

- Góc độ giải quyết của AI Chatbot: [Tính năng cụ thể khắc phục nỗi đau này]

3. BỘ TỪ KHÓA SEO MỤC TIÊU:

- Từ khóa chính (1 từ):

- Từ khóa phụ (3-4 từ):

Yêu cầu: Trình bày ngắn gọn, súc tích, tập trung vào số liệu và hiệu quả kinh doanh thực tế. Không viết bài PR ở bước này.

Prompt 2: Thiết lập dàn ý bài PR chuẩn SEO (Outline)

Mục tiêu: Kế thừa toàn bộ dữ liệu từ Bước 1 để dựng khung xương bài viết dài 1000 - 1500 từ, khóa chặt cấu trúc và giọng điệu.

text

Bạn là một Biên tập viên Nội dung PR Công nghệ (Tech PR Editor).

Dựa trên dữ liệu nghiên cứu khách hàng dưới đây:

<INPUT_DATA>

[Dán toàn bộ kết quả đầu ra từ Prompt 1 vào đây]

</INPUT_DATA>

Hãy lập một dàn ý chi tiết (Outline) cho bài viết PR dài khoảng 1000 - 1500 từ. Dàn ý phải bám sát các Pain Points ở trên và tuân thủ nghiêm ngặt cấu trúc sau:

1. THIẾT LẬP TIÊU CHUẨN BÀI VIẾT:

- Giọng điệu (Tone of voice): Chuyên nghiệp, khách quan, tin cậy, mang tính tư vấn giải pháp (không quảng cáo phô trương).

- Mật độ từ khóa: Phân bổ tự nhiên từ khóa chính và phụ từ <INPUT_DATA>.

2. CẤU TRÚC DÀN Ý CHI TIẾT:

- Tiêu đề chính (H1): Đề xuất 2 phương án tiêu đề thu hút, đánh trúng nỗi đau lớn nhất.

- Đoạn mở đầu (Lead - khoảng 150 từ): Nêu bối cảnh thị trường, chạm vào Pain Point và hé lộ giải pháp.

- Phần 1 (H2): [Tiêu đề H2 phản ánh thực trạng/nỗi đau] -> Kèm 2-3 ý triển khai (H3) và số liệu/ví dụ cần có.

- Phần 2 (H2): [Tiêu đề H2 giới thiệu giải pháp AI Chatbot] -> Kèm 2-3 ý triển khai (H3) về tính năng nổi bật.

- Phần 3 (H2): [Tiêu đề H2 chứng minh hiệu quả/ROI cho doanh nghiệp] -> Kèm các ý về tối ưu chi phí, tăng tỷ lệ chuyển đổi.

- Kết bài & Kêu gọi hành động (CTA - khoảng 100 từ): Tóm tắt giá trị cốt lõi và điều hướng dùng thử/nhận tư vấn.

Yêu cầu: Ghi rõ mục tiêu số từ cho từng phần để tổng bài đạt 1000 - 1500 từ. Chỉ xuất ra dàn ý, chưa viết nội dung chi tiết.

Prompt 3: Triển khai viết bài chi tiết & Tối ưu SEO

Mục tiêu: Viết nội dung hoàn chỉnh dựa trên dàn ý Bước 2, giữ nguyên văn phong từ đầu đến cuối.

text

Bạn là một Chuyên gia Copywriter mảng Công nghệ B2B.

Hãy viết bài PR hoàn chỉnh (độ dài mục tiêu: 1000 - 1500 từ) dựa trên dàn ý chi tiết dưới đây:

<OUTLINE_DATA>

[Dán toàn bộ kết quả đầu ra từ Prompt 2 vào đây]

</OUTLINE_DATA>

Quy tắc thực thi bắt buộc:

1. Tuân thủ tuyệt đối cấu trúc H1, H2, H3, Lead và CTA đã duyệt trong <OUTLINE_DATA>.

2. Duy trì nhất quán giọng điệu: Chuyên nghiệp, sắc bén, đáng tin cậy xuyên suốt từ câu mở đầu đến câu kết thúc. Không dùng ngôn ngữ sáo rỗng, khoa trương.

3. Tối ưu hóa SEO: Chèn tự nhiên các từ khóa chính và từ khóa phụ vào H1, H2, đoạn Lead và rải đều trong thân bài. Bôi đậm các từ khóa hoặc luận điểm quan trọng để tăng tính dễ đọc (scannability).

4. Viết sâu sắc, có dẫn chứng logic cho từng luận điểm thay vì liệt kê hời hợt.

Hãy bắt đầu viết toàn bộ bài PR ngay bây giờ.

Cơ chế xử lý đứt gãy ngữ cảnh (Anti-Truncation Protocol)

Khi AI viết bài dài (trên 1000 từ) và bị dừng đột ngột giữa chừng do chạm giới hạn token đầu ra (max output tokens), bạn không được gõ các lệnh chung chung như "viết tiếp đi" (dễ làm AI viết lặp lại ý hoặc đổi giọng văn).

Hãy sử dụng Prompt điều khiển tiếp tục dưới đây:

text

Quá trình tạo văn bản vừa bị ngắt quãng do giới hạn độ dài. Hãy tiếp tục viết phần còn lại của bài PR dựa trên <OUTLINE_DATA> đã cung cấp.

Quy tắc nối tiếp bắt buộc:

1. Không lặp lại tiêu đề, không xin lỗi, không giải thích.

2. Nối tiếp trực tiếp và hoàn hảo từ câu cuối cùng bị ngắt sau đây:

"[Copy và dán 1-2 câu cuối cùng mà AI vừa viết trước khi bị dừng vào đây]"

3. Giữ nguyên văn phong chuyên nghiệp, tin cậy và tiếp tục hoàn thiện các thẻ H2,

6. Ràng buộc kỹ thuật

Không gộp chung quy trình vào 1 prompt duy nhất.

Không được thay đổi giọng điệu bài viết giữa các phần (giữ nguyên tone chuyên nghiệp, tin cậy).

Đoạn văn viết tiếp sau khi bị đứt gãy phải nối khớp hoàn hảo với câu trước đó.
