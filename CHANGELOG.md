<!-- One change per bullet, on one line: English, then the Vietnamese on the next line. The release workflow sends a version's section to Discord as it is. -->
# What's new in Fabrik · Có gì mới

Test builds (`-nightly`) reach only a Fabrik set to get test versions; the same changes then come out for everyone.  
Bản thử (`-nightly`) chỉ đến Fabrik đã bật nhận bản thử; sau đó các thay đổi này ra bản chính thức cho mọi người.

## 1.2.0

- Splitter has a new layout: all cut tools in one column on the left, Draw a cut (Line, Ring, Paint, Curved) and Auto split (Body parts, Fit the bed, Grid, By colour), and the model stays clear on a 1280 x 640 screen.
  Splitter có bố cục mới: mọi công cụ cắt nằm trong một cột bên trái, Vẽ vết cắt (Đường thẳng, Vòng, Tô vùng, Cong) và Tự chia (Phần cơ thể, Vừa bàn in, Lưới, Theo màu); mẫu vẫn thấy rõ trên màn hình 1280 x 640.
- Splitter, Paint: paint the piece you want to cut off with a brush or fill, Check my paint, then Cut from paint. When a cut can't be made, it says why in plain words and marks the stray patch.
  Splitter, Tô vùng: tô phần muốn cắt ra bằng cọ hoặc đổ màu, Kiểm tra vùng tô, rồi Cắt từ vùng tô. Khi không cắt được, Splitter nói rõ lý do và đánh dấu mảng tô bị lạc.
- Splitter: Auto everything cuts into body parts, fits them to the bed, numbers the parts and lays out the plates in one click, then tells you what it did. Turn on Review the cuts first to check each cut before it is made.
  Splitter: Tự động tất cả chia theo phần cơ thể, cho vừa bàn in, đánh số các phần và xếp lên bàn in chỉ với một lần bấm, rồi cho biết đã làm gì. Bật Xem lại các vết cắt trước để kiểm tra từng vết cắt trước khi cắt.
- Splitter: one Joints card under every cut tool, with a new Push-fit joint and a choice of cut face; a Spread the parts slider for every cut.
  Splitter: một thẻ Khớp nối chung dưới mọi công cụ cắt, thêm khớp Cắm khít và chọn mặt cắt; thanh Dãn các phần ra cho mọi vết cắt.
- Splitter: export an assembly guide (PDF) showing which part goes where.
  Splitter: xuất hướng dẫn lắp ráp (PDF) cho biết phần nào lắp vào đâu.
- Splitter: a model with a few open or flipped faces is repaired and cut, instead of failing with Not manifold; a warning before cutting catches wrong units and open models.
  Splitter: mẫu có vài mặt hở hoặc bị lật giờ được sửa rồi cắt, không còn báo lỗi Not manifold; một cảnh báo trước khi cắt phát hiện sai đơn vị và mẫu bị hở.
- Splitter: a cut that parts off a very small piece keeps it as a part, and joints no longer leave paper-thin slivers on the cut face.
  Splitter: vết cắt tách ra một mảnh rất nhỏ vẫn giữ mảnh đó thành một phần, và khớp nối không còn để lại lớp mỏng như giấy trên mặt cắt.
- Fabrik's window can no longer be made too small for the apps (1280 x 680 at 100% scaling), and it opens at least that big.
  Cửa sổ Fabrik không còn thu nhỏ quá mức cho các ứng dụng (1280 x 680 ở tỉ lệ 100%), và luôn mở ít nhất cỡ đó.
- Messages that came out half in English are now fully in Vietnamese.
  Các thông báo trước đây nửa tiếng Anh giờ đã hoàn toàn bằng tiếng Việt.

## 1.1.0

- Splitter, Loop and Cut & Pin: new setting Plan the pin automatically, off by default. Off, moving a point no longer makes you wait while the pin is planned again: press Plan pin when the cut is where you want it. Apply places the pin either way.
  Splitter, Vòng và Cut & Pin: thêm cài đặt Tự tính chốt, mặc định tắt. Khi tắt, di chuyển một điểm không còn phải chờ tính lại chốt: bấm Tính chốt khi đường cắt đã đúng chỗ. Áp dụng vẫn đặt chốt dù bật hay tắt.
- Splitter: the region colours in the parts preview (By limbs, By colour) now show clean regions on big models (over 700,000 triangles), instead of stripes all over the model.
  Splitter: màu các vùng khi xem trước (Theo tay chân, Theo màu) giờ hiện đúng từng vùng trên mẫu lớn (trên 700.000 tam giác), không còn bị sọc lốm đốm khắp mẫu.
- Splitter: colours on a painted model no longer get mixed up after you click on it.
  Splitter: màu trên mẫu đã tô không còn bị xáo trộn sau khi bấm vào mẫu.
- Updates install while a print is running: the printer carries on, and Spotter is back watching it a few seconds later.
  Cài bản cập nhật được cả khi máy đang in: máy vẫn in tiếp, vài giây sau Spotter lại theo dõi.
- The start page no longer has the Open all button.
  Trang đầu bỏ nút Mở tất cả.
- Pointing at a link no longer shows its address at the bottom of Fabrik's window.
  Rê chuột lên đường link không còn hiện địa chỉ ở góc dưới cửa sổ Fabrik.

## 1.0.1-nightly.1 (test build · bản thử)

- Splitter: the region colours in the parts preview (By limbs, By colour) now show clean regions on big models (over 700,000 triangles), instead of stripes all over the model.
  Splitter: màu các vùng khi xem trước (Theo tay chân, Theo màu) giờ hiện đúng từng vùng trên mẫu lớn (trên 700.000 tam giác), không còn bị sọc lốm đốm khắp mẫu.
- Updates install while a print is running: the printer carries on, and Spotter is back watching it a few seconds later.
  Cài bản cập nhật được cả khi máy đang in: máy vẫn in tiếp, vài giây sau Spotter lại theo dõi.
- The start page no longer has the Open all button.
  Trang đầu bỏ nút Mở tất cả.
- Pointing at a link no longer shows its address at the bottom of Fabrik's window.
  Rê chuột lên đường link không còn hiện địa chỉ ở góc dưới cửa sổ Fabrik.

## 1.0.0

- Maker, Splitter, Bracer and Spotter together in one window.
  Maker, Splitter, Bracer và Spotter chung một cửa sổ.
- Choose English or Tiếng Việt the first time you open it.
  Chọn English hoặc Tiếng Việt khi mở lần đầu.
- Spotter watches your printers and sends alerts to Telegram or email.
  Spotter theo dõi máy in và gửi thông báo qua Telegram hoặc email.
- Report a problem from any working page, then send the file to Derek.
  Báo lỗi từ bất kỳ trang làm việc nào, rồi gửi tệp cho Derek.
- Fabrik checks for a new version once a day and asks before installing.
  Fabrik kiểm tra bản mới mỗi ngày một lần và hỏi trước khi cài.
