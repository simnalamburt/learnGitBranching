LearnGitBranching 한국어 번역 프로젝트
========

![screenshot][]

**LearnGitBranching** 는 git 교육용으로 만들어진 git 저장소 시각화, 샌드박스,
튜토리얼, 퀴즈 프로젝트입니다. 한때 한국어로 완전하게 [번역되었었지만][urigit],
2년이라는 세월동안 번역이 원작 업데이트를 못쫓아가서 한글화 비율이 50% 밑으로
떨어져버렸습니다. 그래서 이번 기회에 다시 한글화를 완료하고자 해요.

관심 있으신분들의 많은 참여 부탁드립니다.

### 빌드하는법

```sh
npm install -g grunt-cli
npm install

grunt fastBuild     # skips tests and linting, faster build
grunt build         # runs tests and lint
```

### 한글화 방침

1.  *당장은* 번역의 질은 심각하게 고민하지 않고, 한글화 커버리지를 100%로 만드는데에 집중하고자 합니다.

1.  Git 고유한 용어의 번역은 실무에서 쓰이는 말이나, [Git 공식 튜토리얼][git]에 쓰인 표기법으로 하는것을 원칙으로 하고자 합니다.

1.  가급적이면 diff를 원본과 conflict를 발생시키지 않는 방향으로 만들고자 합니다.

1.  원문에 쓰여있는 농담이나 말장난, 영화 대사 패러디 등은 최대한 살릴 수 있도록 노력하고자 합니다.

    *ex)* `src/levels/index.js`의 [123번째 줄][example], 토이스토리 버즈 라이트이어의 대사 패러디

    |                   |             영어           |              한글           |
    |------------------:|:--------------------------:|:---------------------------:|
    |        토이스토리 | To Infinity, and Beyond!   | 무한한 공간, 저 너머로!     |
    | LearnGitBranching | To **Origin**, and Beyond! | **원격** 저장소, 저 너머로! |

--------

### TODOs

- [x] src/js/dialogs/confirmShowSolution.js
- [x] src/js/dialogs/levelBuilder.js
- [x] src/js/dialogs/nextLevel.js
- [x] src/js/dialogs/sandbox.js
- [ ] src/js/intl/strings.js
- [ ] src/levels/advanced/multipleParents.js
- [x] src/levels/index.js
- [x] src/levels/intro/branching.js
- [x] src/levels/intro/commits.js
- [ ] src/levels/intro/merging.js
- [ ] src/levels/intro/rebasing.js
- [ ] src/levels/mixed/describe.js
- [ ] src/levels/mixed/grabbingOneCommit.js
- [ ] src/levels/mixed/jugglingCommits.js
- [ ] src/levels/mixed/jugglingCommits2.js
- [ ] src/levels/mixed/tags.js
- [ ] src/levels/rampup/cherryPick.js
- [ ] src/levels/rampup/detachedHead.js
- [ ] src/levels/rampup/interactiveRebase.js
- [ ] src/levels/rampup/relativeRefs.js
- [ ] src/levels/rampup/relativeRefs2.js
- [ ] src/levels/rampup/reversingChanges.js
- [ ] src/levels/rebase/manyRebases.js
- [ ] src/levels/rebase/selectiveRebase.js
- [ ] src/levels/remote/clone.js
- [ ] src/levels/remote/fakeTeamwork.js
- [ ] src/levels/remote/fetch.js
- [ ] src/levels/remote/fetchArgs.js
- [ ] src/levels/remote/fetchRebase.js
- [ ] src/levels/remote/mergeManyFeatures.js
- [ ] src/levels/remote/pull.js
- [ ] src/levels/remote/pullArgs.js
- [ ] src/levels/remote/push.js
- [ ] src/levels/remote/pushArgs.js
- [ ] src/levels/remote/pushArgs2.js
- [ ] src/levels/remote/pushManyFeatures.js
- [ ] src/levels/remote/remoteBranches.js
- [ ] src/levels/remote/sourceNothing.js
- [ ] src/levels/remote/tracking.js

[urigit]: https://github.com/urigit/learnGitBranching
[screenshot]: assets/learnGitBranching.png
[git]: http://git-scm.com/book/ko/
[example]: https://github.com/simnalamburt/learnGitBranching/blob/master-korean/src/levels/index.js#L123
