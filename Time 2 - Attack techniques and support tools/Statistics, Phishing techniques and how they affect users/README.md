# Thống kê số liệu, các loại kỹ thuật Phishing và cách chúng tác động người dùng

<small>*Ngày cập nhật: 16 tháng 5, 2024 - 15:30*</small>

Chuyển đổi an ninh mạng đang diễn ra với tốc độ chóng mặt, cùng với đó các biện pháp phòng thủ kỹ thuật ngày càng tinh vi hơn ra đời mỗi ngày. Tuy nhiên, điều này cũng khiến chính `con người` – yếu tố dễ bị tấn công hơn – trở thành mục tiêu hấp dẫn đối với tin tặc. Lừa dối người dùng thường đơn giản và hiệu quả hơn nhiều so với việc vượt qua các hệ thống phòng thủ nhiều lớp. Nhận thức được điều này, tin tặc đang chuyển hướng sang các chiến thuật kỹ thuật xã hội tinh vi để vượt qua các lá chắn an ninh mạng cứng rắn, điển hình nhất là `Phishing`.

## Nội dung chính:
[I. Thống kê chi tiết](#thong-ke-chi-tiet)

[II. Phân tích tâm lý người dùng - Những yếu tố khiến người dùng dễ mắc lừa phishing](#phan-tich-tam-ly-nguoi-dung-nhung-yeu-to-khien-nguoi-dung-de-mac-lua)

[III. Kỹ thuật lừa đảo trong phishing - Mở rộng phạm vi](#ky-thuat-lua-dao-trong-phishing-mo-rong-pham-vi)
- [1. Kỹ thuật Spoofing](#ky-thuat-spoofing)
- [2. Kỹ thuật Social Engineering](#ky-thuat-social-engineering)
- [3. Kỹ thuật sử dụng hình ảnh và ngôn ngữ](#ky-thuat-su-dung-hinh-and-va-ngon-ngu)

<a name="thong-ke-chi-tiet"></a>
## Thống kê chi tiết:
Theo Báo cáo Chi phí Vi phạm Dữ liệu 2023 của [IBM](https://www.ibm.com/account/reg/us-en/signup?formid=urx-52258), các tổ chức phải đối mặt với mức chi phí trung bình hơn 4,5 triệu USD cho mỗi vụ vi phạm dữ liệu được thực hiện thông qua `Social engineering`. Đáng chú ý, `phishing` đã vượt qua đánh cắp thông tin đăng nhập trở thành phương thức tấn công phổ biến nhất trong năm 2022, cho thấy sự tinh vi ngày càng gia tăng của các thủ đoạn tấn công này.

Báo cáo cũng chỉ ra hậu quả nghiêm trọng của việc bị đánh cắp hoặc xâm phạm thông tin đăng nhập. Trung bình, các tổ chức mất đến 11 tháng (328 ngày) để xác định và ngăn chặn vi phạm dữ liệu, và 10 tháng (308 ngày) để giải quyết các trường hợp do nội gián gây ra.\
(Nguồn: IBM. ["Get insights to better manage the risk of a data breach"](https://www.ibm.com/account/reg/us-en/signup?formid=urx-52258))

Theo [Barracuda](https://assets.barracuda.com/assets/docs/dms/spear-phishing_report_vol6.pdf), một tổ chức uy tín về an ninh mạng, các cuộc tấn công `Spear Phishing` đang ngày càng gia tăng và trở thành mối đe dọa nghiêm trọng đối với các doanh nghiệp. Báo cáo của họ chỉ ra những con số đáng báo động sau:

- **Mục tiêu nhắm vào:**
    - **Lãnh đạo cấp cao:** Các CEO là đối tượng ưa thích của tin tặc với trung bình `57 cuộc tấn công` Spear Phishing mỗi năm. Lý do là họ thường nắm giữ thông tin nhạy cảm và có quyền truy cập vào tài chính của doanh nghiệp.
    - **Nhân viên CNTT:** Nắm giữ vai trò then chốt trong hệ thống an ninh mạng, nhân viên CNTT cũng là mục tiêu thường xuyên bị tấn công với trung bình `40 cuộc tấn công` mỗi năm.
- **Loại hình tấn công:** Tấn công Email Doanh nghiệp (BEC) là một trong mười phương thức tấn công `Social Engineering` phổ biến nhất. Tin tặc sử dụng email giả mạo để lừa đảo nhân viên chuyển tiền hoặc tiết lộ thông tin nhạy cảm.
- **Tần suất tấn công:** Một tổ chức điển hình phải đối mặt với `hơn 700 cuộc tấn công` lừa đảo qua mạng mỗi năm, cho thấy mức độ phổ biến và nguy hiểm của các mối đe dọa này.\
(Nguồn: Barracuda. ["Spear Phishing: Top Threats and Trends"](https://assets.barracuda.com/assets/docs/dms/spear-phishing_report_vol6.pdf), July 2021)

Nghiên cứu mới nhất của [Statista](https://www.statista.com/topics/8385/phishing/#topicOverview) về thực trạng tấn công lừa đảo trực tuyến đã vẽ nên một bức tranh ảm đạm về sự gia tăng đáng báo động của các mối đe dọa mạng này. Phân tích chuyên sâu dựa trên dữ liệu Statista cho thấy những điểm đáng chú ý sau:

1. **Mạng lưới lừa đảo khổng lồ:** Hơn `1,35 triệu` trang web lừa đảo độc đáo được phát hiện trên toàn cầu, tạo thành mối đe dọa nghiêm trọng cho người dùng internet ở mọi khu vực.

2. **Mục tiêu hàng đầu - Tổ chức tài chính:** Các tin tặc tinh vi nhắm mục tiêu vào các `tổ chức tài chính`, khai thác lòng tin và sơ hở bảo mật để đánh cắp thông tin nhạy cảm và tiền bạc của khách hàng, gây ra thiệt hại to lớn về tài chính và uy tín.

3. **Phần mềm và webmail trong tầm ngắm:** `18% các cuộc tấn công lừa đảo` trực tuyến nhắm vào `phần mềm` và `webmail` dựa trên web, khai thác lỗ hổng bảo mật để xâm nhập hệ thống và thu thập dữ liệu quan trọng.

4. **Smishing (SMS Phishing) - Mối đe dọa lan rộng:** `76% doanh nghiệp toàn cầu` phải đối mặt với nguy cơ bị tấn công Smishing, sử dụng tin nhắn SMS được giả mạo để đánh lừa người dùng cung cấp thông tin cá nhân hoặc nhấp vào liên kết độc hại.

5. **Thương hiệu chịu ảnh hưởng nặng nề:** Chỉ trong tháng 10 năm 2022, `599 thương hiệu` đã trở thành nạn nhân của các cuộc tấn công lừa đảo trực tuyến, gây tổn hại nghiêm trọng đến danh tiếng và niềm tin của khách hàng.

6. **Quốc gia bị tấn công bởi Phishing nhiều nhất:** `Việt Nam` có tỷ lệ người dùng Internet phải đối mặt với các cuộc tấn công Phishing lớn nhất.

7. **Kỹ thuật Social Engineering - Vũ khí lợi hại:** Kỹ thuật `Social Engineering chiếm 98%` tất cả các cuộc tấn công mạng, cho thấy sự tinh vi và nguy hiểm của phương thức tấn công này. Kỹ thuật này khai thác tâm lý và hành vi con người để lừa đảo người dùng cung cấp thông tin nhạy cảm hoặc thực hiện hành động mong muốn.

(Nguồn: Statista. ["Phishing - Statistics & Facts"](https://www.statista.com/topics/8385/phishing/#topicOverview))

Báo cáo `Điều tra Vi phạm Dữ liệu 2022 (DBIR)` do [Verizon](https://www.verizon.com/business/en-gb/resources/2022-data-breach-investigations-report-dbir.pdf) công bố gần đây đã tiếp tục vẽ nên bức tranh đáng báo động về vai trò chủ đạo của yếu tố con người trong các vụ tấn công mạng. Theo báo cáo, `con người là nguyên nhân trực tiếp dẫn đến 82%` các vụ vi phạm dữ liệu, cho thấy đây là mắt xích yếu nhất trong chuỗi an ninh mạng.

Mặc dù tỷ lệ nhân viên thực sự nhấp vào email lừa đảo vẫn tương đối thấp, chỉ ở `mức trung bình 2,9%` theo ghi nhận qua nhiều năm, con số này vẫn là mối đe dọa đáng kể đối với an ninh mạng của tổ chức. Kẻ tấn công chỉ cần nhắm mục tiêu vào một số ít cá nhân để thành công, và họ không ngừng tinh vi hóa các kỹ thuật lừa đảo để đánh lừa cả những người cảnh giác nhất.\
(Nguồn: Verizon. [DBIR - Data Breach Investigations Report](https://www.verizon.com/business/en-gb/resources/2022-data-breach-investigations-report-dbir.pdf), 2022)

<a name="phan-tich-tam-ly-nguoi-dung-nhung-yeu-to-khien-nguoi-dung-de-mac-lua"></a>
## Phân tích tâm lý người dùng - Những yếu tố khiến người dùng dễ mắc lừa phishing:
Như trong phần thống kê chúng ta có thể thấy được người dùng chính là nguyên nhân trực tiếp dẫn đến 82% các vụ vi phạm dữ liệu. Ngoài những yếu tố cơ bản như `thiếu kiến thức`, `tính tò mò` và `lòng tin` được nêu rõ ở [phần trước](https://github.com/vinh1312/Research-progress-report-Phishing/blob/master/Time%201%20-%20Concept%20of%20Phishing/README.md) thì một số yếu tố tâm lý khác cũng có thể khiến người dùng dễ mắc lừa phishing, bao gồm:

- **Áp lực thời gian:** Kẻ lừa đảo có thể tạo ra cảm giác cấp bách hoặc hối thúc người dùng hành động ngay lập tức để họ không có thời gian suy nghĩ kỹ lưỡng. Khi đứng trước việc không có sự lựa chọn mà cụ thể ở đây chính là không đủ thời gian để quyết định, con người thường có xu hướng "bỏ qua" để làm nhanh nhất có thể mà không nghĩ đến hậu quả. Ví dụ: Một người nhận được email thông báo tài khoản ngân hàng của họ bị khóa và yêu cầu họ phải truy cập vào trang web để "mở khóa" tài khoản trong vòng 24 giờ. Do cảm giác cấp bách, người dùng này có thể không suy nghĩ kỹ lưỡng và cung cấp thông tin cá nhân cho kẻ lừa đảo.

- **Thiếu sự nghi ngờ:** Một số người dùng có xu hướng tin tưởng vào những gì họ nhìn thấy và không đặt câu hỏi về tính xác thực của thông tin. Họ luôn cho rằng quyết định của mình là đúng đắng, đặt biệt là những người tin vào trực giác thay vì ý kiến khách quan và nó sẽ tệ hơn nếu họ nghĩ đây chỉ là vấn đề nhỏ không đáng để tâm thì mức cảnh giác sẽ gần như bằng 0. Điều này khiến họ dễ dàng bị đánh lừa bởi những email, tin nhắn hoặc trang web giả mạo được thiết kế tinh vi.

- **Mong muốn hòa nhập:** Kẻ lừa đảo có thể lợi dụng mong muốn hòa nhập và được chấp nhận của người dùng để thực hiện hành vi lừa đảo. Đây là mong muốn cơ bản của mỗi người, đặt biệt là nếu kẻ xấu biết được nạn nhân có xu hướng bị cô lập hoặc khó khăn trong việc giao tiếp, đây chính là điểm yếu nhất mà kẻ lừa đó có thể dễ dàng khai thác. Ví dụ: Một người nhận được email mời tham gia vào một nhóm độc quyền trên mạng xã hội. Do mong muốn được hòa nhập và kết bạn mới, người dùng này có thể cung cấp thông tin cá nhân cho kẻ lừa đảo.

<a name="ky-thuat-lua-dao-trong-phishing-mo-rong-pham-vi"></a>
## Kỹ thuật lừa đảo trong phishing - Mở rộng phạm vi:

Với việc hiện nay chúng ta có thể tìm kiếm thông tin về mọi thứ cần thiết ở trên mạng chỉ với một dòng tìm kiếm, đặc biệt khi có `sự trợ giúp của AI` làm cho việc này đơn giản hơn nhiều khi nó có thể thống kê và sàn lọc các kết quả tìm kiếm. Kẻ lừa đảo có thể sử dụng các công cụ AI để làm "cánh tay" đắc lực hỗ trợ trong việc sàn lọc thông tin, qua đó chúng sẽ dễ dàng tìm hiểu về các kĩ thuật đánh lừa và sử dụng chúng một cách tinh vi để đánh lừa người dùng, bao gồm:

<a name="ky-thuat-spoofing"></a>
### 1. Kỹ thuật Spoofing: 
Kỹ thuật Spoofing là một thủ đoạn tinh vi được sử dụng bởi kẻ lừa đảo trong các vụ `tấn công phishing` nhằm `che giấu danh tính` thực sự của họ và đánh lừa người dùng tiết lộ thông tin cá nhân hoặc thực hiện hành động theo yêu cầu. Kỹ thuật này thường được sử dụng kết hợp với các kỹ thuật lừa đảo khác như `Social Engineering` để tăng hiệu quả tấn công.

**Dựa trên phương thức thực hiện, kỹ thuật Spoofing có thể được chia thành các loại chính sau:**

- **IP Spoofing:** Kẻ lừa đảo thay đổi địa chỉ IP nguồn trong các gói tin dữ liệu để đánh lừa hệ thống máy tính tin rằng gói tin đến từ một nguồn đáng tin cậy. Ví dụ: kẻ lừa đảo có thể giả mạo địa chỉ IP của ngân hàng để gửi email phishing đến khách hàng.
- **Email Spoofing:** Kẻ lừa đảo giả mạo địa chỉ email của một tổ chức uy tín để gửi email phishing đến người dùng. Ví dụ: kẻ lừa đảo có thể sử dụng địa chỉ email giả mạo giống hệt địa chỉ email của ngân hàng để gửi email thông báo về hoạt động đáng ngờ trong tài khoản của người dùng.
- **Website Spoofing:** Kẻ lừa đảo tạo ra một trang web giả mạo giống hệt trang web của một tổ chức uy tín để đánh lừa người dùng truy cập và cung cấp thông tin cá nhân. Ví dụ: kẻ lừa đảo có thể tạo một trang web giả mạo giống hệt trang web đăng nhập của ngân hàng để đánh cắp thông tin đăng nhập của khách hàng.
- **DNS Spoofing:** Kẻ lừa đảo tấn công máy chủ DNS và thay đổi các bản ghi DNS để hướng lưu lượng truy cập của người dùng đến các trang web giả mạo. Ví dụ: khi người dùng truy cập vào trang web của ngân hàng, họ có thể bị chuyển hướng đến một trang web giả mạo do kẻ lừa đảo kiểm soát.
- **Caller ID Spoofing:** Kẻ lừa đảo sử dụng công nghệ để thay đổi số điện thoại hiển thị trên màn hình của người gọi khi họ thực hiện cuộc gọi điện thoại. Ví dụ: kẻ lừa đảo có thể sử dụng số điện thoại của ngân hàng để gọi cho khách hàng và yêu cầu họ cung cấp thông tin cá nhân.

<a name="ky-thuat-social-engineering"></a>
### 2. Kỹ thuật Social Engineering: 
Kỹ thuật Social Engineering (kỹ thuật thao túng tâm lý) là một thủ đoạn tinh vi được sử dụng bởi kẻ lừa đảo trong các vụ `tấn công phishing` nhằm đánh lừa người dùng `tiết lộ thông tin cá nhân` hoặc thực hiện hành động theo yêu cầu của họ. Kỹ thuật này khai thác những yếu tố tâm lý con người như `lòng tin`, `sự tò mò`, `sợ hãi`, v.v. để khiến người dùng đưa ra những quyết định không sáng suốt.

**Dựa trên phương thức thực hiện, kỹ thuật Social Engineering có thể được chia thành các loại chính sau:**

- **Baiting:** Kẻ lừa đảo sử dụng mồi nhử hấp dẫn như quà tặng miễn phí, giải thưởng, hoặc thông tin độc quyền để thu hút sự chú ý của người dùng và khiến họ thực hiện hành động mong muốn. Ví dụ: kẻ lừa đảo có thể gửi email thông báo cho người dùng rằng họ đã giành được giải thưởng và yêu cầu họ cung cấp thông tin cá nhân để nhận thưởng.
- **Pretexting:** Kẻ lừa đảo tạo ra một câu chuyện hoặc tình huống giả mạo để khiến người dùng tin tưởng và tiết lộ thông tin cá nhân. Ví dụ: kẻ lừa đảo có thể giả vờ là nhân viên cơ quan chức năng và yêu cầu người dùng cung cấp thông tin cá nhân để "điều tra một vụ án".
- **Quid pro quo:** Kẻ lừa đảo đề nghị cung cấp cho người dùng một thứ gì đó có giá trị để đổi lấy thông tin cá nhân hoặc hành động của họ. Ví dụ: kẻ lừa đảo có thể đề nghị cung cấp cho người dùng phần mềm miễn phí để đổi lấy thông tin email của họ.
- **Scareware:** Kẻ lừa đảo sử dụng các thông điệp đe dọa hoặc cảnh báo để khiến người dùng sợ hãi và thực hiện hành động mong muốn. Ví dụ: kẻ lừa đảo có thể hiển thị thông báo trên màn hình máy tính thông báo rằng máy tính bị nhiễm virus và yêu cầu người dùng mua phần mềm chống virus giả mạo để "sửa chữa" máy tính.

>>_Sở dĩ có cả kĩ thuật `Social Engineering` trong `Phishing` là vì Phishing là một kỹ thuật phổ biến trong Social Engineering và thường được `sử dụng kết hợp` với các kỹ thuật khác để tăng hiệu quả tấn công. Thay vì chỉ tập trung vào một kỹ thuật cụ thể, việc cung cấp thông tin về Social Engineering giúp người dùng có được kiến thức và kỹ năng cần thiết để bảo vệ bản thân khỏi nhiều loại tấn công mạng._

<a name="ky-thuat-su-dung-hinh-and-va-ngon-ngu"></a>
### 3. Kỹ thuật sử dụng hình ảnh và ngôn ngữ: 
Kỹ thuật sử dụng hình ảnh và ngôn ngữ là một yếu tố quan trọng trong các chiến dịch lừa đảo phishing nhằm đánh lừa người dùng và khiến họ tin tưởng vào tính xác thực của thông tin. Kẻ lừa đảo `sử dụng những hình ảnh và ngôn ngữ chuyên nghiệp`, trau chuốt để tạo dựng hình ảnh uy tín và khiến người dùng không mảy may nghi ngờ.

**Phân tích kỹ thuật sử dụng hình ảnh và ngôn ngữ:**

- **Hình ảnh:**
	+ Sử dụng logo của các tổ chức uy tín để tạo dựng niềm tin cho người dùng.
	+ Sử dụng hình ảnh chất lượng cao, thiết kế chuyên nghiệp để tạo cảm giác an toàn và tin tưởng.
	+ Sử dụng hình ảnh có liên quan đến chủ đề email hoặc trang web giả mạo để tăng tính thuyết phục.
	+ Sử dụng hình ảnh tạo cảm giác cấp bách hoặc hối thúc để khiến người dùng đưa ra quyết định nhanh chóng mà không suy nghĩ kỹ lưỡng.
- **Ngôn ngữ:**
	+ Sử dụng ngôn ngữ trang trọng, lịch sự và chuyên nghiệp để tạo dựng hình ảnh uy tín.
	+ Sử dụng ngữ pháp chính xác, không có lỗi chính tả để tăng tính tin cậy.
	+ Sử dụng các từ ngữ tạo cảm giác cấp bách hoặc hối thúc để khiến người dùng hành động ngay lập tức.
	+ Sử dụng các từ ngữ đánh vào tâm lý người dùng như `miễn phí`, `giải thưởng`, `bảo mật`, v.v. để thu hút sự chú ý và khiến họ tin tưởng.

Lừa đảo phishing là một mối đe dọa nghiêm trọng đối với an ninh mạng và có thể gây ra hậu quả nghiêm trọng cho người dùng. Kẻ lừa đảo sử dụng nhiều thủ đoạn tinh vi để đánh lừa người dùng tiết lộ thông tin cá nhân hoặc thực hiện hành động theo yêu cầu của họ. Một số yếu tố tâm lý có thể khiến người dùng dễ mắc lừa phishing bao gồm `thiếu kiến thức`, `tính tò mò`, `lòng tin`, `áp lực thời gian` và `mong muốn hòa nhập`. Kẻ lừa đảo sử dụng các kỹ thuật như `spoofing`, `social engineering` và `sử dụng hình ảnh và ngôn ngữ` để đánh lừa người dùng. Bằng cách nâng cao nhận thức, sử dụng các biện pháp phòng ngừa và hợp tác với nhau, chúng ta có thể tạo dựng một môi trường mạng an toàn cho tất cả mọi người.



