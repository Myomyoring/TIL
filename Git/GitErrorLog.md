[1]

현재 브랜치 main
현재 브랜치와 'origin/main'이(가) 갈라졌습니다,
다른 커밋이 각각 1개와 3개 있습니다.
  (리모트의 브랜치를 현재 브랜치로 병합하려면 "git pull"을 사용하십시오)

커밋하도록 정하지 않은 변경 사항:
  (무엇을 커밋할지 바꾸려면 "git add <파일>..."을 사용하십시오)
  (use "git restore <file>..." to discard changes in working directory)
	수정함:        .DS_Store

커밋할 변경 사항을 추가하지 않았습니다 ("git add" 및/또는 "git commit -a"를
사용하십시오)

이 상태에서 푸쉬할 경우,

To   
 ! [rejected]        main -> main (non-fast-forward   
error: 레퍼런스를 에 푸시하는데 실패했습니다   
힌트: 현재 브랜치의 끝이 리모트 브랜치보다 뒤에 있으므로 업데이트가
힌트: 거부되었습니다.   
푸시하기 전에 ('git pull ...' 등 명령으로) 리모트
힌트: 변경 사항을 포함하십시오.   
힌트: 자세한 정보는 'git push --help'의 "Note about fast-forwards' 부분을
힌트: 참고하십시오.

<br>

- 원인



- 해결방법
[참고 사이트](https://velog.io/@eunddodi/git-pull-%EC%8B%9C-%EB%B0%9C%EC%83%9D%ED%95%98%EB%8A%94-warning-%ED%95%B4%EA%B2%B0%ED%95%98%EA%B8%B0Need-to-specify-how-to-reconcile-divergent-branches)

<br>

[2]

Need to specify how to reconcile divergent branches.
	
[3]

remote: Write access to repository not granted. unable to access '(repo url)': The requested URL returned error: 403   
	
- 원인 : 나의 경우엔 토큰 만료로 인한 에러!


- 해결방법 : 토큰 재발급 후, git remote set-url origin https://{token}@github.com/{git_repository_url} 


[4]


	
- 원인 : 


- 해결방법 : 
