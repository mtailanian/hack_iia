# hack_iia
Introducción a la Inteligencia Artificial - Curso Hack Academy

# Configuracion de entorno


Primero instalar python3.6:

En Ubuntu (Linux):
```
sudo apt-get install python3-pip python3-dev
```

Desde la Maquina Virtual distribuida con Ubuntu (Linux) sólo este comando:
```
sudo apt install python3-pip
```


En OSX debemos primero instalar Homebrew:
```
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```

Luego correr el siguiente comando en consola:
```
brew install https://raw.githubusercontent.com/Homebrew/homebrew-core/f2a764ef944b1080be64bd88dca9a1d80130c558/Formula/python.rb
```

Una vez instalado Python se debe continuar de la siguiente manera:
Desde consola crear un virtual environment con nombre "ha_env"
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
pip3 install -r requirements.txt
```


No olvidarse al terminar de trabajar ejecutar:
```
deactivate
```
