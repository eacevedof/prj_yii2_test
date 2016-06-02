# prj_yii2_test
INSTALANDO YII2 EN C9.io

Pruebas de: http://www.yiiframework.com/download/


TUTORIAL COMPOSER:
    http://www.yiiframework.com/doc-2.0/guide-start-installation.html#verifying-installation

    PASO 1: compruebo que hay en mis binarios. No hay nada
    
    tree /usr/local/bin/
    .
    
    0 directories, 0 files
    
    PASO 2: Ejecuto 
    sudo curl -sS https://getcomposer.org/installer | php
    
    PASO 3: 
    sudo mv composer.phar /usr/local/bin/composer
    chmod 7775 /usr/local/bin/composer 

    PASO 4: comprobar ultima version composer
    sudo composer self-update

    tree /usr/local/bin/
    
    /usr/local/bin/
    └── composer
    
INSTALANDO PLUGIN CONVERSOR DE PAQUETES PARA COMPOSER "fxp/composer-asset-plugin:~1.1.1"
    http://www.yiiframework.com/download/
    
    PASO 1: ejecuto
    php /usr/local/bin/composer global require "fxp/composer-asset-plugin:~1.1.1"
    
    RESULTADO:
    
    You are running composer with xdebug enabled. This has a major impact on runtime performance. See https://getcomposer.org/xdebug
    Changed current directory to /home/ubuntu/.composer
    You are running composer with xdebug enabled. This has a major impact on runtime performance. See https://getcomposer.org/xdebug
    ./composer.json has been created
    Loading composer repositories with package information
    Updating dependencies (including require-dev)
    Installing fxp/composer-asset-plugin (v1.1.1)
    Downloading: 100%         
    Writing lock file
    Generating autoload files

    tree /home/ubuntu/.composer
        cache/
            files/
                fxp/
                    composer-asset-plugin/
                        daca454b94539a4e6d30937dfc6b817eceb03f28.zip
            ...
        composer.json
        composer.lock
        vendor/
            autoload.php
            composer/
            fxp/
                composer-asset-plugin/
                ...
                
INSTALANDO LA APLICACION AVANZADA 
    http://www.yiiframework.com/download/
    php composer.phar create-project yiisoft/yii2-app-advanced advanced 2.0.6
    
    segun mi proyecto y la configuracion previa adapto la llamada al comando composer
    
    PASO 1: 
    php /usr/local/bin/composer create-project yiisoft/yii2-app-advanced advanced
    
    You are running composer with xdebug enabled. This has a major impact on runtime performance. See https://getcomposer.org/xdebug
    Installing yiisoft/yii2-app-advanced (2.0.6)
    Installing yiisoft/yii2-app-advanced (2.0.6)
    Downloading: 100%         
    
    Created project in advanced
    Loading composer repositories with package information
    Installing dependencies (including require-dev)
    Reading bower.json of bower-asset/jquery (1.11.1)
    ...
    
    Installing fzaninotto/faker (v1.5.0)
    Downloading: 100%         

    Installing yiisoft/yii2-faker (2.0.3)
    Downloading: 100%         

    Writing lock file
    Generating autoload files    

    crea una carpeta en:
        /home/ubuntu/workspace/advanced
            backend/
            common/
            console/
            enviroments/
            frontend/
            tests/
            vendor/
            ...
        
    NOTA:
        No entiendo muy bien esta instalación. No hay un archivo index que reciba
        todas las peticiones.
        02/06/2016 Me corrijo, existen 3 archivos index dos dentro de enviroments/ y uno en frontend/ que es la carpeta
        pública, a donde apunte la dirección raiz, es decir http://localhost/.
        Despues de configurar apache para que use esta carpeta se debe dar permisos a www-data:www-data ya que se necesitarán permisos de escritura en distintos subdirectorios de frontend. Uno de ellos es /runtime/logs/
        
INSTALANDO LA APLICACION BASICA  

    Dentro de /home/ubuntu/workspace
    
    PASO 1: Ejecuto
    php /usr/local/bin/composer create-project yiisoft/yii2-app-basic basic
    
    RESULTADO
    You are running composer with xdebug enabled. This has a major impact on runtime performance. See https://getcomposer.org/xdebug
    Installing yiisoft/yii2-app-basic (2.0.6)
      - Installing yiisoft/yii2-app-basic (2.0.6)
        Downloading: 100%         
    
    Created project in basic
    Loading composer repositories with package information
    Installing dependencies (including require-dev)
    
    ....
    
    Installing yiisoft/yii2-gii (2.0.4)
    Loading from cache
    
    Installing fzaninotto/faker (v1.5.0)
    Loading from cache
    
    Installing yiisoft/yii2-faker (2.0.3)
    Loading from cache

    Writing lock file
    Generating autoload files
    > yii\composer\Installer::postCreateProject
    chmod('runtime', 0777)...done.
    chmod('web/assets', 0777)...done.
    chmod('yii', 0755)...done.
    
    para verla en ejecucion:
        https://prj-yii2-test-ioedu.c9users.io/basic/web/index.php
        
        la ruta fisica a index.php es:
        workspace/
            basic/
                web/
                    index.php
                
RESUMEN
    Aunque parezca que van unidos, composer se debe instalar por separado en un entorno normal "no como aqui en c9" ya que
    te crea un workspace para cada proyecto obligandote a repetir la instalación de composer en cada uno de ellos.
    
    Primero se instala composer, que no es más que bajarse el archivo composer.phar (archivo php) y ejecutarlo
    este creara una carpeta ./composer a nivel global me imagino que es para llevar el historico de los paquetes
    que se van importanto y los plugins que se le van añadiendo.
    
    Entre los plugins necesarios para YII2 que necesita composer es fxp/composer-asset-plugin:~1.1.1
    es un tipo de helper que lo que hace es permitir la incorporacion de librerias css y js entre otras cosas
    alojadas en repositorios npm y bower
    
    Se puede seleccionar la instalación AVANZADA (,,,yiisoft/yii2-app-advanced <cualquier nombre de la carpeta de destino>) 
    o BÁSICA (...yiisoft/yii2-app-basic <cualquier nombre de la carpeta de destino>)
    
    No conseguí ponerla en ejecucion a la avanzada.
    
    Al ejecutar la instalación con composer sobre YII2 puede que necesite dependencias almacenadas en github
    para esto es necesario crearse un token en www.github.com:
    (tucuentadegithub>arribaderechaflechadedespliegue>settings>personal access tokens) ojo con esto que una vez
    que la crees no aparecera más, asi que guardala.
    
    Cuando en c9 te pida que falta un token 0Auth solo pega este contenido y presiona intro.
    Si da error empezaras a ver mensajes de invlidez del token y te lo volvera a pedir para la siguiente dependencia
    En este caso opté por cancelar la instalacion y reinstalar todo nuevamente.
    
    Puedo ver que YII2 así como otros tantos frameworks concentran las peticiones en su archivo index.php
    este se encuentra en la carpeta web, que entiendo deberia ser la carpeta virtual pública.
    
    
    
    
    
    
