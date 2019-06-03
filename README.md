# BDE Flask App


The only tricky dependency here is [`rdkit`](http://www.rdkit.org/docs/Install.html), but it can be installed with 
```
conda install -c conda-forge rdkit
```


The dependencies are therefore
* rdkit
* pandas
* seaborn (for colors)
* flask
* wtforms

## To update submodules (add new compounds)
`git submodule foreach git pull origin master`

## To launch a local server:
```
cd bde_prediction
gunicorn --bind 0.0.0.0:2222 main:app
```

Then browse to 0.0.0.0:2222 in a web browser
