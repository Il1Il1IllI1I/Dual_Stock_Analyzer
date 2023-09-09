# Dual_Stock_Analyzer
## 💡 코드 해설

### 📦 라이브러리 임포트
- **`yfinance`**: Yahoo Finance에서 주식 데이터를 가져옵니다. 🌐
- **`pandas`**: 데이터를 처리하고 분석합니다. 🐼
- **`matplotlib`**: 데이터를 그래프로 시각화합니다. 📊

---

### 📈 주식 데이터 다운로드
- **`yf.Ticker(stock).info`**: 선택한 주식의 기본 정보를 가져옵니다. 📜
- **`yf.download(stock)['Adj Close']`**: 조정 종가 데이터를 다운로드합니다. 💹

---

### 🛠 분석 및 시각화
- 선택한 기간에 따라 주식 데이터를 분석하고 그래프로 표현합니다. 📅

---

### 📝 결과 해설
- **`상관계수`**: 두 주식의 가격 움직임의 관계를 나타냅니다. ↔️
- **`변동성`**: 주식 가격의 안정성을 나타냅니다. 🌪️
- **`수익률`**: 특정 기간 동안의 주식 수익을 나타냅니다. 💰


# 주식 분석 스크립트 사용 가이드

## 소개

이 Python 스크립트는 `yfinance` 라이브러리를 이용하여 두 종목의 주가를 분석하고 시각화합니다.  
분석하는 정보에는 기간 별 주가, 수익률, 변동성, 상관계수가 포함됩니다.

---

## 설치 방법

1. 필요한 패키지를 설치합니다.
    ```bash
    pip install yfinance pandas matplotlib
    ```

---

## 사용 방법

### 기본 설정

- **한글 폰트 설정**:  
  - Mac 사용자는 `AppleGothic`을, Windows 사용자는 `Malgun Gothic`을 사용하세요.

---

### 함수 설명

- **show_stock_analysis(stock1, stock2, periods)**:  
    - `stock1`, `stock2`: 분석할 주식의 심볼
    - `periods`: 분석할 기간을 담은 리스트. 각 기간은 ('시작일', '종료일') 형식으로 지정

---

### 사용 예시

```python
periods = [
    ('2021-06-10', '2023-08-29'),  # 아이폰 15 출시 전
]
show_stock_analysis('USDKRW=X', '069500.KS', periods)



