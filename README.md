# prj_yii2_test
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
    
    