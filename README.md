B
Bạn đang thiết kế một biểu đồ cột (Bar chart) để so sánh hiệu suất giữa hai nhóm, với sự khác biệt thực tế chỉ là 5% (ví dụ: 95% so với 100%). Để làm cho sự khác biệt này trông ấn tượng và lớn hơn trong mắt người xem, bạn quyết định cắt trục Y (Truncated Y-axis), bắt đầu từ giá trị 90% thay vì 0%. Hành động này đã vi phạm nguyên tắc thiết kế trực quan hóa nào?
Đáp án: Trung thực

Bạn cần trực quan hóa và so sánh mức độ yêu thích trung bình (thang điểm 1-10) của 8 loại sản phẩm khác nhau. Khi có nhiều danh mục, loại biểu đồ nào được khuyến nghị là gọn gàng và giúp so sánh giá trị đơn lẻ giữa các danh mục hiệu quả?
Đáp án: Dot plot (Biểu đồ điểm).

Bạn có một bảng dữ liệu bán hàng, trong đó mỗi sản phẩm có thể xuất hiện nhiều lần... Muốn tạo báo cáo bán hàng từng sản phẩm theo tháng (dạng rộng, hiển thị tổng doanh số)... dùng hàm nào?
Đáp án: pd.pivot_table()

Bạn cần đọc nhiều sheet từ file Excel lớn. Cách nào tránh phải mở file nhiều lần?
Đáp án: xfile = pd.ExcelFile("file.xlsx") xfile.parse("Sheet1") xfile.parse("Sheet2")

Bạn muốn đọc file orders.xlsx trong đó dữ liệu cần lấy nằm ở sheet thứ hai trong workbook. Lệnh nào phù hợp?
Đáp án: pd.read_excel("orders.xlsx", sheet_name=1)

Bạn muốn đọc file report.csv nhưng chỉ đọc 100 dòng đầu tiên để xem trước dữ liệu. Lệnh nào nên dùng?
Đáp án: pd.read_csv("report.csv", nrows=100)

Bạn muốn đọc file report.xlsx nhưng chỉ đọc 50 dòng đầu tiên để xem trước dữ liệu. Lệnh nào nên dùng?
Đáp án: pd.read_excel("report.xlsx", nrows=50)

Biểu đồ nào phù hợp trong các biểu đồ dưới đây dùng để hiển thị dữ liệu theo thời gian?
Đáp án: Biểu đồ đường (Line chart).

Bước Làm sạch dữ liệu trong bối cảnh phân tích kinh doanh thường bao gồm việc xử lý vấn đề nào?
Đáp án: Xử lý dữ liệu bị thiếu hoặc trùng lặp.

C
Cách viết comment một dòng trong Python là gì?
Đáp án: # comment

Câu lệnh nào sau đây đúng để tạo một DataFrame từ danh sách (sales) trong thư viện Pandas?
Đáp án: pd.DataFrame(sales)

Câu lệnh sau đây thực hiện thao tác biến đổi nào trên DataFrame df? df.pivot(index="date", columns="item", values="value")
Đáp án: Tạo DataFrame mới với các dòng là các ngày ("date"), các cột là tên các mặt hàng ("item"), và điền dữ liệu vào ô bằng cột "value".

Câu lệnh sau đây thực hiện thao tác biến đổi nào trên DataFrame df? pandas.melt(df, id_vars="key", value_vars=["A", "B"])
Đáp án: Chuyển các cột "A", "B" thành các hàng, giữ nguyên cột "key" làm cột định danh.

Câu lệnh thêm cột "len_name" chứa độ dài chuỗi của cột "name" là gì?
Đáp án: df["len_name"] = df["name"].str.len()

Cấu trúc if...elif...else sau đây có hợp lệ không? (if x > 5:... elif x == 5:... else:...)
Đáp án: Hợp lệ.

Cấu trúc nào không dùng để truy cập nhiều cột?
Đáp án: df.get('A', 'B')

Câu nào sau đây là cú pháp đúng để định nghĩa hàm trong Python?
Đáp án: def myFunction() :

Cho DataFrame df, cú pháp df.iloc[2] sẽ trả về đối tượng gì?
Đáp án: Series

Cho dataframe, làm sao để tính tổng lượt truy cập theo ngày?
Đáp án: Sử dụng hàm groupby() kết hợp với hàm sum().

Cho dữ liệu JSON có dạng sau: {"meta": {...}, "data": [{"id":1,...},{"id":2,...}]}. Cách nào để lấy DataFrame từ phần “data”, không phụ thuộc vào phần “meta”?
Đáp án: obj = json.loads(json_str); df = pd.DataFrame(obj["data"])

Cho đoạn code sau, kết quả in ra là gì: a = np.array([5, 10, 15, 20]); print(a[1:3])
Đáp án: 10 15

Cho đoạn code sau, kết quả in ra là gì: x=1; while x<4: x*=2; print(x)
Đáp án: 4

Cho hai DataFrame df1 và df2... Thực hiện đoạn mã sau cho kết quả như thế nào? pd.merge(df1, df2, on='key', how='inner')
Đáp án: DataFrame kết quả có 6 dòng.

