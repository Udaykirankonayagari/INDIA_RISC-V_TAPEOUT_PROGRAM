# WEEK-0
📝 Week 0: Toolchain Setup and Installation

The goal of this week was to set up the development environment by installing all the necessary open-source EDA tools for the SoC design flow.

### **System Requirements**

  * **OS:** Ubuntu 20.04 or higher
  * **vCPU:** 4 cores
  * **RAM:** 6 GB
  * **HDD:** 50 GB of free space

-----


### ** EDA Tool Installation**


#### **Icarus Verilog 
$ sudo apt-get update
$ sudo apt-get install iverilog
<img width="1327" height="689" alt="icarus" src="https://github.com/user-attachments/assets/58e25ab0-7b83-4ed4-9fc6-d2a943e4a7cd" />






 #### **GTKWave**
$ sudo apt-get update
$ sudo apt install gtkwave
<img width="1863" height="512" alt="gtkwave" src="https://github.com/user-attachments/assets/b9bfbd0d-25a8-42cc-8a29-810601d92ee5" />



#### **Yosys (Synthesis Tool)**
 $ sudo apt-get update
$ git clone https://github.com/YosysHQ/yosys.git
$ cd yosys
$ sudo apt install make               # If make is not installed
$ sudo apt-get install build-essential clang bison flex \
    libreadline-dev gawk tcl-dev libffi-dev git \
    graphviz xdot pkg-config python3 libboost-system-dev \
    libboost-python-dev libboost-filesystem-dev zlib1g-dev
$ make config-gcc
# Yosys build depends on a Git submodule called abc, which hasn't been initialized yet. You need to run the following command before running make
$ git submodule update --init --recursive
$ make 
$ sudo make install

<img width="1341" height="624" alt="yosys" src="https://github.com/user-attachments/assets/05d1c527-8cd0-491d-b395-684fbf8b0512" />

