<!-- One change per bullet, on one line: English, then the Vietnamese on the next line. The release workflow sends a version's section to Discord as it is. -->
# What's new in Fabrik · Có gì mới

Test builds (`-beta`) reach only a Fabrik set to get test versions; the same changes then come out for everyone.  
Bản thử (`-beta`) chỉ đến Fabrik đã bật nhận bản thử; sau đó các thay đổi này ra bản chính thức cho mọi người.

## 1.4.3

- Fabrik shows its version in the window title and the top bar, and a report carries it in its file name, so you can always tell which version you are on.
  Fabrik hiện số phiên bản trên thanh tiêu đề và thanh trên cùng, và báo lỗi ghi số phiên bản trong tên tệp, nên bạn luôn biết mình đang dùng bản nào.
- Splitter, Cut: a loading window covers the app as soon as you press Cut, so a big model no longer looks frozen.
  Splitter, Cắt: cửa sổ chờ phủ lên ứng dụng ngay khi bấm Cắt, nên mẫu lớn không còn trông như bị treo.
- Splitter, Cut: when a cut cannot part the model, the loading window says so at once, while it looks for where the model is still joined. Press Stop if you don't need the red line: nothing has been cut.
  Splitter, Cắt: khi vết cắt không tách được mẫu, cửa sổ chờ báo ngay, trong lúc tìm chỗ còn dính. Bấm Dừng nếu không cần xem đường đỏ: chưa có gì bị cắt.

## 1.4.2

- Splitter, Cut: pressing Cut on a big model no longer freezes the app. The check before the cut runs in the background, and Stop ends it.
  Splitter, Cắt: bấm Cắt với mẫu lớn không còn làm treo ứng dụng. Bước kiểm tra trước khi cắt chạy ngầm, và nút Dừng kết thúc được nó.
- Splitter: the loading card shows how far a cut is, as a percentage beside the seconds; work that cannot be measured shows the seconds.
  Splitter: thẻ chờ cho biết vết cắt đã xong bao nhiêu, bằng phần trăm cạnh số giây; việc không đo được thì hiện số giây.
- Splitter: Undo and Redo go back exactly one step in Loop, Plane, Shape and Curve, and bring back the tool you had selected. Deleting a plane and moving a slider are steps too.
  Splitter: Hoàn tác và Làm lại lùi đúng một bước trong Vòng, Mặt phẳng, Hình và Cắt cong, và trả lại công cụ bạn đang chọn. Xóa mặt phẳng và kéo thanh trượt cũng là một bước.
- Splitter, Loop: Preview split shows the parts apart, each ring has its own pin, and Undo takes back Carry on before the cut.
  Splitter, Vòng: Xem trước khi chia hiện các phần tách rời, mỗi vòng có chốt riêng, và Hoàn tác lấy lại Cắt tiếp trước khi lấy lại vết cắt.
- Splitter, Loop: click a ring or its button to edit it, in any order. Rings are numbered, the one being edited stands out, and the ring buttons hold their text in Vietnamese.
  Splitter, Vòng: bấm vào một vòng hoặc nút của nó để sửa, theo thứ tự nào cũng được. Các vòng được đánh số, vòng đang sửa nổi bật, và chữ tiếng Việt nằm gọn trong nút vòng.
- Splitter, Loop: Ctrl+drag shapes a ring at one spot, Ctrl+click adds one point, and Add points says what to do when a ring is full.
  Splitter, Vòng: Ctrl+kéo chỉnh vòng tại một chỗ, Ctrl+bấm thêm một điểm, và Thêm điểm cho biết phải làm gì khi vòng đã đầy.
- Splitter, Loop: when rings do not part the model, the red line shows where it is still joined, looked for away from the cut.
  Splitter, Vòng: khi các vòng không tách được mẫu, đường đỏ chỉ chỗ còn dính, được tìm ở xa vết cắt.