Cho hai DataFrame: SanPham... GiaBan... Đoạn mã nào sau đây phù hợp để nối hai DataFrame sao cho toàn bộ sản phẩm trong DataFrame SanPham được giữ lại cùng với giá bán?
Đáp án: pd.merge(GiaBan, SanPham, on="ma_sp", how="right")

Cho DataFrame df, câu lệnh thêm cột "len name chứa độ đã chuỗi của cột "name" là gì?
Đáp án: df["len_name"] = df["name"].str.len()

Cho DataFrame df chứa dữ liệu lịch sử truy cập website với các cột: ngay, gio, luot_truy_cap. Câu lệnh nào của Python dùng để tính tổng lượt truy cập theo từng ngày (cột “ngay”) là gì?
Đáp án: df.groupby("ngay")["luot_truy_cap"].sum()

Cho mảng hai chiều arr. Cú pháp arr.sum() sử dụng để tính gì?
Đáp án: Tổng tất cả các phần tử của mảng.

Cho Series s. Thuộc tính s.index.name dùng để làm gì?
Đáp án: Đặt hoặc lấy tên của chỉ mục (index) của Series.

Cho series: s = pd.Series([4, 7, 5, 3], index=["d", "b", "a", "c"]); print(s["a"]). Kết quả là:
Đáp án: 5.

Công thức, cấu trúc IQR?
Đáp án: IQR = Q3 - Q1

D
Dictionary có cho phép trùng key không?
Đáp án: Không

Dùng KNN Hồi quy (K=3) với 3 hàng xóm là [10, 12, 14], giá trị dự đoán là bao nhiêu?
Đáp án: 12

Dự đoán sai nhiều trong tập train gọi là?
Đáp án: Underfitting (Dưới khớp)

Dữ liệu bán cấu trúc?
Đáp án: JSON

Dữ liệu giao dịch trong kinh doanh có dạng?
Đáp án: Dữ liệu có cấu trúc trong bảng.

Dữ liệu từ API của IMF hoặc World Bank thuộc loại nào?
Đáp án: Dữ liệu vĩ mô về kinh tế, xã hội.

Dùng mô hình 3D khiến người xem đứng gần thấy nó to hơn, các trang trí khiến người quan sát khó tập trung vào dữ liệu. việc lạm dụng mô hình 3D vi phạm nguyên tắc gì?
Đáp án: rõ ràng

Đ
Đặc điểm nào mô tả đúng nhất về định dạng bảng dài (long format)?
Đáp án: Bảng có rất nhiều hàng và ít cột.

Đâu là phương thức dùng để tạo và thêm một subplot vào một Figure trong thư viện Matplotlib?
Đáp án: add_subplot()

Để đảm bảo biểu đồ giữ được độ sắc nét và không bị vỡ (răng cưa) khi phóng to hoặc in ấn ở kích thước lớn, bạn nên ưu tiên sử dụng định dạng file nào sau đây?
Đáp án: PDF

Để đảo ngược thứ tự các phần tử trong một mảng một chiều arr, bạn có thể sử dụng cú pháp slicing nào?
Đáp án: arr[::-1]

Để tính tổng của mỗi cột trong một mảng 2 chiều arr , bạn sẽ sử dụng cú pháp nào?
arr.sum(axis=0)

