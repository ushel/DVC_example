# DVC_example

stage_01 -> Creating a file (artifact.txt)
stage_02 -> Reading file and printing it

if we run stage_02.py file without running stage_01 then it will give an error, hence we need to execute in sequence.

It uses DAG stage_01 -> stage_02

``` bash 
conda environment create

 conda create -n dvc_demo python=3.7 -y

 conda activate dvc_demo

 pip install dvc

 for DVC running


 1. git init

 2. dvc init

 3. touch dvc.yml (create a dvc.yml file)

 4. dvc repro

 if files are already present it will not try to execute again.