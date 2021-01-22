Modified PythonAPI to plot ego vehicle position in the 2D map.

1. Include the following library path in `~/.bashrc` file.
```
export LD_LIBRARY_PATH=${LD_LIBRARY_PATH}:/usr/local/MATLAB/R2019b/bin/glnxa64/
```

2. Use `python3.7` virtual environment.
3. Run the following command one by one in multiple terminal inside the `PythonAPI/examples` folder.
```
./CarlaUE4.sh
python spawn_npc.py -n 500
python automatic_control_our.py -a Roaming
python no_rendering_mode.py
```
4. After generating 1000 corner position for the ego vehicle `no_rendering_mode.py` will be terminated.
5. You can see the ego vehicle positions in `./cache/no_rendering_mode/mymap.tga` file.
6. Here is a sample map.
![carlamap](https://user-images.githubusercontent.com/530250/105437961-cf2f1900-5cad-11eb-85a6-abef035cb4cc.png)
