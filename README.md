# about this image
* Debian 9 where Jupyter Lab installed
* Jupyter setting
```/root/.jupyter/jupyter_notebook_config.py 
c.NotebookApp.allow_root = True  
c.NotebookApp.ip = '*'  
c.NotebookApp.open_browser = False  
c.NotebookApp.notebook_dir = '/notebook'  
c.NotebookApp.token = 'pass'  
```
---
# Notes
* build  
```sh:console
 sudo docker build -t sin1/jupyter .  
```
* run
```sh:console
 sudo docker run -itd -v "/notebook:/notebook" -p "8888:8888" --name notebook sin1/jupyter
```

---

# Software dependencies
| Software component | version |
|:-----------|:------------|
| jupyter | 4.3.0 |
| python2 | 2.7.13 |
| python3 | 3.5.3 |
| R | 3.3.3 |
| ruby | 2.3.3 |
| julia | 0.6.0 |
| node.js | 4.8.2 |
| octave | 4.0.3 |
| swi-prolog | 7.2.3 |
| Glasgow Haskell Compiler | 8.0.2 |
| GNU Compiler Collection | 6.3.0 |
