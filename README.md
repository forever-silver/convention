# Forever silver convention

## 브랜치 전략

![image](https://user-images.githubusercontent.com/19657870/101913836-e1c22700-3c06-11eb-8ff6-e4876ca6efc6.png)

### master

- 최종 배포 브랜치 

### develop

- 개발 중인 브랜치, CI 테스트 코드 실패에 크게 관심을 두지 않는다.

### release

- 배포 준비 및 테스트 중인 브랜치, CI 테스트 코드가 반드시 성공하도록 수정해야된다.

ex) release-1.0.0

### feature

- 기능 개발 중인 브랜치

ex) feature/{이름}/{기능} : feature/ewan/find_user, feature/jose/create_user, feature/jade/delete_user, feature/yeti/update_user

### hotfix

- 배포 후 발생하는 긴급도 높은 이슈를 처리하는 브랜치

ex) hotfix/{태그명}/{이슈번호} : hotfix/v1.0.0/1

### tag

- release -> master 머지 후 태그 생성

ex) v1.0.0, v1.0.1

## 코드 리뷰

- feature -> develop로 pull request에 대한 코드 리뷰를 진행한다.

- Reviewer는 팀 단위로 선택한다.

- pr 작성 시 기능에 대한 상세 설명을 첨부한다.
