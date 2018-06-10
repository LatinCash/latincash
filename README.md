## This is the reference code for LatinCash cryptocurrency

* Official homepage: http://www.latincashcoin.com
* Official repository: https://github.com/LatinCash/
* Official Announcement thread: https://bitcointalk.org/index.php?topic=4389341.0
* Official Twitter: https://twitter.com/LatinCashCoin
* Official Discord: https://discordapp.com/invite/keez2rW
* Official Whitepaper:
* Official paper wallet generator: http://wallet.latincashcoin.com
* Official Mining Pool: http://pool.latincashcoin.com
* Official Block explorer: http://explorer.latincashcoin.com

## LatinCash Cryptocurrency

LatinCash [LCH] is an ASIC resistant CryptoNightLite V1 algorithm based cryptocurrency. 
Fast transactions & privacy make this coin perfect for rewarding your workers, co-workers and colleagues for a job well done.

- Algorithm: CryptoNightLite V1
- Max. supply: 50,000,000.00
- CryptoNote name: LatinCash
- Ticker: LCH
- Decimal points: 4
- Block time: 120
- Emission speed factor: 20
- P2P port: 20634
- RPC port: 20635


## How to compile

### Compile on Linux Ubuntu 16

**1. Install dependencies**

``
sudo apt-get update
``

``
sudo apt-get install -y build-essential python-dev gcc g++ git cmake librocksdb-dev libboost-all-dev
``

**2. Get the coin**

``
git clone https://github.com/LatinCash/latincash.git latincash
``

**3. CHMOD**

- navigate to:

``
cd latincash/external/rocksdb/build_tools
``

- execute the following commands:

``
chmod +x build_detect_platform
``

``
chmod +x version.sh
``

**4. Build executables**

- Navigate back to repo folder 

``
cd
``

``
cd latincash
``

``
mkdir build && cd $_
``

``
cmake ..
``

``
export CXXFLAGS="-std=gnu++11"
``

``
make
``

_Your executables will be located in `build/src` folder._


### Compile on Windows 7/8/10

**1. Environment**

- Visual Studio 2017 Community Edition with desktop development with C++ and the VC++ v140 toolchain features selected
- Boost 1.59.0, with the installer for MSVC 14 (tested with Boost 1.65.1)

**2. Build**

- From the start menu, open 'x64 Native Tools Command Prompt for vs2017'

``
cd <latincash_directory>
``

``
mkdir build
``

``
cd build
``


-  Set the PATH for Cmake:

``
set PATH="C:\Program Files (x86)\Microsoft Visual Studio\2017\Community\Common7\IDE\CommonExtensions\Microsoft\CMake\CMake\bin";%PATH%
``

- Run Cmake (Set correct location of your boost folder):

``
cmake -G "Visual Studio 14 Win64" .. -DBOOST_ROOT=C:\local\boost_1_59_0
``

- Build:

``
MSBuild LatinCash.sln /p:Configuration=Release /m
``

_Your binaries  will be located in `..\build\src\Release` folder._


### Credits
Cryptonote Developers, Bytecoin Developers, Monero Developers, Forknote Project, TurtleCoin Developers, Worktips Developers
