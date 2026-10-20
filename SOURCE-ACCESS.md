# 외부 구성요소 대응 소스

MoaDock 자체 코드는 비공개로 유지합니다. 이 문서는 Qt/PySide6/Shiboken·7-Zip·Qt 미디어 FFmpeg 등의 대응 소스에 관한 안내입니다.

배포 시 실행 ZIP과 동일한 다운로드 페이지에 **MoaDock-third-party-sources-20261020.zip** 및 **SHA256SUMS.txt**를 함께 제공하세요. 이 파일은 MoaDock 자체 소스를 포함하지 않으며, 별도 비용이나 추가 가입 조건 없이 실행 ZIP의 수령자에게 같은 접근 조건으로 제공해야 합니다. 실행 파일만 다른 곳으로 옮겨 배포하는 경우에도 대응 소스 묶음과 고지를 함께 제공하세요.

- 공식 다운로드: https://github.com/c01021322969-lang/MoaDock-Releases/releases/tag/v0.1.0-beta-license1
- 외부 구성요소 대응 소스: https://github.com/c01021322969-lang/MoaDock-Releases/releases/download/v0.1.0-beta-license1/MoaDock-third-party-sources-20261020.zip
- 체크섬: https://github.com/c01021322969-lang/MoaDock-Releases/releases/download/v0.1.0-beta-license1/SHA256SUMS.txt

MoaDock 자체 개발 소스와 개발 기록은 이 저장소에 포함하지 않습니다.

원본 주소·SHA-256·크기는 `source-manifest.json`에 기록합니다. 해당 자료가 실제로 준비되지 않은 경우 배포 준비 완료라고 표시하지 않습니다. 단순 상위 홈페이지 링크만으로 대응 소스 제공을 대체했다고 간주하지 않습니다.

Qt/PySide6/Shiboken 6.12.0은 공식 원본입니다. 7-Zip은 26.04, Qt 미디어 FFmpeg는 바이너리의 `av_version_info()`가 보고한 9.0.1입니다. 라이브러리 소스는 수정하지 않았습니다. 바이너리의 버전·구성 증거와 재연결 안내를 유지하세요.
