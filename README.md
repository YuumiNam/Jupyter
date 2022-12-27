### miniconda & jupyter 설치하는법
1. [miniconda 다운로드](https://docs.conda.io/en/latest/miniconda.html)

2. [microsoft terminal 다운로드](https://apps.microsoft.com/store/detail/windows-terminal/9N0DX20HK701?hl=ko-kr&gl=kr)

3. https://windowsterminalthemes.dev/ 에서 원하는 theme 다운로드

4. 환경변수 -> 시스템변수에서 miniconda script 파일까지 추가

![miniconda01](https://user-images.githubusercontent.com/114986610/209664244-8a65d0e7-a986-4182-85c4-851c168b3af8.png)
5. (관리자권한 powershell에서) Set-ExecutionPolicy RemoteSigned

6. (conda prompt에서) conda init powershell

7. (다운받은 terminal에서) conda config --set auto_activate_base False

8. conda activate <<< (다음 실행할때는 conda activate mldl-env) \ conda env list \ conda create -n mldl-env python=3.8  <<<<  가상환경 설치 (install은 경로가 아닌 어느 가상환경에 설치할것인지가 중요) \
conda install numpy \
conda install pandas \
conda install matplotlib \
conda install jupyter \
conda install scikit-learn \
conda list

pip install mglearn \
conda install graphviz  --->  (환경변수에서 -> 시스템변수 추가) C:\Users\BIT\miniconda3\envs\ml-env\Lib\site-packages\graphviz

conda install tensorflow \
conda install seaborn

9. (원하는 경로로 간다음) jupyter notebook  <<<<  jupyter 실행
