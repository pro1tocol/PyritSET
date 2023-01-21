# Pyrit fine configuration

--------------------------

### Prerequisite plugins (based on debian)

    apt-get install pip libpcap-dev python2-dev libffi-dev libssl-dev libxml2-dev libxslt1-dev zlib1g-dev
#### Download [pyrit](https://github.com/JPaulMora/Pyrit)

    git clone https://github.com/JPaulMora/Pyrit.git
    
    cd pyrit/
    sed -i "s/COMPILE_AESNI/COMPILE_AESNIX/" ./cpyrit/_cpyrit_cpu.c
#### Build and install

    python2 setup.py clean
    python2 setup.py build
    python2 setup.py install
#### Test

    pyrit list_cores
    
    reboot
