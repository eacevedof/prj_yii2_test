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
    - Installing fxp/composer-asset-plugin (v1.1.1)
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
      - Installing yiisoft/yii2-app-advanced (2.0.6)
        Downloading: 100%         
    
    Created project in advanced
    Loading composer repositories with package information
    Installing dependencies (including require-dev)
    Reading bower.json of bower-asset/jquery (1.11.1)
    ...
  - Installing fzaninotto/faker (v1.5.0)
    Downloading: 100%         

  - Installing yiisoft/yii2-faker (2.0.3)
    Downloading: 100%         

    Writing lock file
    Generating autoload files    

    crea una carpeta en /home/ubuntu/workspace/advanced
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
    
  - Installing yiisoft/yii2-gii (2.0.4)
    Loading from cache

  - Installing fzaninotto/faker (v1.5.0)
    Loading from cache

  - Installing yiisoft/yii2-faker (2.0.3)
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
                