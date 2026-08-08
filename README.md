# vocarock-site

보카락(VocaRock) 앱 공식 웹사이트. 앱스토어 · 구글플레이 제출과 통신판매업 신고에 사용하는 공개 페이지입니다.

순수 HTML/CSS이며 빌드 과정이 없습니다. `main` 브랜치 루트를 GitHub Pages로 서빙합니다.

## 페이지

| 파일 | 용도 | 스토어에서 쓰이는 곳 |
| --- | --- | --- |
| `index.html` | 랜딩 | 조직 웹사이트 URL, 스토어 등록정보 웹사이트 |
| `privacy.html` | 개인정보처리방침 | Play Console 개인정보처리방침 URL, App Store Privacy Policy URL |
| `terms.html` | 이용약관 + 구매/환불 안내 | App Store EULA/약관 URL |
| `support.html` | 고객지원 · FAQ | App Store Support URL (필수) |
| `delete-account.html` | 계정 삭제 안내 | Play Console 데이터 삭제 URL, App Store 심사지침 5.1.1(v) |

## 채워야 하는 항목

각 페이지 푸터에 `class="ph"` 로 표시된 항목이 미기입 상태입니다. 전역 치환으로 채우면 됩니다.

- `[상호명 입력 예정]` → 사업자등록증상 상호
- `[000-00-00000]` → 사업자등록번호
- `[신고 완료 후 기재 예정]` → 통신판매업신고번호

## 로컬 확인

```bash
python3 -m http.server 4173
```

## 콘텐츠 원본

법무 문서 본문은 앱 저장소(`vocab-lock-app`)의 `docs/legal/` 를 옮긴 것입니다.
내용을 고칠 때는 양쪽을 함께 맞춰 주세요.
