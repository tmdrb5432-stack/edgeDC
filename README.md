# 전국 데이터센터 영업 현황

## GitHub Pages 배포

1. GitHub에 새 저장소를 만듭니다.
2. 이 폴더의 `index.html`과 `README.md`를 저장소 최상위에 업로드하고 Commit합니다. ZIP 파일 자체를 올리지 마세요.
3. Settings → Pages → Build and deployment에서 Source를 Deploy from a branch로 선택합니다.
4. Branch를 `main`, 폴더를 `/ (root)`로 선택하고 Save합니다.
5. 배포가 완료되면 Settings → Pages의 Visit site 링크를 엽니다.

일반적인 프로젝트 사이트 주소: `https://계정명.github.io/저장소명/`

## 지도

현재 지도는 Leaflet과 OpenStreetMap을 사용하며 API 키는 필요하지 않습니다. Leaflet 코드는 HTML 안에 포함되어 있으나 지도 이미지에는 인터넷 연결이 필요합니다. 지도 이미지 접속이 차단되면 오류 안내가 표시됩니다. OpenStreetMap 타일 서비스는 무중단을 보장하지 않으므로 지속적인 업무 서비스에는 별도 지도 API를 검토하세요. 타일 정책: https://operations.osmfoundation.org/policies/tiles/

국내 지도에는 카카오맵 Web(JavaScript) SDK를 추천합니다. 카카오 개발자 앱 생성, 카카오맵 API 활성화, JavaScript 키 발급, 배포 도메인 등록이 필요하며 적용 시 지도 코드를 교체해야 합니다. 이 파일에는 아직 카카오맵이 연결되어 있지 않습니다. REST API 키나 관리자 키를 공개 저장소에 넣지 마세요.

## 데이터와 공개 범위

사업 데이터는 `index.html`의 `const D` 배열에 들어있으며 자동 갱신되지 않습니다. 좌표는 대략적인 참고 위치입니다. 출처와 실제 주소를 확인해 갱신하세요.

GitHub Pages는 일반적으로 공개 웹사이트입니다. 저장소를 비공개로 설정해도 Pages 사이트가 자동으로 비공개가 되는 것은 아닙니다. 민감한 영업 데이터는 올리지 마세요. 접근 제한이 필요하면 인증 기능이 있는 별도 호스팅을 사용하세요.
