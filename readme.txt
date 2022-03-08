git clone https://github.com/paparazzi/paparazzi.git
cd paparazzi/
git checkout v6.1.0_stable 
make
(this will get messages.xml)


git clone https://github.com/enacuavlab/demo_utm.git
cd demo_utm
export PAPARAZZI_SRC= ...
export PAPARAZZI_HOME= ..
./restore.sh
(this will update messages.xml)


cd paparazzi
make
(this will compile with updated messages.xml)
./start.py
(Conf: userconf/ENAC/conf_enac.xml)
(Controlpanel: userconf/ENAC/control_panel.xml)


./paparazzi
Tools/PprzGCS


export PAPARAZZI_HOME= ..
./backup.sh
