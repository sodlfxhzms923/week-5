# ADR-0001: GitHub Wiki를 문서 관리 도구로 사용

## 1. 기본 정보

- **상태:** Accepted
- **작성일:** 2026-11-12
- **작성자:** sodlfxhzms923

## 2. 결정 배경 (Context)

week-5 프로젝트에서는 개발 과정에서 필요한 문서와 문제 해결 방법을 체계적으로 관리할 필요가 있습니다.

특히 Getting Started, Development Guide, Troubleshooting 등의 문서를 작성하고 서로 연결해야 합니다.

따라서 별도의 복잡한 환경 구축 없이 GitHub에서 문서를 작성하고 공유할 수 있는 방법을 검토하였습니다.

## 3. 고려한 대안 (Alternatives)

### 대안 A: GitHub Wiki

장점:
- GitHub 저장소와 연결하여 사용할 수 있습니다.
- Markdown을 지원합니다.
- 문서별 페이지와 링크를 쉽게 관리할 수 있습니다.
- 별도의 웹 서버를 구축할 필요가 없습니다.

단점:
- GitHub Wiki가 비활성화되면 문서에 접근하기 어렵습니다.
- 일반 저장소 코드와 Wiki의 버전 관리가 분리되어 있습니다.

### 대안 B: README.md 및 docs 디렉터리

장점:
- 일반 코드와 문서를 함께 관리할 수 있습니다.
- Pull Request를 통한 문서 리뷰가 가능합니다.

단점:
- 문서가 많아지면 별도 목차 관리가 필요합니다.
- Wiki에 비해 문서 탐색 환경을 직접 구성해야 합니다.

## 4. 최종 결정 (Decision)

일반적인 프로젝트 안내 및 개발 가이드는 GitHub Wiki에서 관리하기로 결정하였습니다.

GitHub Wiki는 문서별 페이지 작성과 상호 링크 기능을 제공하므로, 이번 프로젝트의 학습 목적에 적합하다고 판단하였습니다.

단, 기술적인 의사결정 기록은 코드 변경과 함께 관리할 수 있도록 docs/adr 디렉터리에 별도로 저장합니다.

## 5. 결정의 영향 (Consequences)

### 긍정적 영향

- 프로젝트 문서를 쉽게 작성하고 공유할 수 있습니다.
- 관련 문서를 링크로 연결하여 탐색성을 높일 수 있습니다.
- 별도의 문서 관리 서버가 필요하지 않습니다.

### 부정적 영향

- Wiki 문서와 일반 저장소 문서가 분리되어 관리됩니다.
- 문서 링크와 내용이 오래되지 않도록 정기적으로 확인해야 합니다.

## 6. 향후 계획

- Wiki 문서를 지속적으로 관리합니다.
- 기술적인 변경 사항은 ADR에 추가합니다.
- 중요한 기술 제안은 GitHub Discussions에서 논의한 뒤 ADR로 기록합니다.

## 7. 관련 자료

- [GitHub Wiki](https://github.com/sodlfxhzms923/week-5/wiki)
- [Getting Started](https://github.com/sodlfxhzms923/week-5/wiki/Getting-Started)
- [Development Guide](https://github.com/sodlfxhzms923/week-5/wiki/Development-Guide)
- [Troubleshooting](https://github.com/sodlfxhzms923/week-5/wiki/Troubleshooting)
