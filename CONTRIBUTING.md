# Contribution Guide

## Branch

작업 전 Issue를 생성하고 새로운 Branch에서 작업합니다.

브랜치 이름은 다음 형식을 권장합니다.

- `feat/12-coupon-ui`
- `fix/24-pod-restart`
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
