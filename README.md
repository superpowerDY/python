# DY Python

?집에서 git하기

-- 맨 처음 git 실행하면 할 일
	1. 집 컴에 git bash 다운로드
	2. 임의의 폴더를 만들어서 마우스 우클릭 -> git bash 클릭
	3. 밑의 명령어 순서대로 입력
		git config --global user.name "깃허브 계정 이름" --superpowerDY
		git config --global user.email "깃허브 계정 이메일"
		git clone https://github.com/superpowerDY/python.git
		
	4. git bash 화면에 아래처럼 (master) 표시 뜨는지 확인 (표시 떠야함)
		-- TJ@DESKTOP-J2LIGQ3 MINGW64 /d/weekend/learn_python (master)

	5. 2번에서 만든 임의의 폴더에 python 문서가 제대로 다운됐는지 확인!
	6. 복습~

-- Git에 있는 자료 내 컴퓨터에 다운 받기
	1. 처음에 만든 임의의 폴더에 마우스 우클릭 -> git bash
	2. git pull 명령어 입력
		-- 중간에 깃 계정 로그인창 뜰 수 있음 로그인 해주면 됨
	3. 임의의 폴더에 자료 다운됐는지 확인

-- 내 컴퓨터에 있는 자료 Git에 업로드하기
	1. 처음에 만든 임의의 폴더에 마우스 우클릭 -> git bash 클릭
	2. 밑의 명령어 순서대로 입력
		git status
			--현재 내가 작업한 파일이 어떤 게 있는지 보여주는 명령어
				-- 빨간글씨 : git에 올려야 할 파일
				-- 초록글씨 : git에 올릴 준비가 끝난 파일
				-- 흰 글씨만 뜬다 = git에 있는 자료랑 내 컴터에 있는 자료가 동일 = 올릴 자료가 없다는 것
		git add *
			-- 빨간 글씨로 뜨는 모든 파일을 git에 업로드하고 싶을 때 사용
			-- 파일 중에 골라서 업로드하고 싶을 때
				git add 특정파일이름 (-- git add 치고 tab키누르면 알아서 자동완성해줌)
				
		git commit -m "어떤 작업을 했는지 메세지 작성하여 이력 남기기" 
			-- (ex) git commit -m "Update python data type list"
		
		git push origin master
			-- git에 업로드하는 명령어
			-- 중간에 깃 계정 로그인창 뜰 수 있음 로그인 해주면 됨
			-- 이거 하고 깃페이지 확인해보면 파일 업로드 되어 있을 것~!