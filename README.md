# hack_iia
Introducción a la Inteligencia Artificial - Curso Hack Academy

# Configuracion de entorno


Primero instalar python3:
```
sudo apt-get install python3-pip python3-dev
```


En OSX debemos tener Homebrew, y luego es simplemente:
```
brew install python
brew postinstall python

brew install python3
brew postinstall python3
```


Luego crear un virtual environment con nombre "eikyou_env"
```
sudo pip3 install virtualenv
virtualenv -p python3 ha_env
```


Activar el VE:
```
source ha_env/bin/activate
```


Instalar las dependencias:
```
pip install -r requirements.txt
```


No olvidarse al terminar de trabajar ejecutar:
```
deactivate
```