- Splitter, Base: Flatten base and Extend base work inside the app, with nothing else to start. A failed run leaves the part as it was, and a finished one is one Undo step.
  Splitter, Đế: Làm phẳng đế và Kéo dài đế chạy ngay trong ứng dụng, không cần khởi động gì thêm. Lần chạy lỗi giữ nguyên phần như cũ, lần chạy xong là một bước Hoàn tác.
- Splitter: Inspect & repair, Shapes & Boolean, Sculpt, Moulds and Paint image open from the Print rail.
  Splitter: Kiểm tra & sửa, Hình khối & Boolean, Điêu khắc, Khuôn và Tô ảnh mở từ thanh In.

## 1.4.1-beta.1 (test build · bản thử)

- Splitter, Base: Flatten base and Extend base now work inside the app, with nothing else to start. A failed run leaves the part as it was, and a finished one is one Undo step.
  Splitter, Đế: Làm phẳng đế và Kéo dài đế giờ chạy ngay trong ứng dụng, không cần khởi động gì thêm. Lần chạy lỗi giữ nguyên phần như cũ, lần chạy xong là một bước Hoàn tác.
- Splitter, By colour: a new Show colour cuts button draws where each colour edge would be cut, with thick outlined lines; edges that cannot be cut are drawn in red with the reason.
  Splitter, Theo màu: nút Hiện vết cắt theo màu mới vẽ chỗ mỗi biên màu sẽ bị cắt bằng nét dày có viền; biên không cắt được vẽ màu đỏ kèm lý do.
- Splitter, Colours: a new Snap colour edges to grooves button moves each colour edge you drew into the nearest groove or crease of the surface, so colours change where the model does.
  Splitter, Màu: nút Kéo biên màu vào rãnh mới đưa mỗi biên màu bạn vẽ vào rãnh hoặc nếp gần nhất của bề mặt, để màu đổi đúng chỗ mẫu đổi.
- Splitter, Draw: a loop that cannot part the model no longer leaves a spinner running that cannot be stopped; the warning stays in the notes with its Cut out as a patch button.
  Splitter, Vẽ: vòng cắt không tách được mẫu không còn để lại vòng xoay chạy mãi không dừng được; cảnh báo nằm trong thông báo cùng nút Cắt thành miếng vá.
- Splitter, Cut: a check after every cut says whether each part is a closed solid, whether the parts hold the volume of the model, and how close the parts come to each other (the cut gap), and warns when something is wrong. On a model of a million triangles it runs after the result is on screen.
  Splitter, Cắt: sau mỗi lần cắt có bước kiểm tra xem từng phần có kín không, tổng thể tích các phần có đủ không và các phần cách nhau bao nhiêu (khe cắt), và cảnh báo khi có gì không ổn. Với mẫu cả triệu tam giác, bước này chạy sau khi kết quả đã hiện.
- Splitter, Loop: a ring that leaves a thin lid, cap or brim (under about 0.6 mm) is no longer refused as "does not separate".
  Splitter, Vòng: vòng cắt để lại nắp, chóp hoặc vành mỏng (dưới khoảng 0,6 mm) không còn bị từ chối với thông báo "không tách được".
- Splitter: a cut that fails now says why in plain words and what to do: the cut misses the model, stops on it, stays inside it, runs too close to the surface, the gap takes all of one side, a loop has too few points or crosses itself.
  Splitter: vết cắt thất bại giờ nói rõ lý do và cách xử lý: vết cắt lệch khỏi mẫu, dừng trên mẫu, nằm trọn bên trong, đi quá sát bề mặt, khe cắt ăn hết một bên, vòng có quá ít điểm hoặc tự cắt qua chính nó.
- Splitter: when a cut leaves the model in one piece, a red line on the model shows the place that still holds it together.
  Splitter: khi vết cắt chưa tách được mẫu, một đường đỏ trên mẫu chỉ ra chỗ còn giữ hai bên dính lại.
