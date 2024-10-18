# Priconne Shiritori Helper <BR>
![녹화_2024_10_14_11_14_28_183 mp4_snapshot_01 25 410](https://github.com/user-attachments/assets/b7237767-8d9e-4386-8238-a2e24ff4d072) <BR>
(🖥 사용 화면) <BR> <BR>

**프린세스 커넥트! Re:Dive** 미니게임 「**대격전! 끝말잇기 드래곤즈**」를 더욱 쉽게 즐길 수 있도록 도와줍니다. <BR>
**プリンセスコネクト！Re:Dive (プリコネR)** のミニゲーム『**大激戦！しりとりドラゴンズ**』をより簡単に楽しむことができるようサポートします。 <BR> <BR>

선택한 서버에 맞게 데이터를 로드하는 것 뿐만 아니라, 서버 전환(* 한국 서버, 일본 서버 데이터) 및 진행 상태 기록까지 할 수 있습니다. <BR>
選択したサーバーに応じてデータをロードするだけでなく、サーバーの切り替え（*韓国サーバー、日本サーバーデータ）や進行状況の記録も行うことができます。 <BR> <BR>

**🔗 URL: https://izh318.github.io/Priconne_SIRITORI_Manager** <BR> <BR>

**이 프로젝트는 비상업적인 목적으로만 사용 가능합니다.** <BR>
**このプロジェクトは非商業目的のみで使用可能です。** <BR>

<BR> <BR> <BR>

## 🔄 업데이트 내역
### v1.0.0 (2024-10-18)
- **기타**
  - `Priconne Shiritori Dragons Helper` 게시

<BR>

<details>
<summary>📜 이전 업데이트 내역 - 클릭하여 열기</summary>
</details>

<BR> <BR> <BR>

## 🔍 웹 사이트 미리보기
![녹화_2024_10_14_11_14_28_183 mp4_snapshot_03 00 000](https://github.com/user-attachments/assets/297c54ce-7029-4661-8098-a515d0855b19) <BR>
(🖥 웹 사이트 첫 로딩 화면) <BR> <BR>

![녹화_2024_10_14_11_14_28_183 mp4_snapshot_00 07 815](https://github.com/user-attachments/assets/29ae689f-6fe1-4e0f-97cd-2e245d43fe07) <BR>
(🖥 메인 화면) <BR> <BR>

![녹화_2024_10_14_11_14_28_183 mp4_snapshot_00 13 086](https://github.com/user-attachments/assets/efc76680-00bf-4847-86fc-e3df1e4b8909) <BR>
(🖥 한국 서버 선택 화면) <BR> <BR>

![녹화_2024_10_14_11_14_28_183 mp4_snapshot_00 31 008](https://github.com/user-attachments/assets/8af5d418-2f2d-42dd-b491-054bf62c55bc) <BR>
(🖥 일본 서버 선택 화면) <BR> <BR>

![녹화_2024_10_14_11_14_28_183 mp4_snapshot_01 25 410](https://github.com/user-attachments/assets/b7237767-8d9e-4386-8238-a2e24ff4d072) <BR>
(🖥 한국 서버 선택 후 단어 검색 화면 (두음법칙(표준) 체크박스 활성화)) <BR> <BR>

![녹화_2024_10_14_11_14_28_183 mp4_snapshot_02 50 000](https://github.com/user-attachments/assets/79a3ea5d-24a3-4eb2-a251-51f185a63aea) <BR>
(🖥 일본 서버 선택 후 단어 검색 화면 (無関係検索 체크박스 활성화) <BR> <BR>

![녹화_2024_10_14_11_14_28_183 mp4_snapshot_00 25 395](https://github.com/user-attachments/assets/4ac0fe4f-f1ca-4a3e-b580-ff0b53c20cda) <BR>
(🖥 진행 내역 강조 색 설정 화면 <BR>

<BR> <BR> <BR>

## 🛠️ 기능
### 1. **동적 뷰포트 조정**
   - **함수**: `setDynamicVh()`
   - **설명**: CSS 사용자 정의 속성 `--vh`를 현재 창의 내부 높이에 따라 창 로드 또는 창 크기가 조정될 때 동적으로 조정 <BR> <BR>

### 2. **WebP 지원 감지**
   - **함수**: `supportsWebP()` 및 `setLoadingImage()`
   - **설명**: 웹 브라우저에서 WebP 이미지 형식 사용 가능 판단 (＊ WebP가 지원할 때 `*.webp` 이미지 표시, 지원하지 않을 경우 `*.gif` 이미지로 대체) <BR> <BR>

### 3. **CSV 데이터 로딩**
   - **함수**: `loadData(server)`
   - **설명**: CSV 데이터 로드 후 구조화된 형식으로 파싱 <BR> <BR>

### 4. **CSV 파싱**
   - **함수**: `parseCSV(text)`
   - **설명**: CSV 텍스트를 한 행씩 파싱하며, 인용된 필드와 쉼표를 처리하고 각 줄에 대한 항목 배열 반환 <BR> <BR>

### 5. **이미지 로딩**
   - **함수**: `preloadImages()`, `loadImage(src)`
   - **설명**: 필요 이미지 로드 <BR> <BR>

### 6. **서버 선택 및 데이터 전환**
   - **함수**: `updateServerDisplay(server)`
   - **설명**: 한국 서버 및 일본 서버 간의 전환을 동적으로 수행하며, 적절한 데이터를 로드하고 UI에 올바른 데이터 업데이트 <BR> <BR>

### 7. **한국어 두음법칙 (두음법칙(표준) 체크박스 활성화 시 작동)**
`switch` 문을 사용하여 단어 첫 글자의 초성(`initial`)을 확인한 후 중성(`medial`)에 따라 새로운 단어를 생성하고 배열(`newInitialSounds`)에 저장 <br> <br>

본 코드에 적용된 규칙은 다음과 같음: <br>
- **첫 글자의 초성이 "ㄴ"인 경우**:
  - 첫 글자의 초성 "ㄴ", "ㅇ"으로 처리, 중성과 종성은 그대로 유지
  - **예:** "녀" → "녀", "여"

- **첫 글자의 초성이 "ㄹ"인 경우**:
  - 첫 글자의 초성 "ㄹ", "ㄴ", "ㅇ"으로 처리, 중성과 종성은 그대로 유지
  - **예:** "려" → "려", "녀", "여"

- **첫 글자의 초성이 "ㅇ"인 경우**:
  - 첫 글자의 초성 "ㅇ", "ㄴ", "ㄹ"으로 처리, 중성과 종성은 그대로 유지
  - **예:** "야" → "야", "냐", "랴" <br> <br>

### 8. **히라가나/가타카나 정규화 (無関係検索 체크박스 활성화 시 작동)**
   - **함수**: `normalizeHiraganaKatakana(word)`
   - **설명**: 일본어 히라가나와 가타카나를 정규화하여 두 형태 간 일관된 검색 처리 <BR> <BR>

### 9. **단어 입력 필드에 할당 (Image 클릭 시 작동)**
   - **함수**: `addWordToInput(word)`
   - **설명**: 단어의 마지막 문자를 단어 입력 필드에 할당
   - **구현**:
     - 단어의 마지막 문자 추출
     - 현재 서버가 한국 서버인 경우 마지막 문자 할당
     - 현재 서버가 일본 서버인 경우 조건 확인:
       - 마지막 문자가 작은 일본어 문자(예: ぁ, ぃ)인 경우 마지막 두 글자 할당
       - 마지막 문자가 "ー" (장음 기호)인 경우 마지막에서 두 번째 글자 할당 <BR> <BR>

### 10. **실시간 검색 및 결과 업데이트**
   - **함수**: `updateResults()`
   - **설명**: 사용자의 입력에 따라 결과 업데이트 <BR> <BR>

### 11. **기록 관리**
   - **함수**: `addToHistory(index)`, `removeFromHistory(index)`, `highlightRows()`, `parseHistory(text)`
   - **설명**: 사용자가 게임 진행 내역을 저장하고 로드할 수 있으며, 찾은 단어를 쉽게 참조할 수 있도록 강조 표시 (* 진행 상황은 오름차순으로 `*.txt` 파일에 저장 및 로드) <BR> <BR>

### 12. **디스플레이 사용자 정의 옵션**
   - **함수**: `createResultTable(results)`
   - **설명**: 사용자 선택 옵션에 따라 결과 테이블 구축(예: Word ID 표시, Image 표시 등) 및 진행 내역 기록 추가, 제거 <BR> <BR>

### 13. **로딩 화면**
   - **함수**: `hideLoadingScreen()`
   - **설명**: 모든 데이터가 완전히 로드되면 로딩 화면 숨김 처리 <BR> <BR>

### 14. **이미지 드래그 방지**
   - **이벤트 리스너**: `document.addEventListener('dragstart', ...)`
   - **설명**: 이미지 드래그 방지 <BR> <BR>

### 15. **언어별 사용자 정의**
   - **서버별 조정**: 선택된 서버(한국 또는 일본)에 따라 UI 요소 및 데이터 등 동적으로 조정 <BR>

<BR> <BR> <BR>

## 📝 출처

- **폰트**: <BR>
  Noto Sans Korean <BR>
  🔗 URL: https://fonts.google.com/noto/specimen/Noto+Sans+KR <BR>
  
  Noto Sans Japanese <BR>
  🔗 URL: https://fonts.google.com/noto/specimen/Noto+Sans+JP <BR> <BR>

- **메인 캐릭터 및 배경 이미지 리소스**:  
  株式会社Cygames © プリンセスコネクト！Re:Dive (プリコネR) Client <BR>

- **메인 캐릭터 및 배경 이미지 리소스 추출 도구** (* 자체 제작 및 수정):  
  PRICONNE_EXTRACTION_TOOLS_Portable <BR>
  🔗 URL: https://github.com/IZH318/PRICONNE_EXTRACTION_TOOLS_Portable <BR>
<BR> <BR> <BR>
