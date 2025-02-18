### Độ Lệch Chuẩn

Độ lệch chuẩn (Standard Deviation) là một đại lượng thống kê đo lường mức độ phân tán của một tập dữ liệu so với giá trị trung bình của nó. Công thức tính độ lệch chuẩn như sau:



***Độ Lệch Chuẩn Mẫu (Sample Standard Deviation)***

$$
s = \sqrt{\frac{1}{n-1} \sum_{i=1}^{n} (x_i - \overline{x})^2}
$$

***Độ Lệch Chuẩn Tổng Thể (Population Standard Deviation)***

$$
\sigma = \sqrt{\frac{1}{N} \sum_{i=1}^{N} (x_i - \mu)^2}
$$

**Với**

- $i$: Chỉ số phần tử trong tập dữ liệu

- $s$: Độ lệch chuẩn mẫu
- $\sigma$: Độ lệch chuẩn tổng thể
- $n$: Số lượng mẫu
- $N$: Số lượng phần tử trong tổng thể
- $x_i$: Giá trị của phần tử thứ $i$
- $\overline{x}$: Giá trị trung bình mẫu
- $\mu$: Giá trị trung bình tổng thể

**Ví Dụ**: Cho một tập dữ liệu mẫu: **[2, 4, 4, 4, 5, 5, 7, 9]**

1. Tính giá trị trung bình mẫu $\overline{x}$:

$$\overline{x} = \frac{2 + 4 + 4 + 4 + 5 + 5 + 7 + 9}{8} = 5$$

2. Tính các giá trị $(x_i - \overline{x})^2$:

$$(2-5)^2, (4-5)^2, (4-5)^2, (4-5)^2, (5-5)^2, (5-5)^2, (7-5)^2, (9-5)^2$$
$$= 9, 1, 1, 1, 0, 0, 4, 16$$

3. Tính tổng các giá trị trên và chia cho $n-1$:

$$\frac{9 + 1 + 1 + 1 + 0 + 0 + 4 + 16}{7} = \frac{32}{7} \approx 4.57$$

4. Lấy căn bậc hai của kết quả trên để có độ lệch chuẩn mẫu:

$$s \approx \sqrt{4.57} \approx 2.14$$

Vậy **độ lệch chuẩn mẫu của tập dữ liệu** trên là khoảng ***2.14***.

---

### Độ Tương Đồng Cosine

Độ tương đồng Cosine (Cosine Similarity) là một thước đo để đánh giá mức độ tương tự giữa hai vector trong không gian vector. Công thức tính độ tương đồng Cosine như sau:

$$
\text{Cosine Similarity} = \cos(\theta) = \frac{\mathbf{A} \cdot \mathbf{B}}{\|\mathbf{A}\| \|\mathbf{B}\|}
$$

**Với**

- $\mathbf{A} \cdot \mathbf{B}$: Tích vô hướng của hai vector $\mathbf{A}$ và $\mathbf{B}$
- $\|\mathbf{A}\|$: Độ dài (norm) của vector $\mathbf{A}$
- $\|\mathbf{B}\|$: Độ dài (norm) của vector $\mathbf{B}$
- $\cos(\theta)$: Giá trị cosine của góc giữa hai vector $\mathbf{A}$ và $\mathbf{B}$

**Ví Dụ**: Cho hai vector $\mathbf{A}$ và $\mathbf{B}$ như sau:

$$
\mathbf{A} = [1, 2, 3]
$$

$$
\mathbf{B} = [4, 5, 6]
$$

1. Tính tích vô hướng $\mathbf{A} \cdot \mathbf{B}$:

$$
\mathbf{A} \cdot \mathbf{B} = 1 \cdot 4 + 2 \cdot 5 + 3 \cdot 6 = 4 + 10 + 18 = 32
$$

2. Tính độ dài của vector $\mathbf{A}$:

$$
\|\mathbf{A}\| = \sqrt{1^2 + 2^2 + 3^2} = \sqrt{1 + 4 + 9} = \sqrt{14}
$$

3. Tính độ dài của vector $\mathbf{B}$:

$$
\|\mathbf{B}\| = \sqrt{4^2 + 5^2 + 6^2} = \sqrt{16 + 25 + 36} = \sqrt{77}
$$

4. Tính độ tương đồng Cosine:

$$
\text{Cosine Similarity} = \frac{32}{\sqrt{14} \cdot \sqrt{77}} = \frac{32}{\sqrt{1078}} \approx 0.9746
$$

**Kết luận**

Độ tương đồng Cosine giữa hai vector $\mathbf{A}$ và $\mathbf{B}$ là khoảng 0.9746, cho thấy hai vector này khá tương tự nhau.

