# TSMAN CCE 점검

Windows 서버·PC의 보안 설정을 KISA「주요정보통신기반시설 기술적 취약점 분석·평가 방법 상세가이드」 기준으로 점검하고, HTML·PDF·Excel 보고서를 만드는 무료 도구입니다.

- 설치 없이 exe 하나로 실행 (원하면 Program Files 에 설치)
- 서버 45개 / PC 15개 항목 자동 점검, 판정: 양호 · 취약 · 수동확인 · 점검불가
- 점검은 읽기 전용, 조치 기능은 기본 꺼짐 (켜도 항목별 승인 · 백업 · 되돌리기)
- 여러 장비 결과 모아보기, Excel 조치 관리 대장
- 외부 전송 없음 — 결과는 실행한 PC 안에만 저장

📖 사용법·소개: https://ittsman.com

## 다운로드

오른쪽 **[Releases](../../releases)** 에서 최신 `TsmanCCE-버전.zip` 을 받으세요.

### 무결성 확인
```powershell
Get-FileHash .\TsmanCCE.exe -Algorithm SHA256
```
Release 페이지와 `SHA256SUMS.txt` 의 값이 같아야 합니다.

### 실행 시 경고
코드 서명이 없는 개인 제작 프로그램이라 "Windows의 PC 보호" 창이 뜹니다. 해시를 확인한 뒤 **추가 정보 → 실행**을 누르세요.

## 실행 환경
| 구분 | OS |
|---|---|
| 실기 확인 | Windows 11 Pro |
| 설계상 대상 (검증 전) | Windows Server 2016 / 2019 / 2022, Windows 10 |
| 지원 안 함 | Windows Server 2012 R2 이하 |

.NET Framework 4.6.2 이상 필요 (위 OS 에는 기본 포함).

## 사용 조건
무료로 사용·공유할 수 있으며 판매·변조 배포는 금지합니다. 자세한 내용은 [LICENSE.txt](LICENSE.txt).
소스 코드는 공개하지 않습니다. KISA 와 관계없는 개인 제작 도구입니다.

## 문의·버그 제보
[Issues](../../issues) 에 남겨 주세요. 점검 결과 파일을 올릴 때는 호스트명·IP·계정명을 지워 주세요.