- Splitter: a model made of separate closed pieces no longer gets a card saying it will not cut; one line says what is ready before you cut.
  Splitter: mẫu gồm nhiều mảnh kín rời nhau không còn bị báo là không cắt được; một dòng cho biết mẫu đã sẵn sàng trước khi cắt.
- Splitter, Export 3MF: every part is checked as the slicer will read it first; a wall too thin for the file's numbers is written with more digits, and a part that cannot be written is stopped with the reason.
  Splitter, Xuất 3MF: mỗi phần được kiểm tra trước theo cách slicer sẽ đọc; thành quá mỏng so với độ chính xác của tệp sẽ được ghi nhiều chữ số hơn, phần không ghi được sẽ bị dừng kèm lý do.
- Splitter: Hollow, Add peg, Grid, Base and Fit the bed work again on a model that needs a repair first (they stopped with a meaningless error); a failed Hollow or Auto Finish now really leaves everything as it was.
  Splitter: Làm rỗng, Thêm chốt, Lưới, Đế và Cho vừa bàn in lại chạy được với mẫu cần sửa trước (trước đây dừng với lỗi vô nghĩa); Làm rỗng hoặc Hoàn thiện tự động thất bại giờ thật sự giữ nguyên mọi thứ.
- Splitter: a loose fragment folded back into a part no longer touches the part beside it, which could weld the two together in the print.
  Splitter: mảnh rời được gộp lại vào một phần không còn chạm phần bên cạnh, điều có thể làm hai phần dính nhau khi in.
- Splitter: the check after a cut now runs after every kind of cut, knows a press fit from a fault, and says when pieces already overlapped before the cut.
  Splitter: bước kiểm tra sau khi cắt giờ chạy sau mọi kiểu cắt, phân biệt được khớp ép với lỗi, và cho biết khi các mảnh đã chồng lên nhau từ trước khi cắt.
- Reports: the report now says which part went wrong (the tool in use is chosen for you), takes pictures pasted with Ctrl+V, and carries Splitter's last messages and state; every Splitter error ends with a short code you can quote.
  Báo lỗi: báo lỗi giờ cho chọn chức năng bị lỗi (chọn sẵn công cụ đang dùng), nhận ảnh dán bằng Ctrl+V, và kèm các thông báo cùng trạng thái gần nhất của Splitter; mỗi lỗi của Splitter có một mã ngắn để bạn đọc cho mình.

## 1.4.1

- Splitter, By colour: a new Show colour cuts button draws where each colour edge would be cut, with thick outlined lines; edges that cannot be cut are drawn in red with the reason.
  Splitter, Theo màu: nút Hiện vết cắt theo màu mới vẽ chỗ mỗi biên màu sẽ bị cắt bằng nét dày có viền; biên không cắt được vẽ màu đỏ kèm lý do.
- Splitter, Colours: a new Snap colour edges to grooves button moves each colour edge you drew into the nearest groove or crease of the surface, so colours change where the model does.
  Splitter, Màu: nút Kéo biên màu vào rãnh mới đưa mỗi biên màu bạn vẽ vào rãnh hoặc nếp gần nhất của bề mặt, để màu đổi đúng chỗ mẫu đổi.
- Splitter, Draw: a loop that cannot part the model no longer leaves a spinner running that cannot be stopped; the warning stays in the notes with its Cut out as a patch button.
  Splitter, Vẽ: vòng cắt không tách được mẫu không còn để lại vòng xoay chạy mãi không dừng được; cảnh báo nằm trong thông báo cùng nút Cắt thành miếng vá.
- Splitter, Cut: a check after every cut says whether each part is a closed solid, whether the parts hold the volume of the model, and how close the parts come to each other (the cut gap), and warns when something is wrong. On a model of a million triangles it runs after the result is on screen.
  Splitter, Cắt: sau mỗi lần cắt có bước kiểm tra xem từng phần có kín không, tổng thể tích các phần có đủ không và các phần cách nhau bao nhiêu (khe cắt), và cảnh báo khi có gì không ổn. Với mẫu cả triệu tam giác, bước này chạy sau khi kết quả đã hiện.
