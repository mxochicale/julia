# Installing and testing Julia
Installation of Julia following [instructrions](https://julialang.org/downloads/platform.html)

## 1. Download julia
Go to https://julialang.org/downloads/ and download the verison 
for your machine OS and arquitecture

```
cd ~/Downloads
wget https://julialang-s3.julialang.org/bin/linux/x64/1.3/julia-1.3.0-linux-x86_64.tar.gz
tar xvfa julia-*
```

Alternatively, you can try:


```
sudo add-apt-repository ppa:staticfloat/juliareleases
sudo add-apt-repository ppa:staticfloat/julia-deps
sudo apt-get update
sudo apt-get install julia
```


## 2. Create symbolic link

```
sudo ln -s ~/Downloads/julia-1.3.0/bin/julia /usr/local/bin/julia
```



### WARNNING 

adding this line in `.profile`
```
PATH=\$PATH:~/julia-1.2.0/bin/
```
create a problem of a login loop 
which was sorted out by commenting such line


## 3. Add packages
open terminal, then load julia:
```
julia
using Pkg; Pkg.add("IJulia")
using IJulia
using Pkg; Pkg.add("DynamicalSystems")
using DynamicalSystems
using Pkg; Pkg.add("Images");
using Images
import Pkg; Pkg.add("ImageMagick")
using ImageMagick
```

## 4. Hello world
```
julia
using IJulia
notebook()
install Jupyter via Conda, y/n? [y]: y
```

## References
https://blog.simos.info/learning-the-julia-computer-language-on-ubuntu/
https://julialang.org/downloads/