Để tính giá trị trung bình (mean) của mỗi hàng trong một mảng 2 chiều arr , bạn sẽ sử dụng cú pháp nào?
Đáp án: arr.mean(axis=1

Điều gì xảy ra khi biến trong Python được gán giá trị mới với kiểu dữ liệu khác?
Đáp án: Biến được cập nhật và mang kiểu dữ liệu mới.

Điều gì xảy ra khi thực hiện câu lệnh sau trong Python? my_dict = {}; my_dict[1] = 'one'
Đáp án: Thêm khóa 1 với giá trị 'one' vào từ điển.

Điều gì xảy ra khi thực hiện lệnh các câu lệnh sau: x = [1, 2, 3]; x.append([4, 5])
Đáp án: Danh sách x sẽ có thêm danh sách [4, 5] như một phần tử.

Điều gì sẽ xảy ra nếu một đoạn mã Python bị canh lề sai (indentation error)?
Đáp án: Python sẽ báo lỗi và không chạy chương trình

Đoạn code nào gọi hàm my_func()?
Đáp án: my_func()

Đồ thị Boxplot có thể được dùng với mục đích gì?
Đáp án: Phát hiện giá trị ngoại lai (outlier).

F
File "sales.csv" có dòng đầu tiên là tên cột. Lệnh nào hợp lý nhất để đọc nội dung file vào DataFrame df?
Đáp án: df = pd.read_csv("sales.csv")

File data.csv và dòng đầu tiên trong file không phải là tiêu đề cột. Bạn muốn Pandas tự tạo tên cột mặc định (0, 1, 2...). Lệnh nào sau đây là đúng?
Đáp án: pd.read_csv("data.csv", header=None)

for i in range(1, 5, 2): print(i, end=' ')
Đáp án: 1 3

G
Giả sử bạn cần tạo biểu đồ phân tích nguyên nhân doanh thu quý III tăng trưởng. Tiêu đề nào dưới đây phù hợp nhất với nguyên tắc "mỗi biểu đồ trả lời một câu hỏi"?
Đáp án: "Doanh thu quý III tăng mạnh nhờ nhóm khách hàng doanh nghiệp"

Giả sử bạn có một tệp tin hoặc chuỗi dữ liệu định dạng JSON chứa danh sách các sinh viên... Để chuyển đổi trực tiếp tập dữ liệu này thành một Pandas DataFrame, bạn nên sử dụng hàm nào?
Đáp án: pd.read_json

Giả sử bạn muốn dạy máy tính phân biệt giữa 'thư rác' và 'thư thường'... Đây là ví dụ của loại hình học máy nào?
Đáp án: Học có giám sát (Supervised Learning).

Giá trị của IQR (Interquartile Range) trong phương pháp chuẩn hóa dữ liệu RobustScaler được tính bởi công thức nào?
Đáp án: Q3 - Q1 (Phân vị 75% - Phân vị 25%).

Giá trị của result sau khi thực thi đoạn mã sau là gì? result = 1 for i in range ( 1 , 4 ): result*= i
Đáp án: 6

Gộp dataframe=merge, sử dụng index ở bên phải?
Đáp án: tham số right_index=True

H
Hàm fit() trong thư viện Scikit-learn thực hiện công việc gì?
Đáp án: Huấn luyện mô hình trên dữ liệu Train.

Hàm nào trong thư viện Pandas được dùng để ghi DataFrame df ra file JSON?
Đáp án: df.to_json()

Hàm np.linspace() khác với np.arange() ở điểm nào?
Đáp án: np.arange() dùng bước nhảy, np.linspace() dùng số lượng phần tử.

Hàm pd.to_datetime() thường được dùng để xử lý vấn đề gì?
Đáp án: Chuyển đổi cột dạng chuỗi (object) sang định dạng thời gian.

Hàm pd.to_datetime() thường được dùng để xử lý vấn đề gì?
Đáp án: Chuyển đổi cột dạng chuỗi (object) sang định dạng thời gian.

Hàm .predict() trong thư viện Scikit-learn thực hiện công việc gì?
Đáp án: Đưa ra dự đoán trên dữ liệu đầu vào.

Hiện tượng mô hình dự đoán sai nhiều ngay cả trên tập Train gọi là gì?
Đáp án: Dưới khớp (Underfitting).

K
Kết quả của df.isna().sum() là gì?
Đáp án: Số lượng dữ liệu thiếu theo từng cột

Kết quả của biến y là gì? (x = 7; y = 3; if x > 5: if x < 10: y = y + x else: y = y - x)
Đáp án: 10

Kết quả của đoạn code sau là gì? a = np.array([1, 2, 3]); print(a + 5)
Đáp án: [6, 7, 8]

Kết quả của đoạn code sau là gì? obj = pd.Series([4, 7, -5, 3]); print(obj.index)
Đáp án: RangeIndex(start=0, stop=4, step=1)

Kết quả của đoạn code sau trả về gì? df = pd.DataFrame({"a": [1,2,3], "b": [4,5,6]}); print(df["a"] > 1)
Đáp án: Series chứa các giá trị True/False

Kết quả của đoạn code sau: t=(1,2,3); t[1]=5; print(t)
Đáp án: Lỗi (TypeError)

Kết quả của đoạn code sau là gì?
import numpy as np 
a = np . array ([[ 1 , 2 ],[ 3 , 4 ]]) 
print ( a . sum ())
Đáp án: 10

Kết quả của đoạn mã sau là gì? def test(a, b=2): print(a + b); test(3)
Đáp án: 5

Kết quả của đoạn mã sau là gì? lst = [x for x in range(3)]; print(lst)
Đáp án: [0, 1, 2]

Kết quả của đoạn mã sau là gì? s = "hello"; t = s; s += "l"; print(s is t)
Đáp án: False

Kết quả của đoạn mã sau là gì? x = 10; while x >= 5: x -= 3; print(x)
Đáp án: 4

Kết quả của đoạn mã sau là gì? x = 3; if x < 5: x += 2; elif x < 10: x += 3; else: x += 4; print(x)
Đáp án: 5

Kết quả của đoạn mã sau là gì? x = [1, 2, 3, 4, 5]; print(x[-1])
Đáp án: 5

Kết quả của đoạn mã sau là gì? s = "abcdef" print ( s [ -2 :])
Đáp án: "ef"

Kết quả của đoạn mã sau là gì?
Đáp án: 0 1 0 1 2 0 1 2 3

Kết quả của đoạn mã sau là gì?
Đáp án: Lỗi

Kết quả của đoạn code sau trả về gì? 
import pandas as pd
df = pd.DataFrame({"a":[1,2,3], "b":[4,5,6]})
print(df["a"] > 1)
Đáp án: Series chứa các giá trị True/False.

Khi chuẩn hóa dữ liệu, tại sao cần fit scaler (ví dụ sử dụng phương thức MinMaxScaler trong thư viện Sklearn) trên tập huấn luyện thay vì toàn bộ tập dữ liệu?
Đáp số: Để tránh data leakage (tập dữ liệu huấn luyện chứa thông tin về mục tiêu cần dự đoán, nhưng thông tin tương tự không tồn tại khi triển khai thực tế.)

Khi dự đoán giá nhà, dữ liệu đầu vào được gọi là gì? và giá thực tế là gì?
Đáp án: Đầu vào: Đặc trưng (Features), Đầu ra: Nhãn (Labels)

Khi dữ liệu bị lệch trái/phải mạnh, ta nên dùng phương pháp xử lý dữ liệu nào sau đây?
Đáp án: Log transform.

Khi đồ thị lệch trái/phải mạnh, ta nên dùng phương pháp nào?
Đáp án: Log transform

Khi đọc dữ liệu từ API sử dụng thư viện requests, thuộc tính nào của đối tượng được trả về resp cho biết mã trạng thái HTTP?
Đáp án: resp.status_code

Khi đọc dữ liệu từ file JSON, một số object trong JSON thiếu key. Khi chuyển sang DataFrame, những ô thiếu key sẽ có giá trị gì?
Đáp án: NaN

Khi đọc file CSV, tham số nào của hàm read_csv() dùng để bỏ qua một số dòng đầu tiên trong file?
Đáp án: skiprows

Khi hai mảng có hình dạng không tương thích... phép cộng có thể thực hiện được nhờ cơ chế nào?
Đáp án: Broadcasting (Phát sóng).

Khi sử dụng phương thức concat trong thư viện Pandas, tham số axis dùng để chỉ định điều gì?
Đáp án: Trục mà theo đó các DataFrame được nối.

Khi sử dụng phương thức concat trong thư viện Pandas để ghép nhiều Series theo chiều ngang (axis=1), đối tượng được tạo ra là kiểu dữ liệu gì?
Đáp án: DataFrame

Khi sử dụng thư viện Scikit-learn cho Linear Regression, tại sao dữ liệu đầu vào X (Feature) thường cần được reshape thành dạng mảng 2 chiều (ví dụ: cột dọc)?
Đáp án: Để tuân thủ quy ước ma trận: mỗi hàng là một mẫu dữ liệu, mỗi cột là một đặc trưng.

Khi xử lý dữ liệu JSON có cấu trúc phức tạp và nhiều cấp lồng nhau... tại sao việc sử dụng hàm pd.json_normalize() lại được ưu tiên?
Đáp án: Vì json_normalize giúp duỗi phẳng cấu trúc lồng nhau thành cột.

Khi file "file.xlsx" có nhiều trang tính (sheet) thì lệnh pd.read_excel("file.xlsx") sẽ trả về nội dung trang tính nào?
Đáp án; Trang đầu tiên

Kiểu dữ liệu set trong Python có đặc điểm nào sau đây?
Đáp án: Không cho phần tử trùng lặp.

Kỹ năng nào là kỹ năng quan trọng nhất đối với một kỹ sư dữ liệu?
Đáp án: SQL và Python.

Kỹ thuật điền giá trị thiếu bằng KNN Imputer dựa trên:
Đáp án: Sự tương đồng giữa các mẫu.

Kỹ thuật Web Scraping là giải pháp phù hợp khi gặp tình huống nào?
Đáp án: Khi cần trích xuất dữ liệu từ các trang web không hỗ trợ API.

Kỹ thuật small multiples hỗ trợ tốt nhất cho mục đích nào?
Đáp án: So sánh nhiều nhóm mà không gây chồng chéo.

L
Label Encoding chuyển đổi đặc trưng phân loại (categorical) thành gì?
Đáp án: Số nguyên tuần tự (0, 1, 2,...)

Làm sạch dữ liệu bắt đầu bằng bước?
Đáp án: Khám phá và hiểu dữ liệu (EDA).

Lệnh kiểm tra kiểu dữ liệu của biến x trong Python là gì?
Đáp án: type(x)

Lệnh nào dùng để thiết lập chế độ hiển thị đồ thị trực tiếp trong Jupyter Notebook?
Đáp án: %matplotlib inline

Lệnh nào sau đây của Python giúp xem các thống kê cơ bản... của các đặc trưng số của DataFrame df?
Đáp án: df.describe()

Lệnh s = pd.Series(5, index=['a', 'b', 'c']) sẽ tạo ra Series s như thế nào?
Đáp án: Series với các giá trị [5, 5, 5] và chỉ số ['a', 'b', 'c'].

Lệnh get.dummies() dùng làm gì
Đáp án: one-hot encoding

Loại biểu đồ nào để phát hiện và trực quan hóa ngoại lai của dữ liệu một cách hiệu quả nhất?
Đáp án: Boxplot

M
Matplotlib, hiển thị lưới grid như thế nào?
Đáp án: Tham số grid (hoặc lệnh plt.grid()).

Máy tính tự động gom các bài báo có nội dung tương tự nhau thành các nhóm mà không hề cho máy biết trước chủ đề. Đây là bài toán:
Đáp án: Học không giám sát (Unsupervised Learning)

Một bác sĩ muốn nghiên cứu mối liên hệ giữa Chỉ số khối cơ thể (BMI) và Mức đường huyết của bệnh nhân... Biểu đồ nào phù hợp nhất?
Đáp án: Scatter Plot (Biểu đồ phân tán).

Một cột dữ liệu phân loại có quá nhiều giá trị duy nhất (High Cardinality). Giải pháp nào là hiệu quả nhất?
Đáp án: Nhóm các giá trị ít xuất hiện vào một nhóm.

Một dấu hiệu phổ biến của data leakage trong việc huấn luyện mô hình học máy là gì?
Đáp án: Độ chính xác (accuracy) quá cao trên tập đánh giá (test).

Một ngân hàng muốn đánh giá rủi ro tín dụng của các khách hàng mới. Để làm điều này, nhà phân tích cần hiểu rõ phân phối của điểm tín dụng... Loại biểu đồ nào là phù hợp?
Đáp án: Histogram.

Một nhà phân tích cần tạo báo cáo để so sánh tỷ lệ sinh viên theo từng Khoa (A, B, C) cho mỗi năm học (1, 2, 3, 4) trong một Câu lạc bộ (CLB). Đồng thời, báo cáo cũng cần trực quan hóa rõ ràng tổng số sinh viên của CLB không thay đổi qua các năm. Loại trực quan hóa nào là phù hợp nhất để thể hiện cả thành phần (tỷ lệ Khoa) và tổng thể (Tổng số sinh viên) trong cùng một hình?
Đáp án: Stacked bar chart.

Mô hình phân tích trong kinh tế - kinh doanh cần đảm bảo điều gì ngoài độ chính xác?
Đáp án: Khả năng giải thích kết quả và tính minh bạch của dữ liệu sử dụng.

Mục đích của mã hóa dữ liệu phân loại (Categorical) là gì?
Đáp án: Chuyển dữ liệu text sang dạng số.

Mục đích của xử lý giá trị thiếu (Data Imputation) là gì?
Đáp án: Tăng tính đầy đủ và nhất quán.

Mục tiêu của việc chia nhánh (splitting) trong cây quyết định là gì?
Đáp án: Tạo ra các nhóm con 'tỉnh khiết' (pure) hơn, tức là chứa các dữ liệu giống nhau nhiều hơn.

Mutilindex dùng cho trục dọc hay ngang hay cả 2
Đáp án: cả 2

N
Nếu bạn muốn mô hình 'khắt khe' hơn trong việc dự báo (chỉ báo 'Có' khi cực kỳ chắc chắn), bạn nên làm gì với ngưỡng (threshold)?
Đáp án: Tăng lên cao (ví dụ 0.9).

Nguyên nhân chính dẫn đến Overfitting là gì?
Đáp án: Mô hình quá phức tạp, học cả nhiễu của dữ liệu.

Nhược điểm chính của phương pháp mã hóa Label Encoding với dữ liệu Nominal là gì?
Đáp án: Tạo thứ tự giả tạo khiến thuật toán hiểu sai.

Nhược điểm lớn nhất của KNN khi tập dữ liệu rất lớn là gì?
Đáp án: Tốc độ dự đoán rất chậm.

Np.dot -> nhân ma trận

P
Phát biểu nào đúng về One-Hot Encoding?
Đáp án: Phù hợp cho biến phân loại không thứ tự.

Phân tích dữ liệu giúp bước xác định bài toán trong dự án Data Science như thế nào?
Đáp án: Cung cấp các thông tin sơ bộ (Insights) để định hướng đi đúng đắn.

Phân tích chẩn đoán (Diagnostic Analytics) tập trung vào điều gì?
Đáp án: Tìm nguyên nhân của các hiện tượng đã xảy ra.

Phương pháp điền giá trị thiếu (Data Imputation) bằng trung vị thường hiệu quả hơn bằng giá trị trung bình khi nào?
Đáp án: Dữ liệu có nhiều giá trị ngoại lai (outliers).

Phương thức nào dùng để xem 5 dòng đầu tiên của một DataFrame?
Đáp án: df.head()

Phương thức pop trong thư viện Pandas trên một DataFrame thực hiện chức năng nào sau đây?
Đáp án: Trả về một cột được chỉ định đồng thời xóa cột đó khỏi DataFrame.

Phương thức nào dùng để kiểm tra từng phần tử có thiếu dữ liệu không?
Đáp án: isna() hoặc isnull()

Phương thức unstack trong thư viện Pandas được sử dụng để thực hiện thao tác gì trên dữ liệu của một DataFrame?
Đáp án: Chuyển hàng thành cột.

Q
Quyết định cắt trục Y (Truncated Y-axis), bắt đầu từ giá trị 90% thay vì 0%. Hành động này đã vi phạm nguyên tắc thiết kế trực quan hóa nào?
Đáp án: Trung thực (Truthful).

Quy trình làm việc có hệ thống giúp ích gì cho dự án dữ liệu?
Đáp án: Biến dữ liệu thô thành thông tin có giá trị.

S
Sản phẩm đầu ra chính của một Data Engineer là gì?
Đáp án: Một hệ thống kho dữ liệu sạch, tin cậy và sẵn sàng cho việc phân tích.

Sử dụng KNN trên tập train, sai số sẽ như thế nào?
Đáp án: Bằng 0

Sử dụng Python để tạo một Series từ thư viện (dictionary) dicta = {"Ohio": 35000, "Texas": 71000} ta sử dụng lệnh nào?
Đáp án: pd.Series(dicta)

T
Tại sao không nên dùng Linear Regression cho bài toán phân loại nhị phân (0/1)?
Đáp án: Vì đầu ra của nó có thể lớn hơn 1 hoặc nhỏ hơn 0, không có ý nghĩa xác suất.

Tại sao chỉ sở hữu dữ liệu là chưa đủ để tạo ra lợi thế cạnh tranh?
Đáp án: Vì dữ liệu thô chưa mang lại giá trị nếu thiếu quá trình xử lý và tư duy phân tích để khai thác tri thức.

Tại sao hiếm khi MSE bằng 0 trên tập huấn luyện đối với Linear Regression?
Đáp án: Vì dữ liệu thực tế thường có nhiễu và không bao giờ nằm thẳng hàng tuyệt đối.

Tại sao Linear Regression rất nhạy cảm với các điểm dữ liệu ngoại lai (outliers) có giá trị quá lớn?
Đáp án: Vì nó dùng bình phương sai số (MSE), sai số lớn từ outlier sẽ bị phóng đại lên, kéo lệch đường thẳng.

Tại sao một mô hình có độ chính xác rất cao (chẳng hạn 99%) trên tập kiểm tra (test set) nhưng lại thất bại khi triển khai thực tế?
Đáp án: Vì tập dữ liệu huấn luyện không đại diện cho thực tế.

Tạo list rỗng như thế nào?
Đáp án: list() hoặc []

Tập Test (Kiểm tra) được sử dụng khi nào?
Đáp án: Sau khi huấn luyện xong, dùng để đánh giá hiệu suất mô hình.

Theo các nguyên tắc thiết kế trực quan hóa dữ liệu hiệu quả, lý do chính khiến việc sử dụng biểu đồ 3D thường bị hạn chế là gì?
Đáp án: Làm mất tính chính xác và khó so sánh.

Thư viện nào thường dùng với Pandas để làm việc với file .xlsx?
Đáp án: openpyxl

Tình huống nào thích hợp nhất để sử dụng biểu đồ thanh ngang plot.barh() thay cho plot.bar()?
Đáp án: Khi có nhiều danh mục với tên dài.

Trong bài toán cảnh báo ung thư sớm, việc bỏ sót người bệnh (False Negative) là không thể chấp nhận. Bạn nên ưu tiên tối ưu chỉ số nào?
Đáp án: Recall (Độ nhạy).

Trong bài toán dự đoán giá nhà bằng mô hình linear regression, nếu hệ số β của biến 'Khoảng cách đến trung tâm' là số âm, điều này có ý nghĩa gì?
Đáp án: Nhà càng xa trung tâm thì giá càng giảm.

Trong bài toán phân loại (Classification), các chỉ số đánh giá mô hình được sử dụng phổ biến là gì?
Đáp án: Độ chính xác (Accuracy), Precision, Recall và F1-Score.

Trong bước tiền xử lý và làm sạch dữ liệu, khi nào nên xóa cột có nhiều giá trị thiếu?
Đáp án: Tỷ lệ thiếu > 50% và cột đó không chứa thông tin quan trọng.

Trong bước xử lý dữ liệu, phân tích dữ liệu đóng vai trò gì?
Đáp án: Đánh giá chất lượng dữ liệu và đề xuất phương án xử lý sai sót.

Trong cấu trúc DataFrame của Pandas, index (chỉ mục) là gì?
Đáp án: Các nhãn dùng để xác định và truy cập các hàng dữ liệu.

Trong ngôn ngữ Python, mục đích của việc sử dụng các hàm như np.sqrt, np.exp, np.log là gì?
Đáp án: Thực hiện các phép toán trên toàn bộ mảng mà không cần vòng lặp.

Trong Python, điều gì sẽ xảy ra nếu không có khối else trong cấu trúc if?
Đáp án: Không làm gì khi điều kiện không thỏa mãn.

Trong Python, khi thực hiện câu lệnh df.loc[5] với DataFrame df, điều kiện để lệnh hoạt động là gì?
Đáp án: Index phải chứa nhãn (label) bằng 5.

Trong Python, lệnh kiểm tra "a" có phải là một key trong dictionary d là gì?
Đáp án: "a" in d

Trong Python, mệnh đề else trong cấu trúc for được thực hiện khi nào?
Đáp án: Khi vòng lặp kết thúc bình thường, không bị dừng bởi break.

Trong Python, phương thức melt() của DataFrame được sử dụng cho mục đích nào?
Đáp án: Chuyển đổi dữ liệu từ dạng rộng sang dạng dài.

Trong Python, phương thức pivot() của DataFrame được sử dụng cho mục đích nào?
Đáp án: Chuyển đổi dữ liệu từ dạng dài sang dạng rộng.

Trong Python, toán tử is dùng để làm gì?
Đáp án: Kiểm tra xem hai biến có tham chiếu cùng một đối tượng hay không.

Trong quản lý chuỗi cung ứng, để so sánh sự phân tán của mức tồn kho và nhận diện các giá trị ngoại lai... loại biểu đồ nào phù hợp nhất?
Đáp án: Boxplot

Trong quy trình Khoa học dữ liệu, vai trò trung tâm của dữ liệu là gì?
Đáp án: Là nguyên liệu đầu vào để trích xuất tri thức, hỗ trợ ra quyết định.

Trong thư viện Matplotlib, để tạo một biểu đồ tròn (pie chart), bạn sử dụng phương thức nào?
Đáp án: plt.pie()

Trong thư viện Matplotlib, nếu bạn muốn đặt nhãn (label) cho trục X của biểu đồ, bạn cần sử dụng phương thức nào?
Đáp án: set_xlabel() (hoặc plt.xlabel())

Trong thư viện Matplotlib, phương thức nào để tùy chỉnh nhãn tick trên trục x?
Đáp án: plt.xticks()

Trong thư viện Matplotlib, phương thức subplots_adjust() được sử dụng cho mục đích chính nào liên quan đến bố cục biểu đồ?
Đáp án: Điều chỉnh khoảng cách giữa các subplot.

Trong thư viện Matplotlib, tham số color (hay c) của hàm vẽ biểu đồ dùng để làm gì?
Đáp án: Đặt màu sắc cho biểu đồ.

Trong thư viện pandas (Python), hàm sort_index(level=...) được dùng trong trường hợp nào?
Đáp án: Sắp xếp theo một cấp cụ thể của MultiIndex.

Trong thư viện pandas (Python), thuộc tính hàm index.levels dùng để làm gì?
Đáp án: Xác định số cấp của chỉ số.

Trong thư viện pandas (Python), phương thức combine_first thường được dùng trong tình huống nào?
Đáp án: Khi bạn kết hợp hai bảng có cấu trúc tương tự, điền các giá trị thiếu (NaN) trong bảng này bằng các giá trị có sẵn tương ứng trong bảng kia.

Trong thư viện pandas (Python), sau khi thực hiện các phép biến đổi, nhãn của các hàng trong DataFrame df bị xáo trộn. Bạn muốn sắp xếp lại DataFrame df dựa trên các nhãn của chỉ số (index). Hàm nào sau đây thực hiện thao tác trên?
Đáp án: df.sort_index()

Trong thư viện pandas (Python), thuộc tính hàm index.levels dùng để làm gì?
Đáp án: Xác định số cấp của chỉ số.

Trong thư viện pandas, giả sử bạn đã có một DataFrame df. Để thống kê chính xác tổng số lượng các giá trị bị thiếu hiện có trong từng cột dữ liệu, bạn nên sử dụng tổ hợp lệnh nào?
Đáp án: df.isnull().sum()

Trong thư viện pandas, lệnh df['col'].str.contains('abc') trả về dữ liệu kiểu gì?
Đáp án: Boolean

Trong thư viện Pandas (Python), sau khi dùng hàm reset_index(), index cũ sẽ được xử lý thế nào?
Đáp án: Trở thành một cột dữ liệu.

Trong thư viện Pandas (Python), với DataFrame df, điểm khác biệt chính giữa phương thức df.stack() và hàm pd.melt() là gì?
Đáp án: df.stack() chuyển cột vào trục chỉ số (tạo MultiIndex), còn pd.melt() chuyển cột thành các hàng dữ liệu mới.

Trong thư viện Pandas, giá trị nào được sử dụng để biểu diễn dữ liệu thiếu cho kiểu số?
Đáp án: NaN

Trong thư viện Pandas, khi dùng các hàm thống kê như sum() và mean() thì tham số axis=1 có ý nghĩa gì?
Đáp án: Tính toán theo chiều ngang, tức theo từng hàng.

Trong thư viện Pandas, khi dùng các hàm thống kê như sum() và mean() thì tham số axis=0 có ý nghĩa gì?
Đáp án: Tính toán theo chiều dọc, tức theo từng cột.

Trong thư viện Pandas, khi dùng hàm merge() với tham số how="inner", kết quả gộp dữ liệu sẽ như thế nào?
Đáp án: Chỉ giữ các dòng có khóa xuất hiện ở cả hai DataFrame.

Trong trực quan hóa dữ liệu với thư viện Matplotlib, tình huống nào thích hợp nhất để sử dụng biểu đồ thanh ngang plot.barh() thay thế cho biểu đồ thanh đứng plot.bar()?
Đáp án: Khi có nhiều danh mục với tên dài.

Trong thư viện Pandas (Python), với DataFrame df, điểm khác biệt chính giữa phương thức df.stack() và hàm pd.melt() là gì?
Đáp án: df.stack() chuyển cột vào trục chỉ số (tạo MultiIndex), còn pd.melt() chuyển cột thành các hàng dữ liệu mới.

Trong thư viện pandas (Python), sau khi dùng hàm reset_index(), index cũ sẽ được xử lý thế nào?
Đáp án: Trở thành một cột dữ liệu.

Trong tiền xử lý dữ liệu, với dữ liệu có đặc trưng thứ tự {Low, Medium, High}, phương pháp mã hóa phù hợp nhất cho đặc trưng này là gì?
Đáp án: Label encoding.

Trong việc đánh giá mô hình cho bài toán phân loại. Mô hình A có Accuracy 95% nhưng F1-Score thấp. Mô hình B có Accuracy 90% nhưng F1-Score cao. Nếu dữ liệu bị mất cân bằng (Imbalanced), bạn nên tin tưởng mô hình nào hơn?
Đáp án: Mô hình B

Trong việc đánh giá mô hình cho bài toán hồi quy. Giá trị thực tế là [10, 20], giá trị dự đoán là [12, 19]. Tính MSE?
Đáp án: 2.5

Trong việc đánh giá mô hình cho bài toán hồi quy, tại sao MAE (Mean Absolute Error) lại ít bị ảnh hưởng bởi nhiễu (outliers) hơn so với MSE?
Đáp án: Vì MAE chỉ lấy trị tuyệt đối.

Trong Pandas, với DataFrame df, lệnh df.set_index("col") thực hiện điều gì?
Đáp án: Gán cột "col" thành index.

V
Vai trò chính của kỹ sư dữ liệu là gì?
Đáp án: Thiết kế và duy trì hạ tầng dữ liệu.

Việc thiếu kiến thức chuyên môn khi thực hiện một dự án liên quan tới dữ liệu có thể dẫn đến vấn đề gì?
Đáp án: Diễn giải sai ý nghĩa của dữ liệu hoặc đưa ra kết luận vô nghĩa.

Vòng lặp while trong Python sẽ dừng khi nào?
Đáp án: Khi điều kiện lặp trở thành False.

Với cột “Giới tính” gồm các giá trị: “Nam”, “Nữ”, “Không xác định”,  phương pháp mã hóa One-Hot Encoding tạo ra bao nhiêu cột?
Đáp án: 3 cột

Với DataFrame df, lệnh nào chọn hàng có cột A > 2 và cột B < 5 điều kiện nhiều cột?
Đáp án: df[(df.A > 2) & (df.B < 5)]

Với DataFrame df , lệnh nào không hợp lệ?
df.iloc[1:3, 'A']

Với DataFrame df , lệnh nào không thể dùng để truy cập nhiều cột?
Đáp án: df.get('A','B')

Với DataFrame df gồm các cột ‘A’ đến ‘E’. Lệnh nào chọn cột 'A' và 'C' bằng vị trí?
Đáp án: df.iloc[:, [0,2]]

Với s = pd.Series([10,20,30], index=["a","b","c"]), thì s["b"] sẽ trả về giá trị là gì?
Đáp án: 20

Y
Yếu tố nào sau đây không phải là trụ cột chính của Khoa học dữ liệu?
Đáp án: Quản lý nhân sự.

Z
Z Score có mean, std =?
Đáp án: 0, 1

Câu hỏi thêm:

1. x="Python", x[2:5] in ra gì?
Đáp án: "tho"

2. Biểu đồ Violin là gì?
Đáp án & Đặc điểm: Biểu đồ Violin (Violin plot) là sự kết hợp giữa biểu đồ hộp (Boxplot) và biểu đồ mật độ (Kernel Density Plot).

3. Các ngành nghề này có vai trò gì? (Trong bối cảnh Khoa học Dữ liệu)

Kỹ sư dữ liệu (Data Engineer): Xây dựng hạ tầng, đường ống (pipeline) để thu thập, lưu trữ và làm sạch dữ liệu từ nhiều nguồn. (Người lo phần nền tảng).

Chuyên viên phân tích dữ liệu (Data Analyst): Lấy dữ liệu đã sạch để trực quan hóa, làm báo cáo/dashboard và tìm ra các insight cơ bản giúp doanh nghiệp ra quyết định.

Nhà khoa học dữ liệu (Data Scientist): Sử dụng toán học, thống kê và Machine Learning để xây dựng các mô hình dự đoán tương lai hoặc phân loại nâng cao.

4. Thư viện nào dùng cùng requests đọc file trong RSS XML?
Đáp án: Chính xác như gợi ý trong câu hỏi của bạn là BeautifulSoup (thường dùng chung với parser xml hoặc lxml).

5. Biểu đồ cột chồng (Stacked bar chart) có đặc điểm gì?
Đáp án: Biểu đồ cột chồng giúp hiển thị đồng thời tổng độ lớn của một hạng mục và thành phần cấu tạo bên trong hạng mục đó.

6. Khôi phục dữ liệu sau khi unstack dùng gì?
Đáp án: Dùng hàm stack()

7. Cộng series s1 và s2 thì ra kết quả gì như nào?
Đáp án: Kết quả là một Series mới, trong đó Pandas sẽ tự động cộng các giá trị có cùng nhãn chỉ mục (index) với nhau.

8. Hàm map() dùng với kiểu dữ liệu nào?
Đáp án: * Trong Python cơ bản: map() dùng với các Iterable (đối tượng có thể lặp) như List, Tuple, Set.

10. Tham số how khi dùng với pd.merge có ý nghĩa gì?
Đáp án: Nó xác định cách thức kết nối (Join type) giữa 2 DataFrame, tương tự như SQL. Các giá trị phổ biến gồm:

11. Dữ liệu nào là bán cấu trúc (Semi-structured data)?
Đáp án: Các định dạng phổ biến nhất là JSON, XML, HTML, hoặc dữ liệu trong các cơ sở dữ liệu NoSQL (như MongoDB).

12. Đặc điểm dữ liệu XML?
Đáp án: XML (Extensible Markup Language) sử dụng cấu trúc cây phân cấp được tạo ra bởi các thẻ (tags) tự định nghĩa.

13. Numpy có cho chứa các dữ liệu có kiểu khác nhau không?
Đáp án: Về bản chất là KHÔNG (nếu muốn tối ưu hiệu suất).

14.One Hot encoding có làm tăng số cột lên không?
Đáp án: Có

15. Cứ tuyến tính + thời gian thì là đường thẳng

16. Có chữ “tỷ lệ” thì chọn stacked bar

17. Đa phần liên quan tới outliers thì sẽ là scatter plot
