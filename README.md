# 📚iOS-CodeVault
### This is a space where I can freely jot down notes.
---
## 📒프로퍼티(Property)
- 저장 프로퍼티(Stored Property)
    - 값을 저장하기 위해 선언되는 상수/변수
    - 클래스, 구조체에서 사용
- 연산 프로퍼티(Computed Property)
- 타입 프로퍼티(Type Property)
  

## 📒초기화(Initializers)
- 저장 속성(
---

## 📒TableView



### ❗️UITableViewDelegate 프로토콜 주요 메서드

🍔 지정된 행이 선택되었음을 알리는 메서드
<br/>
func tableView(UITableView, didSelectRowAt: IndexPath) 
<br/>
<br/>

🍔 지정된 행의 선택이 해제되었음을 알리는 메서드
<br/>
func tableView(UITableView, didDeselectRowAt: IndexPath)
<br/>
<br/>

🍔 특정 위치 행의 높이를 묻는 메서드
<br/>
func tableView(UITableView, heightForRowAt: IndexPath)
<br/>
<br/>

🍔 특정 위치 행의 들여쓰기 수준을 묻는 메서드
<br/>
func tableView(UITableView, indentationLevelForRowAt: IndexPath)
<br/>
<br/>

🍔 특정 섹션의 헤더뷰 또는 푸터뷰를 요청하는 메서드
<br/>
func tableView(UITableView, viewForHeaderInSection: Int)
<br/>
func tableView(UITableView, viewForFooterInSection: Int)
<br/>
<br/>

🍔 특정 섹션의 헤더뷰 또는 푸터뷰의 높이를 물어보는 메서드
<br/>
func tableView(UITableView, heightForHeaderInSection: Int)
<br/>
func tableView(UITableView, heightForFooterInSection: Int)
<br/>
<br/>

🍔 테이블뷰가 편집모드에 들어갔음을 알리는 메서드
<br/>
func tableView(UITableView, willBeginEditingRowAt: IndexPath)
<br/>
<br/>

🍔 테이블뷰가 편집모드에서 빠져나왔음을 알리는 메서드
<br/>
func tableView(UITableView, didEndEditingRowAt: IndexPath?)
<br/>
<br/>
<br/>
<br/>

### ❗️UITableViewDataSource 프로토콜 주요 메서드 (🌟 => required)

🌟 특정 위치에 표시할 셀을 요청하는 메서드
<br/>
func tableView(UITableView, cellForRowAt: IndexPath) 
<br/>
<br/>

🌟 각 섹션에 표시할 행의 개수를 묻는 메서드
<br/>
func tableView(UITableView, numberOfRowsInSection: Int)
<br/>
<br/>

🍣 테이블뷰의 총 섹션 개수를 묻는 메서드
<br/>
func numberOfSections(in: UITableView)
<br/>
<br/>

🍣 특정 섹션의 헤더 혹은 푸터 타이틀을 묻는 메서드
<br/>
func tableView(UITableView, titleForHeaderInSection: Int)
func tableView(UITableView, titleForFooterInSection: Int)
<br/>
<br/>

🍣 특정 위치의 행을 삭제 또는 추가 요청하는 메서드
<br/>
func tableView(UITableView, commit: UITableViewCellEditingStyle, forRowAt: IndexPath)
<br/>
<br/>

🍣 특정 위치의 행이 편집 가능한지 묻는 메서드
<br/>
func tableView(UITableView, canEditRowAt: IndexPath)
<br/>
<br/>

🍣 특정 위치의 행을 재정렬 할 수 있는지 묻는 메서드
<br/>
func tableView(UITableView, canMoveRowAt: IndexPath)
<br/>
<br/>

🍣 특정 위치의 행을 다른 위치로 옮기는 메서드
<br/>
func tableView(UITableView, moveRowAt: IndexPath, to: IndexPath)
<br/>
<br/>

---

## 📒위치 권한
### Privacy - Location When In Use Usage Description (iOS 11 이상)
→ 앱이 포그라운드에서 실행 중일 때만 위치 정보에 엑세스

### Privacy - Location Always and When In Use Usage Description (iOS 11 이상)
→ 앱이 백그라운드에서 실행되는 동안 위치 정보에 엑세스

### Privacy - Location Always Usage Description (iOS 11 이전, deprecated)
→ 앱이 백그라운드에서 위치 정보에 엑세스 하고, iOS 11이전의 대상에 배포하는 경우!

### Privacy - Location Temporary Usage Description Dictionary
→ 앱의 한 부분에서 사용자 위치에 대한 임시 엑세스를 요청하는 이유를 설명

### Privacy - Location Usage Description(mac)
→ macOS 앱이 사용자의 위치 정보에 엑세스하는 API를 사용하는 경우에만 필요

### Privacy - Location Default Accuracy Reduced (iOS 14 이상)‼️
true: 기본적으로, 정확도가 떨어지는지 묻는 메세지가 표시되도록 키 값 설정
→ 사용자 선택 X. 대략적인 위치만을 제공
→ only reducedAccuracy


false: 전체 위치 정확도를 묻는 메시지가 표시되도록 설정(default)
→ 구체적인 위치를 제공할지,하지 않을지에 대해서 사용자가 선택 가능
→ fullAccuracy and reducedAccuracy

![image](https://github.com/iOS-Dev-Hyun/StudyNote/assets/142004247/375bb8ea-05b5-4e17-8350-347265eb4b01)

---


*Source*
- https://woonhyeong.tistory.com/6
