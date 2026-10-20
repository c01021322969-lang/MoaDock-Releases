# MoaDock 제3자 소프트웨어 고지

MoaDock 자체 프로그램은 `LICENSE.txt`의 소스 비공개 무료 사용 조건으로 제공됩니다. 아래 구성요소는 별도의 오픈소스/제3자 라이선스로 제공되며 MoaDock의 조건으로 재라이선스되지 않습니다. 그 권리와 의무가 해당 구성요소에 우선합니다.

## Qt / PySide6 / Shiboken 6.12.0

MoaDock은 Qt/PySide6/Shiboken의 LGPLv3 사용 가능한 구성요소를 동적 라이브러리로 사용합니다. Qt는 The Qt Company 및 기여자의 저작물입니다. 상용 라이선스를 구매했다고 주장하지 않습니다. 패키지에 포함된 상용 라이선스 안내문은 대안 조건의 원문 보존이며 MoaDock의 상용 라이선스 보유 증거가 아닙니다.

LGPLv3 및 GPLv3 원문은 `third_party/Qt-open-source`에, 대응 소스 안내는 `SOURCE-ACCESS.md`에 있습니다. 수정·교체·재연결과 그 디버깅에 필요한 역공학을 허용하며 MoaDock의 자체 코드 비공개 조건으로 이를 제한하지 않습니다. 사용하지 않는 Qt DataVisualization·VirtualKeyboard 모듈은 배포에서 제외합니다. 라이선스: https://doc.qt.io/qt-6/licensing.html

## 7-Zip 26.04

MoaDock의 7Z/RAR 압축 해제는 Igor Pavlov와 기여자가 제작한 7-Zip 실행 파일과 DLL을 별도 프로세스로 사용합니다. MoaDock이 압축 엔진을 자체 작성했다고 주장하지 않습니다.

원본 고지 `vendor/7zip/License.txt` 및 `third_party/7zip/License.txt`를 유지합니다. 주요 라이선스는 GNU LGPL이며 일부 코드는 BSD, RAR 해제 코드는 unRAR 제한을 따릅니다. unRAR 소스를 RAR 호환 압축기 개발에 사용할 수 없다는 제한 등은 해당 고지 원문을 확인하세요. LGPLv2.1 원문도 제공합니다. 원본: https://www.7-zip.org/ / 대응 소스는 별도 묶음에 포함합니다.

## FFmpeg 구분

- **포함됨**: Qt 영상 재생용 FFmpeg 9.0.1 DLL. 바이너리가 LGPL 2.1-or-later 및 shared 빌드를 보고했습니다. 원문은 `third_party/FFmpeg`, 버전·빌드 옵션은 `third_party/FFmpeg/build-evidence.json`, 대응 소스는 별도 소스 묶음에 있습니다.
- **포함하지 않음**: 화면 녹화를 위해 별도 실행하는 `ffmpeg.exe`. 사용자가 설치한 빌드의 GPL/LGPL·코덱 조건은 해당 빌드에 따릅니다. 향후 함께 배포하려면 별도 검토해야 합니다.
- OpenCV는 이미지 처리에 사용하며 사용하지 않는 선택적 videoio FFmpeg 플러그인 DLL은 새 배포 ZIP에서 제외합니다. 기존 OpenCV 고지는 원문대로 유지합니다.

FFmpeg 라이브러리의 zlib 빌드 의존성 소스도 함께 보관합니다. https://ffmpeg.org/legal.html

## 나머지 구성요소

| 구성요소 | 주요 조건·고지 |
|---|---|
| Python 3.13.2 | Python 라이선스 원문과 포함된 제3자 고지 |
| QtPy / qtmaterialsymbols | MIT, 원문 고지 유지 |
| Google Material Symbols 폰트 | Apache 2.0, 별도 원문 포함 |
| OpenCV / opencv-python-headless | Apache 2.0 및 휠의 제3자 고지 |
| NumPy와 내장 구성요소 | BSD/MIT 등, 패키지의 전체 LICENSE 원문 |
| openpyxl / et-xmlfile / python-docx | MIT 등 패키지별 LICENSE/LICENCE 원문 |
| olefile / pypdf / xlrd / lxml | BSD 등 패키지별 고지와 lxml 내장 의존성 고지 |
| pypdfium2 / PDFium | Apache/BSD 및 빌드별 제3자 고지 |
| PyInstaller 부트로더 | GPL 및 실행 파일 배포 예외, 원문 보존 |

정확한 설치 버전과 원문 경로는 `third_party/inventory.json`을 확인하세요. 프로젝트가 전체 구성요소를 자체 소유하거나 모두 동일 라이선스라고 주장하지 않습니다.

## 앱 자산·샘플·데이터

2026-10-20 관리자는 기존 icon.ico·icon.png·logo.png를 직접 제작했거나 재배포 권한이 있다고 확인했습니다. 이름·로고를 이용한 공식 사칭은 허용하지 않습니다. 리뷰·튜토리얼의 실제 앱 화면 사용은 LICENSE.txt에 따릅니다.
개발 저장소의 libarchive 테스트 자료에는 별도 `tests_data/LIBARCHIVE-LICENSE.txt`가 적용됩니다. 실행 ZIP에는 사용자 설정·메모·문서·캡처·테스트 자료를 포함하지 않습니다.

대응 소스와 라이브러리 교체 방법은 SOURCE-ACCESS.md와 LIBRARY_REPLACEMENT.md를 확인하세요. 모듈·배포 파일이 바뀌면 실제 구성과 이 문서를 다시 대조해야 합니다.
