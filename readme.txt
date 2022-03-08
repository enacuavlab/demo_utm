git clone https://github.com/paparazzi/paparazzi.git
cd paparazzi/
git checkout v6.1.0_stable 
make



git clone https://github.com/enacuavlab/demo_utm.git
cd demo_utm
export PAPARAZZI_SRC= ...
export PAPARAZZI_HOME= ..
./restore.sh

export PAPARAZZI_SRC=$PWD
export PAPARAZZI_HOME=$PWD
make
./start.py
(Conf: userconf/ENAC/conf_enac.xml)
(Controlpanel: userconf/ENAC/control_panel.xml)

./paparazzi

./backup.sh