- Splitter, Loop: a ring that leaves a thin lid, cap or brim (under about 0.6 mm) is no longer refused as "does not separate".
  Splitter, Vòng: vòng cắt để lại nắp, chóp hoặc vành mỏng (dưới khoảng 0,6 mm) không còn bị từ chối với thông báo "không tách được".
- Splitter: a cut that fails now says why in plain words and what to do: the cut misses the model, stops on it, stays inside it, runs too close to the surface, the gap takes all of one side, a loop has too few points or crosses itself.
  Splitter: vết cắt thất bại giờ nói rõ lý do và cách xử lý: vết cắt lệch khỏi mẫu, dừng trên mẫu, nằm trọn bên trong, đi quá sát bề mặt, khe cắt ăn hết một bên, vòng có quá ít điểm hoặc tự cắt qua chính nó.
- Splitter: when a cut leaves the model in one piece, a red line on the model shows the place that still holds it together.
  Splitter: khi vết cắt chưa tách được mẫu, một đường đỏ trên mẫu chỉ ra chỗ còn giữ hai bên dính lại.
- Splitter: a model made of separate closed pieces no longer gets a card saying it will not cut; one line says what is ready before you cut.
  Splitter: mẫu gồm nhiều mảnh kín rời nhau không còn bị báo là không cắt được; một dòng cho biết mẫu đã sẵn sàng trước khi cắt.
- Splitter, Export 3MF: every part is checked as the slicer will read it first; a wall too thin for the file's numbers is written with more digits, and a part that cannot be written is stopped with the reason.
  Splitter, Xuất 3MF: mỗi phần được kiểm tra trước theo cách slicer sẽ đọc; thành quá mỏng so với độ chính xác của tệp sẽ được ghi nhiều chữ số hơn, phần không ghi được sẽ bị dừng kèm lý do.
- Splitter: Hollow, Add peg, Grid, Base and Fit the bed work again on a model that needs a repair first (they stopped with a meaningless error); a failed Hollow or Auto Finish now really leaves everything as it was.
  Splitter: Làm rỗng, Thêm chốt, Lưới, Đế và Cho vừa bàn in lại chạy được với mẫu cần sửa trước (trước đây dừng với lỗi vô nghĩa); Làm rỗng hoặc Hoàn thiện tự động thất bại giờ thật sự giữ nguyên mọi thứ.
- Splitter: a loose fragment folded back into a part no longer touches the part beside it, which could weld the two together in the print.
  Splitter: mảnh rời được gộp lại vào một phần không còn chạm phần bên cạnh, điều có thể làm hai phần dính nhau khi in.
- Splitter: the check after a cut now runs after every kind of cut, knows a press fit from a fault, and says when pieces already overlapped before the cut.
  Splitter: bước kiểm tra sau khi cắt giờ chạy sau mọi kiểu cắt, phân biệt được khớp ép với lỗi, và cho biết khi các mảnh đã chồng lên nhau từ trước khi cắt.
- Reports: the report now says which part went wrong (the tool in use is chosen for you), takes pictures pasted with Ctrl+V, and carries Splitter's last messages and state; every Splitter error ends with a short code you can quote.
  Báo lỗi: báo lỗi giờ cho chọn chức năng bị lỗi (chọn sẵn công cụ đang dùng), nhận ảnh dán bằng Ctrl+V, và kèm các thông báo cùng trạng thái gần nhất của Splitter; mỗi lỗi của Splitter có một mã ngắn để bạn đọc cho mình.

## 1.4.0

- Splitter, Pins: the pin goes where you click, and a placed pin can be moved, made bigger or smaller, and given an exact radius and reach in mm; a magnet can be any size.
  Splitter, Chốt: chốt nằm đúng chỗ bạn bấm, chốt đã đặt có thể dời, làm to nhỏ và đặt bán kính, độ ăn sâu chính xác theo mm; nam châm có thể có cỡ bất kỳ.
