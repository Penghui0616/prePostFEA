# prePostFEA
A general pre and post process framework for finite element analysis, such as ABAQUS, OpenSees et al.

[![GitHub](https://img.shields.io/github/license/Junjun1guo/prePostFEA?color=red&logoColor=blue)](https://github.com/Junjun1guo/prePostFEA/blob/master/LICENSE)
[![GitHub Pipenv locked Python version](https://img.shields.io/github/pipenv/locked/python-version/Junjun1guo/prePostFEA)](https://www.python.org/downloads/release/python-368/)
![GitHub top language](https://img.shields.io/github/languages/top/Junjun1guo/prePostFEA)
[![GitHub Pipenv locked dependency version](https://img.shields.io/github/pipenv/locked/dependency-version/Junjun1guo/prepostFEA/numpy)](https://numpy.org/)
[![GitHub Pipenv locked dependency version](https://img.shields.io/github/pipenv/locked/dependency-version/Junjun1guo/prepostFEA/pyvista)](https://docs.pyvista.org/)
[![GitHub Pipenv locked dependency version](https://img.shields.io/github/pipenv/locked/dependency-version/Junjun1guo/prepostFEA/records)](https://github.com/kennethreitz-archive/records)
![GitHub repo size](https://img.shields.io/github/repo-size/Junjun1guo/prePostFEA?color=GREEN)
![GitHub stars](https://img.shields.io/github/stars/Junjun1guo/prePostFEA)
![GitHub last commit](https://img.shields.io/github/last-commit/Junjun1guo/prePostFEA)

<img width="390" height="300" src="https://github.com/Junjun1guo/prePostFEA/blob/master/misesStress.gif"/><img width="390" height="300" src="https://github.com/Junjun1guo/prePostFEA/blob/master/dispForce.gif"/>

## Usage 
1. __Generate finite element model__. If use commercial software,such as ABAQUS, you can write python script to establish FEM(referring __abaqusPythonScript.py__). If use open source software, such as OpenSees, you can also write python script to generate the input file(referring __abaqusPythonScript.py__). In additon, for two or three dimensional problems, [pygmsh](https://github.com/nschloe/pygmsh) can be used to mesh the model.       
2. __outPut process__. If use commercial software,such as ABAQUS, you can write python script to read the output database(referring __abaqusODBProcess.py__).If use open source software, such as OpenSees, you can process the output files and save data to [pysqlite](https://github.com/ghaering/pysqlite) database(referring __saveDataToSqlite.py__).    
3. __result display__. [pyvista](https://docs.pyvista.org/) is adopted to generate static and dynamic graphs(referring __prePostProcess.py__).


 
