# MY EMACS CONFIGURATION

이 저장소는 개인적으로 사용하고 있는 Emacs 설정 파일을 정리합니다.

## 목표
이 설정은 Emacs를 텍스트 에디터로써 활용하고자 하는 비-개발자를 목표로 하고 있습니다. 이를 위하여 아래 사항들을 목표로 삼습니다.

- 한글 입력: 기본적으로 Emacs는 다국어 지원이 잘 되어 있으며, 한글이라고 예외는 아닙니다. 심지어 자체적으로 한글 입력기를 내장하고 있는 등, 사실상 Unix 기반 환경에서 한글을 가장 잘 지원하는 플랫폼 중 하나입니다. 따라서 본 설정에서는 한글 입력 및 표시 등을 잘 지원할 수 있도록 합니다.
- 가독성: 다른 텍스트 에디터 프로그램에 비해 폰트나 레이아웃 등 가독성을 최대한 고려하도록 설정합니다.
- 텍스트 입력: org-mode, markdown 등 다양한 환경과 문법에서 텍스트를 입력하거나 관리할 수 있도록 설정합니다.
- 크로스플랫폼: 현재 윈도우 및 OSX 환경에서 동시에 테스트되고 있으며, 리눅스 환경에서도 사용 가능하도록 합니다.

## 설치법
1. 설정파일들을 다운받아 HOME 디렉토리에 복사합니다. 혹은 git clone 명령어를 사용해도 됩니다(이쪽을 더 추천합니다). 윈도우즈의 경우, [이 문서](https://www.gnu.org/software/emacs/manual/html_node/emacs/Windows-HOME.html)를 참고하여 폴더를 찾거나 설정합니다.
3. 복사한 .emacs 파일을 열고, 다운받은 폴더 경로를 custom-file-path에 입력한 다음 저장합니다.

## 사용법
### 다국어 설정
기본적으로 한글(두벌식, 세벌식 390/391), 영문, 일문 입력을 바로 할 수 있도록 설정되어 있습니다.

- _C-\_: 입력기 (두벌식 - 390 - 391 - 일문) 를 전환합니다.
- _S-space: 설정한 입력기와 영문을 전환합니다.

## 파일 목록
- init.el: 처음 Emacs가 읽어들이는 파일입니다.
- freshstart.el: 맨 처음 설정을 적용한 경우, 초기화 및 필요한 패키지를 다운받기 위해 읽어들이는 파일입니다.
- config.org: 모든 설정이 모여져 있는 파일입니다. org-mode 형식으로 쓰여져 있으며, 따라서 Emacs나 Github 등에서 쉽게 읽을 수 있습니다.

## 패키지 목록
아래 목록은 이 설정에서 적용한 패키지 중 일부입니다. 전체 목록은 config.org 파일을 확인해 보세요.

### 문법 확장
- markdown-mode: 마크다운을 표시 및 입력할 수 있도록 합니다.
- org: Org-mode

### 인터페이스 확장
- writeroom-mode: 전체화면에서 수정할 수 있도록 합니다.
- powerline: vim과 유사하게 mode-line을 보기 좋게 수정해 줍니다.
- wc-mode: mode-line에 문서의 단어수를 표시합니다.

### 기타
- magit: Git을 편리하게 관리할 수 있습니다.

## 수정사항
- 한글을 깔끔답게 표시할 수 있도록 기본 폰트를 D2Coding으로 설정하였습니다.
- Emacs에서는 패키지 관리를 위해 여러 솔루션을 제공하지만, 가장 편리하게 관리할 수 있는 use-package를 사용하였습니다.

## TODO
- 구동시간 최적화
- 더 편리한 사용자 설정
- 별개의 프로젝트로, Emacs 한글화를 진행할 예정입니다.

## 기타
이 설정은 비정기적으로, 수시 업데이트됩니다. 개선점은 이 저장소의 issue나 이메일 (clockoon@gmail.com)을 통해 반영될 것입니다.

-- Sungbin Jeon
