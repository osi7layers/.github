# Contribution Guide

## Issue

WBS의 작업 항목을 기준으로 Issue를 생성합니다.

- WBS의 작업을 기준으로 Issue를 생성합니다.
- 실제 진행할 세부 작업은 체크리스트로 작성합니다.
- WBS 항목이 너무 크거나 작은 경우 작업하기 적절한 단위로 나누거나 합칠 수 있습니다.
- 작업을 시작하면 Project의 Status를 `In Progress`로 변경합니다.
- 작업이 완료되면 관련 Pull Request를 연결합니다.

### Priority

Issue의 우선순위는 다음 기준으로 지정합니다.

| Priority | 기준                                                             |
| -------- | ---------------------------------------------------------------- |
| Urgent   | 현재 다른 작업을 막고 있거나 즉시 해결이 필요한 문제             |
| High     | 프로젝트 핵심 목표 달성에 필수이며 우선적으로 진행해야 하는 작업 |
| Medium   | 계획된 작업이지만 다른 작업을 즉시 막지는 않는 일반 작업         |
| Low      | 핵심 목표 달성에 필수적이지 않은 추가 기능 및 개선 작업          |

`Urgent`는 일반적인 계획 작업에는 사용하지 않고,
진행 중 발생한 Blocker 또는 즉시 해결해야 하는 문제에 사용합니다.

## Branch

작업 전 Issue를 생성하고 새로운 Branch에서 작업합니다.

브랜치 이름은 다음 형식을 권장합니다.

- `feat/12-coupon-ui`
- `fix/24-pod-restart`
- `infra/25-aws-vpc`
- `ci/31-jenkins-pipeline`

## Commit

커밋 메시지는 다음 형식을 사용합니다.

`type: 작업 내용`

### Commit Type

| Type     | 설명                |
| -------- | ------------------- |
| feat     | 새로운 기능         |
| fix      | 버그 수정           |
| chore    | 설정 및 기타 작업   |
| docs     | 문서 수정           |
| refactor | 코드 리팩터링       |
| test     | 테스트 추가 및 수정 |
| ci       | CI/CD 관련 작업     |

### 예시

`feat: 쿠폰 발급 UI 추가`

`fix: 로그인 API 연동 오류 수정`

`infra: AWS VPC 구성`

`infra: Product Service HPA 설정`

`ci: Jenkins 이미지 빌드 파이프라인 구성`

`docs: 배포 가이드 수정`

## Pull Request

- 작업 완료 후 Pull Request를 생성합니다.
- 관련 Issue가 있다면 `Closes #이슈번호`를 작성합니다.
- Merge 전 변경 사항을 확인합니다.
