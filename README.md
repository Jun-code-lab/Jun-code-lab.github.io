
# 서울 휴지통 지도 (GitHub Pages 배포용)

## 파일 구성
- `index.html` : 메인 페이지 (모바일 HTTPS에서 위치 동작)
- `주소 수정.csv` : 휴지통 좌표 데이터 (lat, lon 필요) (포함됨)
- `HangJeongDong_ver20250401.geojson` : 서울 행정경계 GeoJSON (포함됨)

## 사용법
- 같은 폴더에 CSV/GeoJSON를 두면 자동 로드
- 파일명이 다르면 URL에 `?csv=내.csv&geo=내.geojson`

## 로컬 테스트
```bash
python -m http.server 8000
# 브라우저에서 http://localhost:8000
```

## GitHub Pages
- 레포지토리 "Settings → Pages"에서 **Deploy from a branch** 선택
- Branch: `main` / Folder: `/root` (또는 `/docs`에 올리는 경우 Folder `/docs`)
- 발급된 HTTPS 주소에서 접속
