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
                
    
