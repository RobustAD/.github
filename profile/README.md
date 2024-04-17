<div align="center">
<img src="https://capsule-render.vercel.app/api?type=waving&color=auto&height=200&section=header&text=Commit_Message_Convention&fontSize=56" /></div>
<br>
<h1>메시지 구조</h1>
<p>먼저 커밋 메시지는 크게 <strong>제목, 본문, 꼬리말</strong> 세 가지 파트로 나누고, 각 파트는 빈줄을 두어서 구분합니다.</p>

<div align="center"><table border="1">
	<tr>
	    <td><strong>Type</strong></td>
	    <td>제목</td>
	</tr>
	<tr>
	    <td><strong>Body</strong></td>
	    <td>본문</td>
	</tr>
  <tr>
    <td><strong>Footer</strong></td>
    <td>꼬리말</td>
  </tr>
</table></div>

<h1>Type</h1><br>
<h2>태그</h2>
<p>타입은 태그와 제목으로 구성되고, 태그는 영어로 쓰되 첫 문자는 대문자로 합니다.</p>
<p><strong>"태그:제목"의 형태이며, : 뒤에만 space가 있음에 유의합니다.</strong></p>
<div align="center"><table border="1">
	<th>태그 이름</th>
	<th>설명</th>
	<tr>
	    <td><strong>Feat</strong></td>
	    <td>새로운 기능을 추가할 경우</td>
	</tr>
	<tr>
	    <td><strong>Fix</strong></td>
	    <td>버그를 고친 경우</td>
	</tr>
  <tr>
    <td><strong>Design</strong></td>
    <td>CSS 등 사용자 UI 디자인 변경</td>
  </tr>
    <tr>
    <td><strong>docs</strong></td>
    <td>문서 수정</td>
  </tr>
    <tr>
    <td><strong>!BREAKING CHANGE</strong></td>
    <td>커다란 API 변경의 경우 (ex API의 arguments, return 값의 변경, DB 테이블 변경, 급하게 치명적인 버그를 고쳐야 하는 경우)</td>
  </tr>
    <tr>
    <td><strong>!HOTFIX</strong></td>
    <td>급하게 치명적인 버그를 고쳐야하는 경우</td>
  </tr>
  <tr>
    <td><strong>Style</strong></td>
    <td>코드 포맷 변경, 세미 콜론 누락, 코드 수정이 없는 경우</td>
  </tr>
  <tr>
    <td><strong>Refactor</strong></td>
    <td>프로덕션 코드 리팩토링, 새로운 기능이나 버그 수정없이 현재 구현을 개선한 경우</td>
  </tr>
  <tr>
    <td><strong>Comment</strong></td>
    <td>필요한 주석 추가 및 변경</td>
  </tr>
  <tr>
    <td><strong>Docs</strong></td>
    <td>문서를 수정한 경우</td>
  </tr>
  <tr>
    <td><strong>Test</strong></td>
    <td>테스트 추가, 테스트 리팩토링(프로덕션 코드 변경 X)</td>
  </tr>
  <tr>
    <td><strong>Chore</strong></td>
    <td>빌드 태스트 업데이트, 패키지 매니저를 설정하는 경우(프로덕션 코드 변경 X)</td>
  </tr>
  <tr>
    <td><strong>Rename</strong></td>
    <td>파일 혹은 폴더명을 수정하거나 옮기는 작업만인 경우</td>
  </tr>
  <tr>
    <td><strong>Remove</strong></td>
    <td>파일을 삭제하는 작업만 수행한 경우</td>
  </tr>
</table></div><br>

