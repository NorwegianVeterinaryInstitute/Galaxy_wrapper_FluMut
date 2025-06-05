# Installation FluMut

- [FluMut git](https://github.com/izsvenezie-virology/FluMut)
- is available via bioconda

- created flumut.yml to install in conda

# Installation in saga

```bash
cd /cluster/projects/nn9305k/src/miniconda/yaml_files
cp /cluster/projects/nn9305k/active/evezeyl/VIGAS-P/Galaxy_wrapper_FluMut/flumut_conda_recipe/flumut_0.6.4.yml .

miniconda
conda env create -f flumut_0.6.4.yml

conda activate flumut_0.6.4
cd test 
# flumut -x test.xlsm EPI_ISL_18933204.fasta
flumut -m markers_output.tsv -M mutations_output.tsv -l literature_output.tsv EPI_ISL_18933204.fasta
conda deactivate
```

It is working

- Now need to do the galaxy xml file