---
### Độ Đo Proximity cho thuộc tính nomial

Độ proximity (gần gũi) đối với thuộc tính nomial của dữ liệu có thể được tính bằng công thức sau:

$$
d(i, j) = \frac{p - m}{p}
$$

**Với**

- $d(i, j)$: Độ proximity giữa hai phần tử $i$ và $j$. Giá trị của $d(i, j)$ càng tiến về 1 $\rightarrow$ Hai đối tượng đang xét càng khác nhau và ngược lại
- $p$: Tổng số thuộc tính nomial được so sánh giữa 2 đối tượng $i$ và $j$
- $m$: Số thuộc tính mà $i$ và $j$ giống nhau


**Ví Dụ**: Có hai phần tử với các thuộc tính như sau:

<center>

| Đối tượng | Màu sắc | Loại xe | Hãng xe | Xuất xứ |
| --- | --- | --- | ---- | ---- |
| A | Đỏ | Sedan | Toyota | JP | 
| B | Xanh | SUV | Toyota | USA | 
| C | Đỏ | Sedan | Hodan | JP | 

</center>

**So sánh giữa đối tượng A và B**

1. Tổng số thuộc tính so sánh $p$ là 4.
2. Số thuộc tính giống nhau $m$ là 1 (**Hãng xe**).

Áp dụng công thức:

$$
d(i, j) = \frac{4 - 1}{4} = \frac{1}{4} = 0.75 
$$

**So sánh giữa đối tượng A và C**

1. Tổng số thuộc tính so sánh $p$ là 4.
2. Số thuộc tính giống nhau $m$ là 3 (**Màu sắc**, **Loại Xe**, **Xuất xứ**).

Áp dụng công thức:

$$
d(i, j) = \frac{4 - 3}{4} = \frac{1}{4} = 0.25 
$$

**Kết luận**

$d(A, B) = 0.75 \rightarrow$ $A$ và $B$ có độ khác biết cao

$d(A, C) = 0.25 \rightarrow$ $A$ và $C$ tương tự nhau hơn

---

### Độ Đo Proximity cho thuộc tính binary

Độ proximity (gần gũi) đối với thuộc tính binary của dữ liệu có thể được tính bằng công thức sau:

$$
d(i, j) = \frac{r + s}{q + r + s + t}
$$

**Với**

- $d(i, j)$: Độ proximity giữa hai phần tử $i$ và $j$
- $q$: Số thuộc tính mà cả $i$ và $j$ đều có giá trị 1
- $r$: Số thuộc tính mà $i$ có giá trị 1 và $j$ có giá trị 0
- $s$: Số thuộc tính mà $i$ có giá trị 0 và $j$ có giá trị 1
- $t$: Số thuộc tính mà cả $i$ và $j$ đều có giá trị 0

<center>

| | j = 1 | j = 0 
| --- | --- | ---- |
| **i = 1** | q | r |
| **i = 0** | s | t |

</center>

**Ví Dụ**: Có hai phần tử với các thuộc tính binary như sau:

<center>

| Đối tượng | Thuộc tính 1 | Thuộc tính 2 | Thuộc tính 3 | Thuộc tính 4 |
| --- | --- | --- | ---- | ---- |
| A | 1 | 0 | 1 | 0 | 
| B | 0 | 1 | 1 | 0 | 

</center>

**So sánh giữa đối tượng A và B**

1. Số thuộc tính mà cả $A$ và $B$ đều có giá trị 1 ($q$) là 1.
2. Số thuộc tính mà $A$ có giá trị 1 và $B$ có giá trị 0 ($r$) là 1.
3. Số thuộc tính mà $A$ có giá trị 0 và $B$ có giá trị 1 ($s$) là 1.
4. Số thuộc tính mà cả $A$ và $B$ đều có giá trị 0 ($t$) là 1.

Áp dụng công thức:

$$
d(i, j) = \frac{r + s}{q + r + s + t} = \frac{1 + 1}{1 + 1 + 1 + 1} = \frac{2}{4} = 0.5
$$

**Kết luận**

$d(A, B) = 0.5 \rightarrow$ $A$ và $B$ có độ khác biệt trung bình

**Khi nào dùng công thức này?**
- Dữ liệu binary đối xứng (0 và 1 đều quan trọng như nhau)
- Cần đo lường tỷ lệ thuộc tính khác nhau giữa hai đối tượng

Nếu như làm việc với dữ liệu binary không đối xứng (khi 1 quan trọng hơn 0, ví dụ dữ liệu bệnh tật hoặc lỗi phần mềm) thì nên dùng **Jaccard distance**:

$$d_J(i, j) = \frac{r + s}{q +r + s}$$

