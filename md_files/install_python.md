sudo add-apt-repository ppa:deadsnakes/ppa
sudo apt-get update
sudo apt-get install python3.10.4 - version !!!

# tar -xvf file

# ./configure --prefix=/home/userpro/.python3.11 --enable-optimizations

make -j8 (8-count cpu)

sudo make altinstall

in file ~/.zshrc:
add
export PATH=/home/rusdev/.python3.11/bin:%PATH
