# Dynamical Systems
> DynamicalSystems.jl is an award-winning Julia software library for the exploration of chaos and nonlinear dynamics. It is part of JuliaDynamics, an organization dedicated to creating high quality scientific software. [:link:](https://juliadynamics.github.io/DynamicalSystems.jl/latest/)

## Installation
julia
using Pkg
Pkg.add("DynamicalSystems")


### install python evironment
```
sudo apt install -y python3-pip
sudo apt install build-essential libssl-dev libffi-dev python3-dev
sudo apt install -y python3-venv
python3.6 -m venv forjulia
source ~/forjulia/bin/activate
pip3 install matplotlib
```

### [PyPlot](https://github.com/JuliaPy/PyPlot.jl)
```
> You will need to have the Python Matplotlib library installed on your machine in order to use PyPlot
ENV["PYTHON"] = "~/forjulia/bin/python3.7"

using Pkg;
Pkg.add("PyPlot")
```


## References 
https://juliadynamics.github.io/DynamicalSystems.jl/latest/