- Splitter, Pins: new outlines (hexagon, square, tapered square, star, cross), loose Tenons with those outlines, and 1 to 12 pins on a face.
  Splitter, Chốt: thêm các hình dạng mới (lục giác, vuông, vuông côn, sao, chữ thập), chốt rời Tenon có các hình đó, và từ 1 đến 12 chốt trên một mặt.
- Splitter, Plane: start from X, Y, Z or the view, set Position and Angle, Swap the halves, and pick which separate areas a plane cuts.
  Splitter, Mặt phẳng: bắt đầu từ trục X, Y, Z hoặc hướng nhìn, đặt Vị trí và Góc, Đổi hai nửa, và chọn vùng riêng nào mặt phẳng sẽ cắt.
- Splitter, Draw: a stroke carries on across views from its loose end and closes when it comes back to its start.
  Splitter, Vẽ: nét vẽ tiếp tục qua nhiều góc nhìn từ đầu nét còn lơ lửng và khép lại khi quay về điểm đầu.
- Splitter: after a cut, carry on cutting one part (the others are set aside but kept for export), and Joint numbers cut the same number into both faces of every joint.
  Splitter: sau khi cắt, cắt tiếp một phần (các phần khác để sang bên nhưng vẫn được xuất), và Số mối ghép khắc cùng một số vào cả hai mặt của mỗi mối ghép.
- Splitter: a Mask for every cut tool (paint a part, hide the rest; the cut still uses the whole model), and Inspect & repair with Advanced repair and Separate the loose pieces.
  Splitter: Mặt nạ cho mọi công cụ cắt (tô một phần, ẩn phần còn lại; vết cắt vẫn dùng cả mẫu), và Kiểm tra & sửa với Sửa nâng cao và Tách các mảnh rời.
- Splitter: new tools Shapes & Boolean (cube, ball, tube, cone, ring; union, difference, intersect), Sculpt (smooth, flatten, inflate, deflate) and Moulds (a printable silicone mould box with lid, pour hole and air vents, or a jacket).
  Splitter: công cụ mới Hình khối & Boolean (lập phương, cầu, ống, nón, vòng; hợp, hiệu, giao), Điêu khắc (làm mịn, làm phẳng, phồng, xẹp) và Khuôn (hộp khuôn silicone in được có nắp, lỗ rót và lỗ thoát khí, hoặc khuôn áo).

## 1.3.1

- Splitter checks a model as it opens: if it is not a closed solid, a card says what is wrong and Repair it now fixes it; a cut that fails on a faulty model offers the repair and cuts again.
  Splitter kiểm tra mẫu ngay khi mở: nếu không phải khối kín, một thẻ cho biết lỗi và nút Sửa ngay sẽ sửa; vết cắt thất bại trên mẫu lỗi sẽ đề nghị sửa rồi cắt lại.
- Splitter: a heavy model is offered Reduce for cutting (Light, Balanced, Strong), so it cuts and paints faster; Undo brings full detail back.
  Splitter: mẫu nặng được đề nghị Giảm để cắt (Nhẹ, Cân bằng, Mạnh) để cắt và tô nhanh hơn; Hoàn tác đưa lại đầy đủ chi tiết.
- Splitter: a model saved in metres or inches gets a card to scale it, and cuts no longer fail on it with a puzzling message.
  Splitter: mẫu lưu theo mét hoặc inch có thẻ để chỉnh tỉ lệ, và không còn cắt lỗi với thông báo khó hiểu.
- Splitter: cuts run in the background with a card showing what is happening and for how long; Stop ends a cut, and the page no longer freezes.
  Splitter: việc cắt chạy nền với thẻ cho biết đang làm gì và bao lâu; nút Dừng kết thúc vết cắt, trang không còn bị đơ.
- Splitter: the left mouse button is always the tool; right-drag turns the view, middle-drag pans, the wheel zooms.
  Splitter: chuột trái luôn dành cho công cụ; kéo chuột phải để xoay, kéo chuột giữa để dời, con lăn để phóng to thu nhỏ.