<h2>구분</h2>
<p>태그는 다음과 같은 같은 종류로 구분됩니다.</p>
<ol>
<li><p><strong>기능: </strong>Feat, Fix, Design, !BREAKING CHANGE
추가적인 문맥 정보를 제공하기 위한 목적으로 괄호 안에 적을 수도 있습니다.
ex)
"Feat(navigation): "
"Fix(database): "
</p></li>
<li><p><strong>개선: </strong>Style, Refactor, Comment</p>
<p>Style의 경우 오타 수정, 탭 사이즈 변경, 변수명 변경 등에 해당하고, Refactor의 경우 코드를 리팩토링 하는 경우에 적용할 수 있습니다. </p></li>
<li><p><strong>그 외: </strong>Docs, Test, Chore, Rename, Remove</p>
<p>Docs의 경우 README.md 수정 등에 해당하고, Test는 test 폴더 내부의 변경이 일어난 경우에만 해당합니다. Chore의 경우 package.json의 변경이나 dotenv의 요소 변경 등, 모듈의 변경에 해당됩니다. </p></li>
</ol><br>

<h2>제목은 어떻게 적는가? </h2>
<p>제목은 코드 변경 사항에 대한 짧은 요약을 나타냅니다. 제목은 다음의 규칙을 지킵니다.</p>
<ol>
  <li>제목의 처음은 동사 원형으로 시작합니다.</li>
  <li>총 글자 수는 50자 이내로 작성합니다.</li>
  <li>마지막에 특수문자는 삽입하지 않습니다. 예) 마침표(.), 느낌표(!), 물음표(?)</li>
  <li>제목은 개조식 구문으로 작성합니다.</li>
</ol>
<p>만약 영어로 작성하는 경우 다음의 규칙을 따릅니다.</p>
<ol>
<li>첫 글자는 대문자로 작성합니다.</li>
<li>"Fix", "Add", "Change"의 명령어로 시작합니다.</li>
</ol>
<p>한글로 제목을 작성하는 경우 다음의 규칙을 따릅니다.</p>
<ol>
<li>"고침", "추가", "변경"의 명령어로 시작합니다.</li>
</ol>
 <div align="center"><table border="1">
 <table><td>예시)<br>Feat: "추가 get data api 함수"</td></table></div>
 
 <h1>Body</h1><br>
 <h2>본문은 어떻게 작성하는가</h2>
 <p>본문은 다음의 규칙을 지킵니다.</p>
 <ol>
 <li>본문은 <strong>한 줄 당 72자 내</strong>로 작성합니다.</li>
 <li>본문 내용은 양에 구애받지 않고 <strong>최대한 상세히 작성</strong>합니다.</li>
 <li>본문 내용은 <strong>어떻게 변경했는지</strong> 보다 <strong>무엇을 변경했는지</strong> 또는 <strong>왜 변경했는지</strong>를 설명합니다.</li>
 </ol><br>
 
 <h1>Footer</h1><br>
 <h2>꼬리말은 어떻게 작성하는가</h2>
 <p>꼬리말은 다음의 규칙을 지킵니다.</p>
 <ol>
 <li>꼬리말은 optional이고 이슈 트래커 ID를 작성합니다.</li>
 <li>꼬리말은 "유형: #이슈 번호" 형식으로 사용합니다.</li>
 <li>여러 개의 이슈 번호를 적을 때는 쉼표로 구분합니다.</li>
 <li>이슈 트래커 유형은 다음 중 하나를 사용합니다.
   <ul>
     <li>Fixes: 이슈 수정중 (아직 해결되지 않은 경우)</li>
     <li>Resolves: 이슈를 해결했을 때 사용</li>
     <li>Ref: 참고할 이슈가 있을 때 사용</li>
     <li>Related to: 해당 커밋에 관련된 이슈번호 (아직 해결되지 않은 경우)</li>
   </ul>
 </li>
 <p><strong>ex) Fixes: #45 Related to: #34, #23</strong></p>
 </ol><br>
 
 <p>지금까지 배운 내용을 토대로 로그인 API를 개발한 내용을 커밋할 때, 커밋 메시지를 작성한다면 어떻게 작성할 수 있을까요?</p>
 <div align="center"><table border="1">
 <table><td>Feat: "추가 로그인 함수"<br>

로그인 API 개발<br>

Resolves: #123
Ref: #456
Related to: #48, #45</td></table></div>
