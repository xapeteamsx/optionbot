Termux cython compiled version bot for binomo

1. Download latest termux on F-Droid then run "pkg update"
2. pkg install build-essential clang make pkg-config binutils git wget python3
3. pkg install python-numpy ta-lib
4. pip install --upgrade pip
5. install TA-lib (manual)

# TA-Lib manual installation

# step 1
* wget http://prdownloads.sourceforge.net/ta-lib/ta-lib-0.4.0-src.tar.gz
* tar -xzvf ta-lib-0.4.0-src.tar.gz
* cd ta-lib/
* termux-fix-shebang configure
* ./configure --prefix=$PREFIX -build=arm
* make && make install

# step 2
* git clone https://github.com/mrjbq7/ta-lib
* cd ta-lib/
* python3 setup.py bdist_wheel
* cd dist/
* pip install TA_Lib-0.4.25-cp310-cp310-linux_aarch64.whl

6. edit setting.json enter all required fields
7. run "python3 main.py"
