# hello git world 
### Git codelab 1 week

---
## git의 주요 개념
- **작업 디렉토리 (Working Directory)** : 내 PC에서 수정할 파일들이 있는 디렉토리
- **준비 영역 (Staging Area, Stage/Index)** : 커밋을 대기하고 있는 파일들이 있는 영역 
- **로컬 저장소 (Local Repository)** : 커밋된 결과가 저장되는 영역
- **원격 저장소 (Remote Repository)** : 커밋한 파일들을 원격 저장소에서 관리되며, 여러사람이 협업할 수 있는 저장소

## 기본 명령어
- **$ git init** : 현재 디렉토리에다가 작업을 하겠다고 git에게 알리는 command
- **$ git status** : 파일들의 버전관리 상태를 파악하는 command
- **$ git add** :  git에게 add하는 파일들을 관리하라고 알려주는 command, add된 파일들은 stage 영역에 대기하게 된다.
- **$ git rm --cached** : 원격 저장소에 있는 파일만 삭제하고, 실제 디스크에는 파일을 남겨두는 command
- **$ git commit** : stage영역에서 커밋대기하고 있는 파일들의 버전을 생성하는 command
- **$ git log** : 각 버전 확인 및 버전과 버전사이의 소스 차이점을 확인하는 command
- **$ git reset**  : 커밋을 취소한다. $ git reset [commit id]를 하면 해당 버전으로 돌아간다. <br>
                 옵션에 따라 영역취소를 달리 할 수 있다.

   Working directory  | Staging Area      | Respository
  |------------------| :----------------:|------------------:|
  |                  |                   |  git reset--soft  |
  |                  | git reset --mixed | git reset --mixed |
  | git reset --hard | git reset --hard  | git reset --hard  |

