# prj_yii2_test
Pruebas de: https://github.com/yiisoft/yii2.git

COMANDO EJECUTADO:
http://www.yiiframework.com/doc-2.0/index.html

global permite la ejecucion de otros comandos como si se estuviera en la carpeta composer 
$COMPOSER_HOME que dicho sea de paso: echo $COMPOSER_HOME no me imprime nada

fxp/composer-asset-plugin:~1.1.1 es un plugin que permite importar paquetes de librerias tipo css,js
almacenadas en repositorios tipo BOWER o NPM

composer global require "fxp/composer-asset-plugin:~1.1.1"
You are running composer with xdebug enabled. This has a major impact on runtime performance. See https://getcomposer.org/xdebug
Changed current directory to /home/ubuntu/.composer
You are running composer with xdebug enabled. This has a major impact on runtime performance. See https://getcomposer.org/xdebug
./composer.json has been created
Loading composer repositories with package information
Updating dependencies (including require-dev)
  - Installing fxp/composer-asset-plugin (v1.1.1)
    Downloading: 100%  

la carpeta .composer esta en /home/ubuntu/
y tiene esta estructura:

.
├── cache
│   ├── files
│   │   └── fxp
│   │       └── composer-asset-plugin
│   │           └── daca454b94539a4e6d30937dfc6b817eceb03f28.zip
│   └── repo
│       ├── https---bower.herokuapp.com-packages
│       ├── https---packagist.org
│       │   ├── p-provider-2013.json
│       │   ├── p-provider-2014.json
│       │   ├── p-provider-2015-04.json
│       │   ├── p-provider-2015-07.json
│       │   ├── p-provider-2015-10.json
│       │   ├── p-provider-2015.json
│       │   ├── p-provider-archived.json
│       │   ├── p-provider-latest.json
│       │   ├── packages.json
│       │   └── provider-fxp$composer-asset-plugin.json
│       └── https---registry.npmjs.org
├── composer.json
├── composer.lock
└── vendor
    ├── autoload.php
    ├── composer
    │   ├── ClassLoader.php
    │   ├── LICENSE
    │   ├── autoload_classmap.php
    │   ├── autoload_namespaces.php
    │   ├── autoload_psr4.php
    │   ├── autoload_real.php
    │   └── installed.json
    └── fxp
        └── composer-asset-plugin
            ├── AssetEvents.php
            ├── Assets.php
            ├── Composer
            │   └── ScriptHandler.php
            ├── Converter
            │   ├── AbstractPackageConverter.php
            │   ├── BowerPackageConverter.php
            │   ├── NpmPackageConverter.php
            │   ├── NpmPackageUtil.php
            │   ├── PackageConverterInterface.php
            │   ├── PackageUtil.php
            │   ├── SemverConverter.php
            │   ├── SemverRangeUtil.php
            │   ├── SemverUtil.php
            │   └── VersionConverterInterface.php
            ├── Event
            │   └── VcsRepositoryEvent.php
            ├── Exception
            │   └── InvalidCreateRepositoryException.php
            ├── FxpAssetPlugin.php
            ├── Installer
            │   ├── AssetInstaller.php
            │   ├── BowerInstaller.php
            │   ├── IgnoreFactory.php
            │   └── IgnoreManager.php
            ├── Package
            │   ├── AbstractLazyCompletePackage.php
            │   ├── LazyCompletePackage.php
            │   ├── LazyPackageInterface.php
            │   ├── Loader
            │   │   ├── LazyAssetPackageLoader.php
            │   │   └── LazyLoaderInterface.php
            │   └── Version
            │       └── VersionParser.php
            ├── README.md
            ├── Repository
            │   ├── AbstractAssetVcsRepository.php
            │   ├── AbstractAssetsRepository.php
            │   ├── AssetVcsRepository.php
            │   ├── BowerRepository.php
            │   ├── FilterUtil.php
            │   ├── NpmRepository.php
            │   ├── Util.php
            │   ├── Vcs
            │   │   ├── AbstractGitHubDriver.php
            │   │   ├── BitbucketUtil.php
            │   │   ├── GitBitbucketDriver.php
            │   │   ├── GitDriver.php
            │   │   ├── GitHubDriver.php
            │   │   ├── HgBitbucketDriver.php
            │   │   ├── HgDriver.php
            │   │   ├── PerforceDriver.php
            │   │   ├── ProcessUtil.php
            │   │   ├── SvnDriver.php
            │   │   └── Util.php
            │   └── VcsPackageFilter.php
            ├── Resources
            │   ├── doc
            │   │   ├── faqs.md
            │   │   ├── index.md
            │   │   └── schema.md
            │   └── meta
            │       └── LICENSE
            ├── Tests
            │   ├── AssetsTest.php
            │   ├── Composer
            │   │   └── ScriptHandlerTest.php
            │   ├── Converter
            │   │   ├── AbstractPackageConverterTest.php
            │   │   ├── BowerPackageConverterTest.php
            │   │   ├── NpmPackageConverterTest.php
            │   │   └── SemverConverterTest.php
            │   ├── Event
            │   │   └── VcsRepositoryEventTest.php
            │   ├── Fixtures
            │   │   ├── Converter
            │   │   │   └── InvalidPackageConverter.php
            │   │   ├── IO
            │   │   │   └── MockIO.php
            │   │   ├── Repository
            │   │   │   ├── MockAssetRepository.php
            │   │   │   └── Vcs
            │   │   │       ├── MockVcsDriver.php
            │   │   │       ├── MockVcsDriverSkipParsing.php
            │   │   │       ├── MockVcsDriverWithPackages.php
            │   │   │       └── MockVcsDriverWithUrlPackages.php
            │   │   └── package
            │   │       ├── bower.json
            │   │       └── npm.json
            │   ├── FxpAssetPluginTest.php
            │   ├── Installer
            │   │   ├── AssetInstallerTest.php
            │   │   ├── BowerInstallerTest.php
            │   │   ├── IgnoreFactoryTest.php
            │   │   └── IgnoreManagerTest.php
            │   ├── Package
            │   │   ├── LazyCompletePackageTest.php
            │   │   └── Loader
            │   │       └── LazyAssetPackageLoaderTest.php
            │   ├── Repository
            │   │   ├── AbstractAssetsRepositoryTest.php
            │   │   ├── AssetVcsRepositoryTest.php
            │   │   ├── BowerRepositoryTest.php
            │   │   ├── NpmRepositoryTest.php
            │   │   ├── UtilTest.php
            │   │   ├── Vcs
            │   │   │   ├── GitBitbucketDriverTest.php
            │   │   │   ├── GitDriverTest.php
            │   │   │   ├── GitHubDriverTest.php
            │   │   │   ├── HgBitbucketDriverTest.php
            │   │   │   ├── HgDriverTest.php
            │   │   │   ├── PerforceDriverTest.php
            │   │   │   ├── SvnDriverTest.php
            │   │   │   └── UtilTest.php
            │   │   └── VcsPackageFilterTest.php
            │   ├── Type
            │   │   ├── AbstractAssetTypeTest.php
            │   │   ├── BowerAssetTypeTest.php
            │   │   └── NpmAssetTypeTest.php
            │   ├── Util
            │   │   ├── PerforceTest.php
            │   │   └── ValidatorTest.php
            │   └── bootstrap.php
            ├── Type
            │   ├── AbstractAssetType.php
            │   ├── AssetTypeInterface.php
            │   ├── BowerAssetType.php
            │   └── NpmAssetType.php
            ├── Util
            │   ├── AssetPlugin.php
            │   ├── Perforce.php
            │   └── Validator.php
            ├── composer.json
            ├── composer.lock
            └── phpunit.xml.dist