--- 

### Độ Đo Proximity cho thuộc tính numeric

Độ proximity (gần gũi) đối với thuộc tính numeric của dữ liệu có thể được tính bằng các công thức sau:

#### Khoảng cách Euclidean

Khoảng cách Euclidean giữa hai điểm $i$ và $j$ trong không gian $n$ chiều được tính bằng công thức:

$$
d_E(i, j) = \sqrt{\sum_{k=1}^{n} (x_{ik} - x_{jk})^2}
$$

**Với**

- $d_E(i, j)$: Khoảng cách Euclidean giữa hai điểm $i$ và $j$
- $x_{ik}$: Giá trị của thuộc tính thứ $k$ của điểm $i$
- $x_{jk}$: Giá trị của thuộc tính thứ $k$ của điểm $j$

#### Khoảng cách Manhattan

Khoảng cách Manhattan giữa hai điểm $i$ và $j$ trong không gian $n$ chiều được tính bằng công thức:

$$
d_M(i, j) = \sum_{k=1}^{n} |x_{ik} - x_{jk}|
$$

**Với**

- $d_M(i, j)$: Khoảng cách Manhattan giữa hai điểm $i$ và $j$
- $x_{ik}$: Giá trị của thuộc tính thứ $k$ của điểm $i$
- $x_{jk}$: Giá trị của thuộc tính thứ $k$ của điểm $j$

#### Khoảng cách Minkowski

Khoảng cách Minkowski giữa hai điểm $i$ và $j$ trong không gian $n$ chiều với tham số $p$ được tính bằng công thức:

$$
d_{M_p}(i, j) = \left( \sum_{k=1}^{n} |x_{ik} - x_{jk}|^p \right)^{\frac{1}{p}}
$$

or

$$
d_{M_p}(i, j) = \sqrt[p]{\sum_{k=1}^{n} |x_{ik} - x_{jk}|^p}
$$

**Với**

- $d_{M_p}(i, j)$: Khoảng cách Minkowski giữa hai điểm $i$ và $j$ với tham số $p$
- $x_{ik}$: Giá trị của thuộc tính thứ $k$ của điểm $i$
- $x_{jk}$: Giá trị của thuộc tính thứ $k$ của điểm $j$
- $p$: Tham số điều chỉnh khoảng cách (khi $p = 1$ là khoảng cách Manhattan, khi $p = 2$ là khoảng cách Euclidean)

**Ví Dụ**: Có hai điểm với các thuộc tính numeric như sau:

<center>

| Đối tượng | Thuộc tính 1 | Thuộc tính 2 | Thuộc tính 3 |
| --- | --- | --- | ---- |
| A | 1 | 2 | 3 | 
| B | 4 | 5 | 6 | 

</center>

**Khoảng cách Euclidean giữa A và B**

$$
d_E(A, B) = \sqrt{(1-4)^2 + (2-5)^2 + (3-6)^2} = \sqrt{9 + 9 + 9} = \sqrt{27} \approx 5.20
$$

**Khoảng cách Manhattan giữa A và B**

$$
d_M(A, B) = |1-4| + |2-5| + |3-6| = 3 + 3 + 3 = 9
$$

**Khoảng cách Minkowski giữa A và B với $p = 3$**

$$
d_{M_3}(A, B) = \left( |1-4|^3 + |2-5|^3 + |3-6|^3 \right)^{\frac{1}{3}} = \left( 27 + 27 + 27 \right)^{\frac{1}{3}} = \left( 81 \right)^{\frac{1}{3}} \approx 4.33
$$

**Kết luận**

- Khoảng cách Euclidean: 5.20
- Khoảng cách Manhattan: 9
- Khoảng cách Minkowski (với $p = 3$): 4.33

---
### Độ Đo Proximity cho thuộc tính ordinal

Độ proximity (gần gũi) đối với thuộc tính ordinal của dữ liệu có thể được tính bằng công thức sau:

$$
Z_{if} = \frac{r_{if} - 1}{M_f - 1}
$$

**Với**

- $Z_{if}$: Giá trị chuẩn hóa của thuộc tính ordinal $f$ của đối tượng $i$
- $r_{if}$: Thứ hạng của thuộc tính ordinal $f$ của đối tượng $i$
- $M_f$: Số lượng thứ hạng có thể có của thuộc tính ordinal $f$

**Ví Dụ**: Có ba đối tượng với các thuộc tính ordinal như sau:

<center>

