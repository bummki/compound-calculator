# 블로그용 복리 계산기

이 저장소에는 블로그에 삽입할 수 있는 복리 계산기가 포함되어 있습니다. 사용자들이 투자 수익률을 계산하고 재테크 계획을 세울 수 있도록 도와주는 유용한 도구입니다.

## 파일 설명

- `compound_interest_calculator.html` - 복리 계산기 독립형 버전
- `blog_post_integration.html` - 블로그 포스트에 복리 계산기를 통합한 예시

## 사용 방법

### 티스토리 블로그 적용 방법

1. **HTML 편집기 활용**
   - 티스토리 블로그 포스트 작성시 HTML 편집 모드로 전환
   - `compound_interest_calculator.html` 파일의 내용을 복사하여 붙여넣기
   - 필요에 따라 스타일을 블로그 테마에 맞게 조정

2. **HTML 위젯으로 사용**
   - 티스토리 스킨 편집에서 HTML/CSS 위젯 추가
   - `compound_interest_calculator.html` 파일의 내용을 복사하여 위젯에 붙여넣기

### 기능 설명

이 복리 계산기는 다음 기능을 제공합니다:

- 초기 투자금액 설정
- 연이율 설정 (%)
- 투자 기간 설정 (년)
- 매년 추가 투자금액 설정
- 복리 계산 주기 선택 (연복리, 반기복리, 분기복리, 월복리, 일복리)
- 계산 결과 테이블 표시 (연차별 원금, 이자, 연말 금액)

## 커스터마이징

필요에 따라 다음 요소를 커스터마이징할 수 있습니다:

- CSS 스타일 - 블로그 디자인에 맞게 색상 및 배치 조정
- 기본값 - 입력 필드의 기본값 변경
- 결과 표시 방식 - 테이블 형식 또는 필요에 따라 그래프 추가

## 샘플 코드

```javascript
// 복리 계산 핵심 로직
for (let period = 0; period < frequency; period++) {
    const periodInterest = balance * (rate / frequency);
    balance += periodInterest;
    yearlyInterest += periodInterest;
}
```

## 라이센스

이 코드는 자유롭게 사용, 수정 및 배포할 수 있습니다.
