---
title: "개발환경 설정"
permalink: /docs/flutter-configuration/
toc: true
toc_label: "개발환경 설정"
---

Windows 환경에서 Flutter 개발환경을 설정합니다.


## 1. 시스템 요구사항
Flutter를 설치하기 위한 최소 요구 사항

- 운영체제 : Windows 7 SP1 이상(64-bit)
- 디스크공간 : 400MB
- Tools : Flutter는 아래와 같은 툴이 필요합니다.<br/>
Windows PowerShell 5.0 이상<br/>
Git for Windows 2.x


## 2. Flutter SDK 설치

### Flutter 다운로드
[Flutter 설치 홈페이지](https://flutter.dev/docs/get-started/install/windows#get-the-flutter-sdk)에서 플러터 SDK를 다운로드 합니다.
다운로드한 압축 파일을 적당한 위치(예를 들어, C:\src\flutter)에 압축을 해제합니다.

**Note** <br/>
특별한 권한이 요구되는 "C:\Program Files\"와 같은 경로에는 설치하면 안됩니다.
{: .notice--warning}

### Flutter SDK Path 등록
`제어판 > 모든 제어판 항목 > 시스템`의 `고급 시스템 설정`을 클릭하여 `시스템 속성` 창을 엽니다.
<figure>
  <img src="{{ '/assets/images/02_01_path_01.png' | relative_url }}" alt="시스템 속성">
</figure>

`고급` 탭의 `환경 변수` 버튼을 클릭하여 `환경변수` 창을 엽니다.
<figure>
  <img src="{{ '/assets/images/02_01_path_02.png' | relative_url }}" alt="환경변수">
</figure>

`시스템 변수`의 Path에 SDK를 설치한 경로의 bin 디렉토리(예를 들어, C:\src\flutter\bin)를 Path에 추가합니다.
<figure>
  <img src="{{ '/assets/images/02_01_path_03.png' | relative_url }}" alt="Path등록">
</figure>

### 플랫폼 의존성 체크(flutter doctor)
flutter doctor 명령어를 실행하여 플랫폼 의존성을 체크할 수 있습니다.
```terminal
C:\src\flutter>flutter doctor
[√] Flutter (Channel stable, v1.12.13+hotfix.8, on Microsoft Windows [Version 10.0.18362.657], locale ko-KR)

[√] Android toolchain - develop for Android devices (Android SDK version 28.0.3)
[√] Android Studio (version 3.5)
[√] VS Code (version 1.42.1)
[!] Connected device
    ! No devices available

! Doctor found issues in 1 category.
```


## 3. Android Studio 설정

### Android Studio 설치
[Android Studio](https://developer.android.com/studio)를 다운로드하고 설치합니다.

### Android 에뮬레이터 설정


### Flutter 플러그인 설치


