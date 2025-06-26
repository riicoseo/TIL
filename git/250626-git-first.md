# Git 기초 정리

## 목차
1. Git이란?
2. Git 기본 용어
3. Git 설정
4. Git 명령어
5. Git 브랜치
6. Git 원격 저장소 연결 및 동기화


---

## 1. Git이란?
- **Git**은 버전 관리 시스템(VCS, Version Control System)의 하나로, 코드 변경 이력을 추적하고 여러 명이 동시에 개발할 수 있도록 도와주는 도구입니다.
- 분산형 시스템으로, 각각의 개발자가 전체 저장소를 로컬에 보유합니다.

---


## 2. Git 기본 용어
- **Repository (저장소)**: 프로젝트의 전체 히스토리를 담는 곳
- **Working Directory**: 현재 작업 중인 디렉토리
- **Staging Area (Index)**: 커밋할 파일을 임시 저장하는 영역
- **Commit**: 변경 사항을 저장소에 기록하는 작업
- **Branch**: 독립적으로 개발을 진행할 수 있는 공간
- **Merge**: 다른 브랜치의 변경 사항을 현재 브랜치에 반영

---

## 3. Git 설정
```bash
# 사용자 정보 설정
git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"

# 설정 확인
git config --list


## 4. Git 명령어 

# 저장소 초기화
git init

# 현재 상태 확인
git status

# 파일 스테이징
git add filename          # 특정 파일 추가
git add .                # 전체 변경 사항 추가

# 커밋
git commit 


## 5. Git 브랜치 

# 브랜치 목록 보기
git branch

# 브랜치 생성
git branch new-branch-name

# 브랜치 전환
git switch new-branch
git checkout new-branch

# 브랜치 병합
git checkout main
git merge new-branch

# 브랜치 삭제
git branch -d new-branch

## 6. Git 원격 저장소 연결 및 동기화
# 원격 저장소 정보 확인
git remote -v

# 푸시 (로컬 → 원격)
git push origin main

# 신규 브랜치 최초 푸시 (새로운 브랜치명과 연결)
git push -u origin main

# 원격 저장소 내용 가져오기
git pull origin main

# 원격 저장소에서 클론
git clone https://github.com/username/repo.git




