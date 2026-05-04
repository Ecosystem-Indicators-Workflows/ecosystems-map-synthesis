
```sh

python3 -m venv .venv

source .venv/bin/activate

pip install --upgrade pip

pip install jupyterlab
pip install numpy pandas geopandas fiona matplotlib owslib folium basemap plotly altair
```

 and more..., then we do

```sh
pip freeze > requirements.txt
```


And we can use it to install the same modules in another environment:

```sh
pip install -r requirements.txt
```

In order to show leaflet maps and other widgets, 
install:

```sh
pip install jupyter-leaflet
pip install ipywidgets
```
And restart the server


For the bash kernel, we need to do these two steps:

```sh
pip install bash_kernel
python -m bash_kernel.install
```

In order to move data from/to Katana, we can set up [streamlined secure remote access](https://medium.com/@prateek.malhotra004/streamlining-secure-remote-access-a-guide-to-passwordless-ssh-connections-between-linux-servers-8c26bb008af9):

```sh
ssh-copy-id user@serverB_IP
```

for faster raster computation in R:

Package `velox` is outddated 

```sh
sudo add-apt-repository -y ppa:ubuntugis/ubuntugis-unstable
sudo apt-get update
sudo apt-get install libgdal-dev libproj-dev libgeos-dev libudunits2-dev
sudo apt-get upgrade
```

```R
require(devtools)
devtools::install_github('hunzikp/velox')
```

Let's use the other recommendation:

`exact_extract`