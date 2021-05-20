
### numpy, pandas, matplotlib, seaborn

conda update conda (or conda update --all)

conda create -n {name} python=3.x

conda activate {name}

conda install -c conda-forge opencv matplotlib jupyterlab scikit-image seaborn git

    1	conda deactivate base
    2	conda create --name kosa python=3.7.6
    3	conda activate kosa 
    4	pip install ipykernel
    5	python -m ipykernel install --user --name kosa --display-name "Python KOSA"
    6	conda install -c conda-forge jupyterlab
    7	conda install -c conda-forge jupyterlab

    8 conda env create -n kosa -f env_kosa.yaml
      
    #
    # To activate this environment, use
    #
    #     $ conda activate project1
    #
    # To deactivate an active environment, use
    #
    #     $ conda deactivate
    
    9   conda remove --name project1 --all
    
    참고자료
    https://velog.io/@tyhlife/%EC%95%84%EB%82%98%EC%BD%98%EB%8B%A4-%EA%B0%80%EC%83%81%ED%99%98%EA%B2%BD%EC%97%90%EC%84%9C-%EA%B0%9C%EB%B0%9C%ED%95%98%EA%B8%B0
    