- Splitter, Loop: drag the loop itself and it eases into place; dragged spots are pinned, right-click releases a pin, and Snap to edges pulls it into the nearest crease.
  Splitter, Vòng: kéo chính vòng cắt và nó giãn mềm vào chỗ; chỗ đã kéo được ghim, chuột phải để thả ghim, và Bám vào cạnh kéo vòng vào nếp gấp gần nhất.
- Splitter: Ctrl+Z undoes the last thing you did, a stray line included, and Ctrl+Shift+Z puts it back; Cut and Auto split open on their tools with none started.
  Splitter: Ctrl+Z hoàn tác việc vừa làm, kể cả đường cắt vẽ nhầm, và Ctrl+Shift+Z làm lại; Cắt và Tự chia mở ra danh sách công cụ, chưa bật công cụ nào.

## 1.3.0

- Splitter's cut tools all work the same way: 1 mark the cut, 2 adjust it, 3 Cut, with one Cut button; a card on top of the view says what to do next.
  Các công cụ cắt của Splitter giờ dùng chung một cách: 1 đánh dấu vết cắt, 2 chỉnh lại, 3 Cắt, với một nút Cắt duy nhất; một thẻ trên khung nhìn cho biết bước tiếp theo.
- Splitter: the Cut menu is Line, Loop, Paint, Curve, Add pins and Review. Curved & drafts is gone: Curve draws a curved cut you can still edit, Review holds cuts waiting to be built.
  Splitter: menu Cắt gồm Đường thẳng, Vòng, Tô vùng, Cắt cong, Thêm chốt và Xem lại. Bỏ Cắt cong & bản nháp: Cắt cong vẽ vết cắt cong vẫn sửa được, Xem lại giữ các vết cắt đang chờ dựng.
- Splitter, Add pins: cut without a pin, then click each cut face to put a pin there, any joint, with its size and length.
  Splitter, Thêm chốt: cắt không chốt, rồi bấm vào từng mặt cắt để đặt chốt ở đó, kiểu khớp nào cũng được, chỉnh cỡ và độ dài.
- Splitter: a Magnet joint makes a hole in each part for a bought disc magnet, 4x3 to 25x5 mm, so it sits flush.
  Splitter: khớp Nam châm khoét lỗ ở mỗi phần vừa nam châm tròn mua sẵn, từ 4x3 đến 25x5 mm, để nam châm nằm ngang mặt.
- Splitter: undo a cut and what you drew (line, loop, paint, shape or curve) comes back, ready to change and cut again.
  Splitter: hoàn tác một vết cắt thì những gì bạn đã vẽ (đường, vòng, vùng tô, hình hoặc đường cong) quay lại, sẵn sàng sửa và cắt lại.
- Splitter: Spread, beside the 3D view, pulls the parts apart to look at the cut faces and pins, and puts them back.
  Splitter: nút Tách ra cạnh khung 3D kéo các phần ra xa để xem mặt cắt và chốt, rồi ghép lại.
- Splitter, Paint: opens with the brush on, and when the painted part still touches the rest (a skirt frill on a leg) it marks the spot in red and says what to do.
  Splitter, Tô vùng: mở là bật cọ ngay, và khi phần đã tô còn chạm phần còn lại (diềm váy chạm chân) thì đánh dấu đỏ chỗ chạm và nói cách xử lý.
- Splitter, Loop: drag any point straight away, only that point moves, and the line runs where the points are. A loop that cannot part the model is no longer cut out as a patch on its own.
  Splitter, Vòng: kéo điểm nào cũng được ngay, chỉ điểm đó di chuyển, và đường cắt đi đúng qua các điểm. Vòng không tách được mẫu không còn tự bị khoét thành mảng.
- Fabrik's window no longer reacts to browser keys such as Ctrl+F, Ctrl+R and F5.
  Cửa sổ Fabrik không còn phản hồi các phím của trình duyệt như Ctrl+F, Ctrl+R và F5.

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
