# Flutter Riverpod MVVM Example 💡

Flutter에서 **책 검색 앱**을 만들며 MVVM 아키텍처와 Riverpod 상태관리를 학습한 프로젝트입니다.  
검색창, GridView, BottomSheet, WebView까지 포함된 실제 UI 기반 앱을 직접 구성하며  
**앱 설계, 레이아웃 배치, 뷰 전환** 등을 실습합니다.

---

## 📁 폴더 구조

```
lib/
├── main.dart
├── data/
│   ├── model/         ← API 응답 데이터 클래스
│   └── repository/    ← API 호출 및 데이터 변환
├── ui/
│   ├── pages/
│   │   ├── home/
│   │   │   ├── widgets/
│   │   │   ├── home_page.dart
│   │   │   └── home_view_model.dart
│   │   └── detail/
│   │       ├── widgets/
│   │       ├── detail_page.dart
│   │       └── detail_view_model.dart
│   └── widgets/       ← 공통 위젯


 ```
 
 

---



## ✨ 주요 학습 내용

| 구성요소        | 설명 |
|----------------|------|
| **View**       | 검색창, 책 리스트(GridView), 상세화면(WebView) |
| **ViewModel**  | 상태 관리 및 동작 처리 (Riverpod 사용) |
| **Model**      | 책 정보 모델 (나중에 OpenAPI 연동 시 확장 가능) |
| **Repository** | 현재는 UI만 구현, 이후 API 통신을 위한 구조 설계 |

이 프로젝트에서는 다음 내용을 학습합니다:

- Flutter에서 **MVVM 구조의 실제 적용 방법**
- 상태관리 라이브러리 **Riverpod 사용법**
- **TextField, GridView, showModalBottomSheet, WebView** 실전 사용법

---

## ✍ 정리하며 – 나의 시행착오와 배운 점

🔸 처음엔 폴더 구조부터 막막했다  
Flutter에서 MVVM 구조를 나누는 기준이 애매했는데, 직접 `data`, `ui/pages`, `widgets`로 쪼개보면서 점점 익숙해졌습니다.  
처음엔 ViewModel과 Repository 역할도 헷갈렸지만, 분리하니 코드를 관리하기가 확실히 쉬워졌습니다.

🔸 실습을 통해 UI 구성 감각이 생겼다  
TextField 안에 controller를 사용하는 법, GridView의 비율 조정, 바텀시트와 WebView까지…  
기존에 이론으로만 봤던 위젯들을 직접 써보며, **UX 중심의 UI 구성 흐름**을 잡을 수 있었습니다.

---

## 🚀 실행 방법

1. Flutter SDK가 설치되어 있는지 확인하세요  
   👉 [Flutter 설치 안내](https://docs.flutter.dev/get-started/install)

2. 저장소를 클론합니다:

```bash
git clone https://github.com/your-username/flutter_book_search_app.git
cd flutter_book_search_app


 ```

 ---
 ##  📸 앱 예시 화면

- AppBar에 검색창(TextField) 배치
- GridView로 책 목록 나열
- 책 클릭 시 BottomSheet → 상세 페이지로 이동
- 상세 페이지에는 InAppWebView를 사용하여 웹페이지 표시



```
[검색창에 '해리포터' 입력 → 이미지 목록 표시 → 클릭 → 하단 정보 → 자세히 보기 → 웹 페이지 이동]

```

 ---

 ## 📚 더 자세한 내용은 블로그에서 확인하세요!
MVVM 구조 설계부터 GridView, BottomSheet, WebView까지의 실제 구현 과정을
시행착오와 함께 상세히 정리해두었습니다.

🔗 블로그 포스팅
[👉 Flutter 숙련 – 책 검색 앱 만들기 Part 01: 구조 소개 & UI 구현](https://grmeems.tistory.com/entry/Flutter-%EC%88%99%EB%A0%A8-TIL-%EC%B1%85%EA%B2%80%EC%83%89-%EC%95%B1-%EB%A7%8C%EB%93%A4%EA%B8%B0-Part-01-TextField-GridView-BottomSheet-WebView)


 ---

 
 ## 🛠 사용 기술
 
 - VSCode + Dart CLI
 - dart:convert 라이브러리 (jsonEncode, jsonDecode)
 - Flutter 3.7
 - Dart
 - Cupertino-style Dialog
 - Git & GitHub
 
 ---
 
 ## 👨‍💻 개발자
 - GitHub: [Linayoo01](https://github.com/Linayoo01)
