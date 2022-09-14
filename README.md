# TestGame

Steps to install cocos2d (Linux):
```
sudo apt-get install python2-minimal git curl g++ libgdk-pixbuf2.0-dev cmake libx11-dev libxmu-dev libglu1-mesa-dev libgl2ps-dev libxi-dev libzip-dev libpng-dev libcurl4-gnutls-dev libfontconfig1-dev libsqlite3-dev libglew-dev libssl-dev libgtk-3-dev libglfw3 libglfw3-dev xorg-dev

curl https://bootstrap.pypa.io/pip/2.7/get-pip.py --output get-pip.py
sudo python2 get-pip.py

cd <to where you want to clone this repo>

git clone https://github.com/cocos2d/cocos2d-x.git

python2 download-deps.py

cd cocos2d-x
git submodule update --init
git submodule update
```

Setting up cocos2d:
```
cd cocos2d-x
python2 ./setup.py
source ~/.bashrc

cocos -v # this command should be successful and show the version of Cocos2d
```

Compile and run the game:
```
git clone git@github.com:argnux/game.git # to clone this repository
cd game

cocos compile -s . -p linux -m release -o ./bin # to build

./bin/TestGame          # just run
cocos run -s . -p linux # build and run
```