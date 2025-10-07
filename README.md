<<<<<<< HEAD
# ReactEx
리액트 배포 연습& README 작성 연습
=======
# React + Vite

This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.

Currently, two official plugins are available:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react) uses [Babel](https://babeljs.io/) for Fast Refresh
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react-swc) uses [SWC](https://swc.rs/) for Fast Refresh

## Expanding the ESLint configuration

If you are developing a production application, we recommend using TypeScript with type-aware lint rules enabled. Check out the [TS template](https://github.com/vitejs/vite/tree/main/packages/create-vite/template-react-ts) for information on how to integrate TypeScript and [`typescript-eslint`](https://typescript-eslint.io) in your project.
>>>>>>> 02a5025 (Initial commit)

# 리액트 bash 배포를 위한 명령어와 에러 

user@DESKTOP-9R0N82A MINGW64 ~/Desktop/BackEend/React/36.React_File upload_download
$ git config --global user.name na (이름 상관x)

user@DESKTOP-9R0N82A MINGW64 ~/Desktop/BackEend/React/36.React_File upload_download (main)        
$ git config --global user.email oooo14@gmail.com (내 깃허브 계정)

user@DESKTOP-9R0N82A MINGW64 ~/Desktop/BackEend/React/36.React_File upload_download (main)
$ git add.(add . 공백후 .이여야함)
git: 'add.' is not a git command. See 'git --help'.

The most similar command is
        add

user@DESKTOP-9R0N82A MINGW64 ~/Desktop/BackEend/React/36.React_File upload_download (main)
$ git commit -m react 배포연습 (커밋메시지)
error: pathspec '배포연습' did not match any file(s) known to git

user@DESKTOP-9R0N82A MINGW64 ~/Desktop/BackEend/React/36.React_File upload_download (main)
$ git remote add origin https://github.com/mi-yeon777/ReactEx.git

user@DESKTOP-9R0N82A MINGW64 ~/Desktop/BackEend/React/36.React_File upload_download (main)
$ git branch -M main

user@DESKTOP-9R0N82A MINGW64 ~/Desktop/BackEend/React/36.React_File upload_download (main)        
$ git push -u origin main
error: src refspec main does not match any
error: failed to push some refs to 'https://github.com/mi-yeon777/ReactEx.git'
(ㄴ>이 에러 메시지는 Git에서 
main 브랜치가 현재 로컬에 존재하지 않거나 커밋이 없는 상태에서 push를 시도했을 때 발생. 
단계별로 확인하고 해결할 수 있다.)

user@DESKTOP-9R0N82A MINGW64 ~/Desktop/BackEend/React/36.React_File upload_download (main)        
$ git push -u origin main
error: src refspec main does not match any
error: failed to push some refs to 'https://github.com/mi-yeon777/ReactEx.git'

user@DESKTOP-9R0N82A MINGW64 ~/Desktop/BackEend/React/36.React_File upload_download (main)        
$ git log (커밋이 있는지 확인 커밋이 하나도 없으면 push 할수 없다. 커밋이 없으면 먼저 커밋)
fatal: your current branch 'main' does not have any commits yet

user@DESKTOP-9R0N82A MINGW64 ~/Desktop/BackEend/React/36.React_File upload_download (main)        
$ git commit -m Initial commit (커밋)
error: pathspec 'commit' did not match any file(s) known to git
(왜 에러?->아래 보면 "안에"입력하면 커밋메시지 들어간다.)

user@DESKTOP-9R0N82A MINGW64 ~/Desktop/BackEend/React/36.React_File upload_download (main)        
$ git add.
git: 'add.' is not a git command. See 'git --help'.

The most similar command is
        add

user@DESKTOP-9R0N82A MINGW64 ~/Desktop/BackEend/React/36.React_File upload_download (main)        
$ git commit -m Initial commit
error: pathspec 'commit' did not match any file(s) known to git

user@DESKTOP-9R0N82A MINGW64 ~/Desktop/BackEend/React/36.React_File upload_download (main)        
$ git commit -m "Initial commit"(커밋 메시지 들어감 커밋시작)
[main (root-commit) 02a5025] Initial commit
 27 files changed, 5029 insertions(+)
 create mode 100644 .gitignore
 create mode 100644 README.md
 create mode 100644 eslint.config.js
 create mode 100644 index.html
 create mode 100644 package-lock.json
 create mode 100644 package.json
 create mode 100644 public/vite.svg
 create mode 100644 src/App.css
 create mode 100644 src/App.jsx
 create mode 100644 src/assets/react.svg
 create mode 100644 src/components/CommonApp.jsx
 create mode 100644 src/components/jpa/JpaApp.jsx
 create mode 100644 src/components/jpa/JpaBoardDetail.jsx
 create mode 100644 src/components/jpa/JpaBoardList.jsx
 create mode 100644 src/components/jpa/JpaBoardWrite.jsx
 create mode 100644 src/components/legacy/BoardDetail.jsx
 create mode 100644 src/components/legacy/BoardList.jsx
 create mode 100644 src/components/legacy/BoardWrite.jsx
 create mode 100644 src/components/legacy/LegacyApp.jsx
 create mode 100644 src/components/legacy/Login.jsx
 create mode 100644 src/components/rest/RestApp.jsx
 create mode 100644 src/components/rest/RestBoardDetail.jsx
 create mode 100644 src/components/rest/RestBoardList.jsx
 create mode 100644 src/components/rest/RestBoardWrite.jsx
 create mode 100644 src/index.css
 create mode 100644 src/main.jsx
 create mode 100644 vite.config.js

user@DESKTOP-9R0N82A MINGW64 ~/Desktop/BackEend/React/36.React_File upload_download (main)
$ git push -u origin main(푸시. 정상적으로 푸시되면 이제 로컬 main 브랜치가 원격 main 브랜치와 연결됨)
info: please complete authentication in your browser...
To https://github.com/mi-yeon777/ReactEx.git
 ! [rejected]        main -> main (fetch first)
error: failed to push some refs to 'https://github.com/mi-yeon777/ReactEx.git'
hint: Updates were rejected because the remote contains work that you do not
hint: have locally. This is usually caused by another repository pushing to
hint: the same ref. If you want to integrate the remote changes, use
hint: 'git pull' before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.
(이 에러는 원격(GitHub)의 main 브랜치에 이미 커밋이 있어서, 로컬 main과 맞지 않기 때문에 발생한 것. 
Git은 자동으로 덮어쓰기를 하지 않아서 막은 상태.

즉, 원격에 이미 초기 커밋(예: README.md)이 있고, 
로컬에도 커밋이 있지만 서로 연결되어 있지 않은 상황.)

user@DESKTOP-9R0N82A MINGW64 ~/Desktop/BackEend/React/36.React_File upload_download (main)        
$ git pull origin main --rebase
(--rebase를 사용하면 로컬 커밋이 원격 커밋 뒤로 정리돼서 깔끔하게 올라감)
remote: Enumerating objects: 3, done.
remote: Counting objects: 100% (3/3), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
Unpacking objects: 100% (3/3), 878 bytes | 67.00 KiB/s, done.
From https://github.com/mi-yeon777/ReactEx
 * branch            main       -> FETCH_HEAD
 * [new branch]      main       -> origin/main
Auto-merging README.md
CONFLICT (add/add): Merge conflict in README.md
error: could not apply 02a5025... Initial commit
hint: Resolve all conflicts manually, mark them as resolved with
hint: "git add/rm <conflicted_files>", then run "git rebase --continue".
hint: You can instead skip this commit: run "git rebase --skip".
hint: To abort and get back to the state before "git rebase", run "git rebase --abort".
hint: Disable this message with "git config set advice.mergeConflict false"
Could not apply 02a5025... # Initial commit

user@DESKTOP-9R0N82A MINGW64 ~/Desktop/BackEend/React/36.React_File upload_download (main|REBASE 1/1)
$ git push -u origin main(푸시)
To https://github.com/mi-yeon777/ReactEx.git
 ! [rejected]        main -> main (non-fast-forward)
error: failed to push some refs to 'https://github.com/mi-yeon777/ReactEx.git'(에러)
hint: Updates were rejected because a pushed branch tip is behind its remote
hint: counterpart. If you want to integrate the remote changes, use 'git pull'
hint: before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.

user@DESKTOP-9R0N82A MINGW64 ~/Desktop/BackEend/React/36.React_File upload_download (main|REBASE 1/1)
$ git rebase --continue(충돌을 해결하면 다시 이어 진행하는 명령어)
README.md: needs merge
You must edit all merge conflicts and then
mark them as resolved using git add

user@DESKTOP-9R0N82A MINGW64 ~/Desktop/BackEend/React/36.React_File upload_download (main|REBASE 1/1)
$ git add.
git: 'add.' is not a git command. See 'git --help'.

The most similar command is
        add

user@DESKTOP-9R0N82A MINGW64 ~/Desktop/BackEend/React/36.React_File upload_download (main|REBASE 1/1)
$ git add . (공백 . 맞음)

user@DESKTOP-9R0N82A MINGW64 ~/Desktop/BackEend/React/36.React_File upload_download (main|REBASE 1/1)
$ git rebase --continue
hint: Waiting for your editor to close the file... 
[detached HEAD 9617164] Initial commit
 27 files changed, 5032 insertions(+)
 create mode 100644 .gitignore
 create mode 100644 eslint.config.js
 create mode 100644 index.html
 create mode 100644 package-lock.json
 create mode 100644 package.json
 create mode 100644 public/vite.svg
 create mode 100644 src/App.css
 create mode 100644 src/App.jsx
 create mode 100644 src/assets/react.svg
 create mode 100644 src/components/CommonApp.jsx
 create mode 100644 src/components/jpa/JpaApp.jsx
 create mode 100644 src/components/jpa/JpaBoardDetail.jsx
 create mode 100644 src/components/jpa/JpaBoardList.jsx
 create mode 100644 src/components/jpa/JpaBoardWrite.jsx
 create mode 100644 src/components/legacy/BoardDetail.jsx
 create mode 100644 src/components/legacy/BoardList.jsx
 create mode 100644 src/components/legacy/BoardWrite.jsx
 create mode 100644 src/components/legacy/LegacyApp.jsx
 create mode 100644 src/components/legacy/Login.jsx
 create mode 100644 src/components/rest/RestApp.jsx
 create mode 100644 src/components/rest/RestBoardDetail.jsx
 create mode 100644 src/components/rest/RestBoardList.jsx
 create mode 100644 src/components/rest/RestBoardWrite.jsx
 create mode 100644 src/index.css
 create mode 100644 src/main.jsx
 create mode 100644 vite.config.js

user@DESKTOP-9R0N82A MINGW64 ~/Desktop/BackEend/React/36.React_File upload_download (main|REBASE 1/1)
$ git rebase --continue --no-edit
error: unknown option `no-edit'
usage: git rebase [-i] [options] [--exec <cmd>] [--onto <newbase> | --keep-base] [<upstream> [<branch>]]
   or: git rebase [-i] [options] [--exec <cmd>] [--onto <newbase>] --root [<branch>]
   or: git rebase --continue | --abort | --skip | --edit-todo

    --[no-]onto <revision>
                          rebase onto given branch instead of upstream
    --[no-]keep-base      use the merge-base of upstream and branch as the current base
    --no-verify           allow pre-rebase hook to run
    --verify              opposite of --no-verify
    -q, --[no-]quiet      be quiet. implies --no-stat
    -v, --[no-]verbose    display a diffstat of what changed upstream
    -n, --no-stat         do not show diffstat of what changed upstream
    --stat                opposite of --no-stat
    --[no-]signoff        add a Signed-off-by trailer to each commit
    --[no-]committer-date-is-author-date
                          make committer date match author date
    --[no-]reset-author-date
                          ignore author date and use current date
    -C <n>                passed to 'git apply'
    --[no-]ignore-whitespace
                          ignore changes in whitespace
    --[no-]whitespace <action>
                          passed to 'git apply'
    -f, --[no-]force-rebase
                          cherry-pick all commits, even if unchanged
    --no-ff               cherry-pick all commits, even if unchanged
    --ff                  opposite of --no-ff
    --continue            continue
    --skip                skip current patch and continue
    --abort               abort and check out the original branch
    --quit                abort but keep HEAD where it is
    --edit-todo           edit the todo list during an interactive rebase
    --show-current-patch  show the patch file being applied or merged
    --apply               use apply strategies to rebase
    -m, --merge           use merging strategies to rebase
    -i, --interactive     let the user edit the list of commits to rebase
    --[no-]rerere-autoupdate
                          update the index with reused conflict resolution if possible
    --empty (drop|keep|stop)
                          how to handle commits that become empty
    --[no-]autosquash     move commits that begin with squash!/fixup! under -i
    --[no-]update-refs    update branches that point to commits that are being rebased
    -S, --[no-]gpg-sign[=<key-id>]
                          GPG-sign commits
    --[no-]autostash      automatically stash/stash pop before and after
    -x, --[no-]exec <exec>
                          add exec lines after each commit of the editable list
    -r, --[no-]rebase-merges[=<mode>]
                          try to rebase merges instead of skipping them
    --[no-]fork-point     use 'merge-base --fork-point' to refine upstream
    -s, --[no-]strategy <strategy>
                          use the given merge strategy
    -X, --[no-]strategy-option <option>
                          pass the argument through to the merge strategy
    --[no-]root           rebase all reachable commits up to the root(s)
    --[no-]reschedule-failed-exec
                          automatically re-schedule any `exec` that fails
    --[no-]reapply-cherry-picks
                          apply all changes, even those already present upstream


user@DESKTOP-9R0N82A MINGW64 ~/Desktop/BackEend/React/36.React_File upload_download (main|REBASE 1/1)
$

user@DESKTOP-9R0N82A MINGW64 ~/Desktop/BackEend/React/36.React_File upload_download (main|REBASE 1/1)
$
Display all 936 possibilities? (y or n)
!
./
:
[
[.exe
[[
]]
___git_complete
__git
__git_aliased_command
__git_checkout_default_dwim_mode
__git_complete
__git_complete_command
__git_complete_common
__git_complete_config_variable_name
__git_complete_config_variable_name_and_value
__git_complete_config_variable_value
__git_complete_fetch_refspecs
__git_complete_file
__git_complete_force_with_lease
__git_complete_index_file
__git_complete_log_opts
__git_complete_refs
__git_complete_remote_or_refspec
__git_complete_revlist
__git_complete_revlist_file
__git_complete_strategy
__git_complete_symbol
__git_complete_worktree_paths
__git_compute_all_commands
__git_compute_config_sections
__git_compute_config_vars
__git_compute_config_vars_all
__git_compute_first_level_config_vars_for_section
__git_compute_merge_strategies
__git_compute_second_level_config_vars_for_section
__git_config_get_set_variables
__git_count_arguments
__git_count_path_components
__git_dequote
__git_dwim_remote_heads
__git_eread
__git_find_last_on_cmdline
__git_find_on_cmdline

user@DESKTOP-9R0N82A MINGW64 ~/Desktop/BackEend/React/36.React_File upload_download (main|REBASE 1/1)
$ tinue --no-edit
bash: tinue: command not found

user@DESKTOP-9R0N82A MINGW64 ~/Desktop/BackEend/React/36.React_File upload_download (main|REBASE 1/1)
$ git rebase --continue --no-edit
(--no-edit 옵션을 쓰면 편집기 열지 않고 Git이 자동으로 기존 메시지를 사용합니다.
충돌 해결 후 바로 rebase를 진행할 수 있어 편리합니다.)

error: unknown option `no-edit'
usage: git rebase [-i] [options] [--exec <cmd>] [--onto <newbase> | --keep-base] [<upstream> [<branch>]]
   or: git rebase [-i] [options] [--exec <cmd>] [--onto <newbase>] --root [<branch>]
   or: git rebase --continue | --abort | --skip | --edit-todo

    --[no-]onto <revision>
                          rebase onto given branch instead of upstream
    --[no-]keep-base      use the merge-base of upstream and branch as the current base
    --no-verify           allow pre-rebase hook to run
    --verify              opposite of --no-verify
    -q, --[no-]quiet      be quiet. implies --no-stat
    -v, --[no-]verbose    display a diffstat of what changed upstream
    -n, --no-stat         do not show diffstat of what changed upstream
    --stat                opposite of --no-stat
    --[no-]signoff        add a Signed-off-by trailer to each commit
    --[no-]committer-date-is-author-date
                          make committer date match author date
    --[no-]reset-author-date
                          ignore author date and use current date
    -C <n>                passed to 'git apply'
    --[no-]ignore-whitespace
                          ignore changes in whitespace
    --[no-]whitespace <action>
                          passed to 'git apply'
    -f, --[no-]force-rebase
                          cherry-pick all commits, even if unchanged
    --no-ff               cherry-pick all commits, even if unchanged
    --ff                  opposite of --no-ff
    --continue            continue
    --skip                skip current patch and continue
    --abort               abort and check out the original branch
    --quit                abort but keep HEAD where it is
    --edit-todo           edit the todo list during an interactive rebase
    --show-current-patch  show the patch file being applied or merged
    --apply               use apply strategies to rebase
    -m, --merge           use merging strategies to rebase
    -i, --interactive     let the user edit the list of commits to rebase
    --[no-]rerere-autoupdate
                          update the index with reused conflict resolution if possible
    --empty (drop|keep|stop)
                          how to handle commits that become empty
    --[no-]autosquash     move commits that begin with squash!/fixup! under -i
    --[no-]update-refs    update branches that point to commits that are being rebased
    -S, --[no-]gpg-sign[=<key-id>]
                          GPG-sign commits
    --[no-]autostash      automatically stash/stash pop before and after
    -x, --[no-]exec <exec>
                          add exec lines after each commit of the editable list
    -r, --[no-]rebase-merges[=<mode>]
                          try to rebase merges instead of skipping them
    --[no-]fork-point     use 'merge-base --fork-point' to refine upstream
    -s, --[no-]strategy <strategy>
                          use the given merge strategy
    -X, --[no-]strategy-option <option>
                          pass the argument through to the merge strategy
    --[no-]root           rebase all reachable commits up to the root(s)
    --[no-]reschedule-failed-exec
                          automatically re-schedule any `exec` that fails
    --[no-]reapply-cherry-picks
                          apply all changes, even those already present upstream


user@DESKTOP-9R0N82A MINGW64 ~/Desktop/BackEend/React/36.React_File upload_download (main|REBASE 1/1)
$ git status (충동 난 파일 표시)

interactive rebase in progress; onto 69f6116
Last command done (1 command done):
   pick 02a5025 # Initial commit
No commands remaining.
You are currently editing a commit while rebasing branch 'main' on '69f6116'.
  (use "git commit --amend" to amend the current commit)
  (use "git rebase --continue" once you are satisfied with your changes)

nothing to commit, working tree clean

user@DESKTOP-9R0N82A MINGW64 ~/Desktop/BackEend/React/36.React_File upload_download (main|REBASE 1/1)
$ git rebase --continue(계속 진행)
Successfully rebased and updated refs/heads/main.

user@DESKTOP-9R0N82A MINGW64 ~/Desktop/BackEend/React/36.React_File upload_download (main)        
$ git push -u origin main (rebase 완료 후 푸시)
Enumerating objects: 38, done.
Counting objects: 100% (38/38), done.
Delta compression using up to 2 threads
Compressing objects: 100% (33/33), done.
Writing objects: 100% (36/36), 41.75 KiB | 1.44 MiB/s, done.
Total 36 (delta 7), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (7/7), done.
To https://github.com/mi-yeon777/ReactEx.git
   69f6116..9617164  main -> main
branch 'main' set up to track 'origin/main'.

user@DESKTOP-9R0N82A MINGW64 ~/Desktop/BackEend/React/36.React_File upload_download (main)        
$

user@DESKTOP-9R0N82A MINGW64 ~/Desktop/BackEend/React/36.React_File upload_download (main)        
$
