# OBS-PYTHON
*Just a portable version of Python for ease of use with OBS scripts.*

I didn't create anything, simply assembled embedded Python 3.6.7

***Made for use with https://github.com/tryptech/obs-zoom-and-follow script.***

#### EASY MODE
1. Download [OBS PYTHON.ZIP](https://github.com/Mushiiies/OBS-PYTHON/files/8596758/OBS.PYTHON.zip "Pre-made portable version of Python 3.6.7")
2. Extract `OBS PYTHON` Folder to wherever you want it.
3. Launch OBS and Click on `Tools->Scripts->Python Settings` Set `OBS PYTHON` as the Python Directory.
4. On `Scripts` Tab, now Click the [+] to add a new script, select `zoom_and_follow_mouse.py`


Follow [tryptech's instructions](https://github.com/tryptech/obs-zoom-and-follow "Zoom and Follow Git") to set up the script settings.

#### MAKE IT YOURSELF
If you would prefer to set this up yourself

1. [Download Python Embed](https://www.python.org/ftp/python/3.6.7/python-3.6.7-embed-amd64.zip "Python 3.6.7 Embedded")
 Extract contents to a folder eg 

```C:\OBS PYTHON\```

2. [Download suitable PIP](https://bootstrap.pypa.io/pip/3.6/get-pip.py "Python 3.6 PIP")
Put PIP in Python folder

```C:\OBS PYTHON\get-pip.py```

3.Edit `python36._pth` with text editor as follow:
```
python36.zip
.

# Uncomment to run site.main() automatically
import site
Lib\site-packages
```

4. Open Command prompt as Administrator. Enter the following:

```
CD C:\OBS PYTHON
python.exe get-pip.py
python.exe -m pip install pywinctl
python.exe -m pip install pynput
python.exe -m pip install screeninfo
```

5. [Download Zoom and Follow Script](https://github.com/tryptech/obs-zoom-and-follow "Zoom and Follow Git")

6. Launch OBS

Navigate the menu:

`Tools->Scripts->Python Settings->[Python Install Path]`
Point it at your Python folder `C:/OBS PYTHON`.

7. Add the Zoom and follow script!
8. Make coffee.
