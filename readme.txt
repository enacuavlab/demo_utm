git clone --recurse-submodules https://github.com/enacuavlab/demo_utm.git
cd demo_utm
./restore.sh

cd paparazzi
export PAPARAZZI_SRC=$PWD
export PAPARAZZI_HOME=$PWD
make
./start.py
(Conf: userconf/ENAC/conf_enac.xml)
(Controlpanel: userconf/ENAC/control_panel.xml)

./paparazzi

./backup.sh
