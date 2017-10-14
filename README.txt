This is an open source project - UMDlte, started by Telecommunication graduates at the University of Maryland,College park.
It's a feature enhancement project of srsLTE - open-source LTE software suite developed by SRS (www.softwareradiosystems.com).

It includes:
srsUE - a complete SDR LTE UE application featuring all layers from PHY to IP
srsENB - a complete SDR LTE eNodeB application
a highly modular set of common libraries for PHY, MAC, RLC, PDCP, RRC, NAS, S1AP and GW layers.

Focus of the project is to enhance relase 8 stack to release 1o, itegrated it on the hardware testbed and add GUI functionalities for configuration.

Getting Started

    Mandatory requirements:
        Common:
            cmake https://cmake.org/
            libfftw http://www.fftw.org/
            PolarSSL/mbedTLS https://tls.mbed.org
        srsUE:
            Boost: http://www.boost.org
        srsENB:
            Boost: http://www.boost.org
            lksctp: http://lksctp.sourceforge.net/
            config: http://www.hyperrealm.com/libconfig/

For example, on Ubuntu 17.04, one can install the required libraries with:

sudo apt-get install cmake libfftw3-dev libmbedtls-dev libboost-all-dev libconfig++-dev libsctp-dev

Note that depending on your flavor and version of Linux, the actual package names may be different.

    Optional requirements:
        srsgui: https://github.com/srslte/srsgui - for real-time plotting.
        VOLK: https://github.com/gnuradio/volk - if the VOLK library and headers are detected, they will be used to accelerate some signal processing functions.

    RF front-end driver:
        UHD: https://github.com/EttusResearch/uhd
        BladeRF: https://github.com/Nuand/bladeRF

Download and build srsLTE:

git clone https://github.com/umdLTE/umdLTE.git
cd umdLTE
mkdir build
cd build
cmake ../
make 

The software suite can also be installed using the command sudo make install.

License
This project is licensed under under the AGPLv3 license and uses software from the OpenLTE project as well.

Thank you srsLTE and openLTE for great open source platform.

