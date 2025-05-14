# Z-變換學習指南

## 1. Z-變換的定義與基本性質

### 核心概念

- **Z-變換定義**:
  \[
  X(z) = \sum_{n=-\infty}^{\infty} x[n] z^{-n}
  \]
  將離散信號 \( x[n] \) 轉換到Z域，其中 \( z \) 是複數變量。

- **線性性質**:
  \[
  Z\{\alpha x_1[n] + \beta x_2[n]\} = \alpha X_1(z) + \beta X_2(z)
  \]

- **時延性質**:
  \[
  Z\{x[n - k]\} = z^{-k} X(z)
  \]

### 練習題

求以下信號的Z-變換：
\[
x[n] = a^n u[n]
\]
其中 \( u[n] \) 是單位階躍信號， \( a \) 是常數。

### 相關影片

- [Z-Transform Introduction and Basic Properties](https://www.youtube.com/watch?v=g8GRjPPm-Ec)
- [Z-Transform: Linearity and Time-shifting](https://www.youtube.com/watch?v=VImOQeXZ9H0)

---

## 2. Z-變換與線性系統

### 核心概念

- **FIR濾波器**:
  \[
  H(z) = \sum_{k=0}^{N-1} h[k] z^{-k}
  \]

- **卷積性質**:
  \[
  Z\{x_1[n] * x_2[n]\} = X_1(z) \cdot X_2(z)
  \]

- **級聯系統**:
  \[
  H(z) = H_1(z) \cdot H_2(z)
  \]

### 練習題

給定兩個離散時間系統，其Z-變換分別為 \( H_1(z) = 1 - z^{-1} \) 和 \( H_2(z) = 1 + 2z^{-1} \)。求這兩個系統級聯後的總系統 \( H(z) \)。

### 相關影片

- [FIR Filters and Z-Transform](https://www.youtube.com/watch?v=5x_yAxb8iC8)
- [Convolution and Z-Transform](https://www.youtube.com/watch?v=shkeYFf3j-0)
- [Cascaded Systems in Z-Transform](https://www.youtube.com/watch?v=9T2qERjKhm0)

---

## 3. 去卷積（反卷積）

### 核心概念

- **去卷積目標**:
  根據已知系統的輸入和輸出，推導系統的傳遞函數 \( H(z) \)：
  \[
  H(z) = \frac{Y(z)}{X(z)}
  \]

### 練習題

已知一個系統的輸入 \( x[n] = \delta[n] \) 和輸出 \( y[n] = \delta[n] + \delta[n-1] \)。求該系統的傳遞函數 \( H(z) \)。

### 相關影片

- [Deconvolution and Inverse Filtering](https://www.youtube.com/watch?v=Q59uRQ1RzUU)

---

## 4. Z域與頻域的關係

### 核心概念

- **Z域與頻域**:
  Z-變換和離散時間傅立葉變換（DTFT）在單位圓上是等價的：
  \[
  X(e^{j\omega}) = X(z) \bigg|_{z = e^{j\omega}}
  \]

- **極點與零點**:
  \[
  H(z) = \frac{\prod_{k=1}^{M} (z - z_k)}{\prod_{l=1}^{N} (z - p_l)}
  \]
  其中 \( z_k \) 是零點， \( p_l \) 是極點。

### 練習題

給定系統函數 \( H(z) = \frac{z-0.5}{z^2 - 1.5z + 0.5} \)，找出其零點和極點的位置。

### 相關影片

- [Z-Domain and Frequency Domain](https://www.youtube.com/watch?v=9m1EdyGk12Y)
- [Poles and Zeros in Z-Transform](https://www.youtube.com/watch?v=8c83uCE7hzY)

---

## 5. Z-平面與單位圓

### 核心概念

- **單位圓**:
  在Z-平面上，單位圓是一個重要的分析工具。DTFT是Z-變換在單位圓上的取值：
  \[
  \text{單位圓} = \{ z : |z| = 1 \}
  \]

### 練習題

對於信號 \( x[n] = (\frac{1}{2})^n u[n] \)，畫出其Z-變換在Z平面上的單位圓和極點的位置。

### 相關影片

- [Understanding the Z-Plane and Unit Circle](https://www.youtube.com/watch?v=pbXUyxb1jGE)

---

## 6. 複雜應用與例子

### 核心概念

- **進階應用**:
  Z-變換在消除特定頻率的濾波器設計中有著重要的應用。設計這些濾波器需要利用零點和極點的特性。

### 練習題

設計一個消除頻率為 \( \pi/4 \) 的二階FIR濾波器，並求其系統函數 \( H(z) \)。

### 相關影片

- [Advanced Applications of Z-Transform](https://www.youtube.com/watch?v=VGe7h5uWLy8)
- [Nulling Filters using Z-Transform](https://www.youtube.com/watch?v=WQJXjMCntqU)

---

### 常見公式總覽

| **概念**                | **公式**                                                                                   |
|------------------------|------------------------------------------------------------------------------------------|
| **Z-變換定義**          | \( X(z) = \sum_{n=-\infty}^{\infty} x[n] z^{-n} \)                                       |
| **單位衝激信號**        | \( Z\{\delta[n]\} = 1 \)                                                                 |
| **指數序列**            | \( Z\{a^n u[n]\} = \frac{1}{1 - az^{-1}}, \quad |z| > |a| \)                            |
| **遞增序列**            | \( Z\{n a^n u[n]\} = \frac{a z^{-1}}{(1 - az^{-1})^2}, \quad |z| > |a| \)               |
| **線性性**              | \( Z\{\alpha x_1[n] + \beta x_2[n]\} = \alpha X_1(z) + \beta X_2(z) \)                   |
| **時延性**              | \( Z\{x[n - k]\} = z^{-k} X(z) \)                                                       |
| **時域縮放**            | \( Z\{a^n x[n]\} = X\left(\frac{z}{a}\right) \)                                         |
| **複數共軛**            | \( Z\{x^*[n]\} = X^*(z^*) \)                                                            |
| **倒置**                | \( Z\{x[-n]\} = X\left(\frac{1}{z}\right) \)                                            |
| **卷積性質**            | \( Z\{x_1[n] * x_2[n]\} = X_1(z) \cdot X_2(z) \)                                        |
| **級聯系統**            | \( H(z) = H_1(z) \cdot H_2(z) \)                                                        |
| **輸出響應**            | \( Y(z) = H(z) \cdot X(z) \)                                                            |
| **逆Z-變換公式**        | \( x[n] = \frac{1}{2\pi j} \oint_{C} X(z) z^{n-1} dz \)                                  |
| **極點與零點**          | \( H(z) = \frac{\prod_{k=1}^{M} (z - z_k)}{\prod{l=1}^{N} (z - p_l)} \)                  |