| Đối tượng | Thuộc tính 1 (Rất kém, Kém, Trung bình, Tốt, Rất tốt) | Thuộc tính 2 (Thấp, Trung bình, Cao) | Thuộc tính 3 (Nhỏ, Vừa, Lớn) |
| --- | --- | --- | ---- |
| A | Trung bình | Cao | Vừa |
| B | Tốt | Trung bình | Lớn |
| C | Kém | Thấp | Nhỏ |

</center>

***Chuyển đổi các thuộc tính ordinal thành thứ hạng***

<center>

| Đối tượng | Thuộc tính 1 (1-5) | Thuộc tính 2 (1-3) | Thuộc tính 3 (1-3) |
| --- | --- | --- | ---- |
| A | 3 | 3 | 2 |
| B | 4 | 2 | 3 |
| C | 2 | 1 | 1 |

</center>

***Chuẩn hóa các giá trị ordinal***

<center>

| Đối tượng | Thuộc tính 1 | Thuộc tính 2 | Thuộc tính 3 |
| --- | --- | --- | ---- |
| A | $\frac{3-1}{5-1} = \frac{2}{4} = 0.5$ | $\frac{3-1}{3-1} = \frac{2}{2} = 1$ | $\frac{2-1}{3-1} = \frac{1}{2} = 0.5$ |
| B | $\frac{4-1}{5-1} = \frac{3}{4} = 0.75$ | $\frac{2-1}{3-1} = \frac{1}{2} = 0.5$ | $\frac{3-1}{3-1} = \frac{2}{2} = 1$ |
| C | $\frac{2-1}{5-1} = \frac{1}{4} = 0.25$ | $\frac{1-1}{3-1} = \frac{0}{2} = 0$ | $\frac{1-1}{3-1} = \frac{0}{2} = 0$ |

</center>

**Kết luận**

- Đối tượng A: Thuộc tính 1 = 0.5, Thuộc tính 2 = 1, Thuộc tính 3 = 0.5
- Đối tượng B: Thuộc tính 1 = 0.75, Thuộc tính 2 = 0.5, Thuộc tính 3 = 1
- Đối tượng C: Thuộc tính 1 = 0.25, Thuộc tính 2 = 0, Thuộc tính 3 = 0

---

### Độ khác biệt của đối tượng dữ liệu có nhiều kiểu thuộc tính

Để tính độ khác biệt giữa hai đối tượng dữ liệu có nhiều kiểu thuộc tính khác nhau, ta sử dụng công thức tổng quát sau:

$$
d(i, j) = \frac{\sum_{f=1}^{p} \sigma^f_{ij} \cdot d^f_{ij}}{\sum_{f=1}^{p} \sigma^f_{ij}}
$$

**Với**

- $d(i, j)$: Độ khác biệt tổng thể giữa hai đối tượng $i$ và $j$
- $p$: Tổng số thuộc tính
- $\sigma^f_{ij}$: Trọng số của thuộc tính $f$ giữa hai đối tượng $i$ và $j$
- $d^f_{ij}$: Độ khác biệt của thuộc tính $f$ giữa hai đối tượng $i$ và $j$

**Giải Thích**

- **Numerical**: Đối với thuộc tính số, $d^f_{ij}$ có thể là khoảng cách Euclidean, Manhattan hoặc Minkowski giữa các giá trị của thuộc tính đó.
    - Ví dụ: $d^f_{ij} = |x_{if} - x_{jf}|$ (khoảng cách Manhattan)

- **Nominal**: Đối với thuộc tính danh nghĩa, $d^f_{ij}$ thường là 0 nếu hai giá trị giống nhau và 1 nếu khác nhau.
    - Ví dụ: $d^f_{ij} = \begin{cases} 
            0 & \text{nếu } x_{if} = x_{jf} \\
            1 & \text{nếu } x_{if} \neq x_{jf} 
            \end{cases}
   $

- **Binary**: Đối với thuộc tính nhị phân, $d^f_{ij}$ có thể được tính bằng công thức Jaccard hoặc công thức khác tùy thuộc vào tính chất đối xứng hay không đối xứng của dữ liệu.
    - Ví dụ: $d^f_{ij} = \frac{r + s}{q + r + s}$ (Jaccard distance)

- **Ordinal**: Đối với thuộc tính thứ tự, $d^f_{ij}$ có thể được tính dựa trên giá trị chuẩn hóa của các thứ hạng.
    - Ví dụ: $d^f_{ij} = |Z_{if} - Z_{jf}|$ với $Z_{if} = \frac{r_{if} - 1}{M_f - 1}$

**Kết Luận**

Công thức tổng quát trên cho phép tính toán độ khác biệt giữa hai đối tượng dữ liệu có nhiều kiểu thuộc tính khác nhau bằng cách sử dụng các phương pháp tính toán phù hợp cho từng loại thuộc tính cụ thể.
