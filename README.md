# Dual_Stock_Analyzer

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
