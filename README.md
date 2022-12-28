### miniconda & jupyter 설치하는법
1. [miniconda 다운로드](https://docs.conda.io/en/latest/miniconda.html)

2. [microsoft terminal 다운로드](https://apps.microsoft.com/store/detail/windows-terminal/9N0DX20HK701?hl=ko-kr&gl=kr)

3. https://windowsterminalthemes.dev/ 에서 원하는 theme 다운로드

4. 환경변수 -> 시스템변수에서 miniconda script 파일까지 추가

![miniconda01](https://user-images.githubusercontent.com/114986610/209664244-8a65d0e7-a986-4182-85c4-851c168b3af8.png)

5. (관리자권한 powershell에서) Set-ExecutionPolicy RemoteSigned 

6. (conda prompt에서) conda init powershell

7. (다운받은 terminal에서) conda config --set auto_activate_base False 

8. conda activate <<< (다음 실행할때는 conda activate mldl-env)\
conda env list\
conda create -n mldl-env python=3.8    <<<<    가상환경 설치 (install은 경로가 아닌 어느 가상환경에 설치할것인지가 중요)\
conda install numpy\
conda install pandas\
conda install matplotlib\
conda install jupyter\
conda install scikit-learn\
conda list\

9. (원하는 경로로 간다음) jupyter notebook  <<<<  jupyter 실행


### jupyter 기본사용법
- 편집모드
  - ctrl + 엔터 = 현재 행 실행
  - shift + 엔터 = 현재 행 실행하고 다음 행 생성

- 커맨드모드
  - dd = 현재 행 삭제
  - a = (현재 행 기준) 앞쪽에 새 행 생성
  - b = (현재 행 기준) 뒤쪽에 새 행 생성