# prj_yii2_test
Pruebas de: https://github.com/yiisoft/yii2.git

COMANDO EJECUTADO:
http://www.yiiframework.com/doc-2.0/index.html

global permite la ejecucion de otros comandos como si se estuviera en la carpeta composer 
$COMPOSER_HOME que dicho sea de paso: echo $COMPOSER_HOME no me imprime nada

fxp/composer-asset-plugin:~1.1.1 es un plugin que permite importar paquetes de librerias tipo css,js
almacenadas en repositorios tipo BOWER o NPM

php composer.phar create-project yiisoft/yii2-app-advanced advanced 2.0.6

You are running composer with xdebug enabled. This has a major impact on runtime performance. See https://getcomposer.org/xdebug
Installing yiisoft/yii2-app-advanced (2.0.6)
  - Installing yiisoft/yii2-app-advanced (2.0.6)
    Downloading: 100%         
Created project in advanced
Loading composer repositories with package information
Installing dependencies (including require-dev)
  - Installing yiisoft/yii2-composer (2.0.3)               
    Downloading: 100%         
  - Installing ezyang/htmlpurifier (v4.6.0)
    Downloading: 100%         

  - Installing cebe/markdown (1.1.0)
    Downloading: 100%         

  - Installing bower-asset/jquery (2.1.4)
    Downloading: 100%         

  - Installing bower-asset/jquery.inputmask (3.1.63)
    Downloading: 100%         

  - Installing bower-asset/punycode (v1.3.2)
    Downloading: 100%         

  - Installing bower-asset/yii2-pjax (v2.0.5)
    Downloading: 100%         

  - Installing yiisoft/yii2 (2.0.6)
    Downloading: 100%         

  - Installing swiftmailer/swiftmailer (v5.4.1)
    Downloading: 100%         
  - Installing yiisoft/yii2-swiftmailer (2.0.4)
    Downloading: 100%         
  - Installing yiisoft/yii2-codeception (2.0.4)
    Downloading: 100%         

  - Installing bower-asset/bootstrap (v3.3.5)
    Downloading: 100%         
  - Installing yiisoft/yii2-bootstrap (2.0.5)
    Downloading: 100%         

  - Installing yiisoft/yii2-debug (2.0.5)
    Downloading: 100%         

  - Installing bower-asset/typeahead.js (v0.10.5)
    Downloading: 100%         

  - Installing phpspec/php-diff (v1.0.2)
    Downloading: 100%         

  - Installing yiisoft/yii2-gii (2.0.4)
    Downloading: 100%         

  - Installing fzaninotto/faker (v1.5.0)
    Downloading: 100%         

  - Installing yiisoft/yii2-faker (2.0.3)
    Downloading: 100%         

Writing lock file
Generating autoload files

la carpeta .composer esta en /home/ubuntu/
y tiene esta estructura:

.
├── auth.json
├── cache
│   ├── files
│   │   ├── bower-asset
│   │   │   ├── bootstrap
│   │   │   │   └── 16b48259a62f576e52c903c476bd42b90ab22482.zip
│   │   │   ├── jquery
│   │   │   │   └── 7751e69b615c6eca6f783a81e292a55725af6b85.zip
│   │   │   ├── jquery.inputmask
│   │   │   │   └── c40c7287eadc31e341ebbf0c02352eb55b9cbc48.zip
│   │   │   ├── punycode
│   │   │   │   └── 38c8d3131a82567bfef18da09f7f4db68c84f8a3.zip
│   │   │   ├── typeahead.js
│   │   │   │   └── 5f198b87d1af845da502ea9df93a5e84801ce742.zip
│   │   │   └── yii2-pjax
│   │   │       └── 6818718408086db6bdcf33649cecb86b6b4f9b67.zip
│   │   ├── cebe
│   │   │   └── markdown
│   │   │       └── 54a2c49de31cc44e864ebf0500a35ef21d0010b2.zip
│   │   ├── ezyang
│   │   │   └── htmlpurifier
│   │   │       └── 6f389f0f25b90d0b495308efcfa073981177f0fd.zip
│   │   ├── fxp
│   │   │   └── composer-asset-plugin
│   │   │       └── daca454b94539a4e6d30937dfc6b817eceb03f28.zip
│   │   ├── fzaninotto
│   │   │   └── faker
│   │   │       └── d0190b156bcca848d401fb80f31f504f37141c8d.zip
│   │   ├── phpspec
│   │   │   └── php-diff
│   │   │       └── 30e103d19519fe678ae64a60d77884ef3d71b28a.zip
│   │   ├── swiftmailer
│   │   │   └── swiftmailer
│   │   │       └── 0697e6aa65c83edf97bb0f23d8763f94e3f11421.zip
│   │   └── yiisoft
│   │       ├── yii2
│   │       │   └── f42b2eb80f61992438661b01d0d74c6738e2ff38.zip
│   │       ├── yii2-app-advanced
│   │       │   └── b54472b89aea3660daece638a26f292c0b1f97d5.zip
│   │       ├── yii2-bootstrap
│   │       │   └── 1464f93834b1d5edb1f5625f7ffd6c3723fa4923.zip
│   │       ├── yii2-codeception
│   │       │   └── de5007e7a99359597abbfe1c88dca3ce620061c5.zip
│   │       ├── yii2-composer
│   │       │   └── ca8d23707ae47d20b0454e4b135c156f6da6d7be.zip
│   │       ├── yii2-debug
│   │       │   └── 1b302e67521d46feb2413d9d96ca94ed82b39b0e.zip
│   │       ├── yii2-faker
│   │       │   └── b88ca69ee226a3610b2c26c026c3203d7ac50f6c.zip
│   │       ├── yii2-gii
│   │       │   └── e5a023e8779bd774194842ec1b8fb4917cf04007.zip
│   │       └── yii2-swiftmailer
│   │           └── 4ec435a89e30b203cea99770910fb5499cb3627a.zip
│   └── repo
│       ├── github.com
│       │   ├── RobinHerbots
│       │   │   └── jquery.inputmask
│       │   │       ├── bower-03e65a2d28159e885e18acee9cae53ac6318372b
│       │   │       ├── bower-0c6ce85c1bc12e81ecb0df62fbc62db116b7b53d
│       │   │       ├── bower-1a863a0c9b733444f6766e5500eaf79b7b1d1d03
│       │   │       ├── bower-1d2a93fd4890ec65056b84136326ec8d7f484ca8
│       │   │       ├── bower-1e42949fd544abcc69027a7b52f55118df90360d
│       │   │       ├── bower-1e667db21e878105686e636efea883fa23b54fb2
│       │   │       ├── bower-2b485a3f9329c829b40872e4463c42143b0c6405
│       │   │       ├── bower-4551607fef63fd4bcd675479a8c347b668b915eb
│       │   │       ├── bower-464cddbdea65411896468f40321e68abcc75a34c
│       │   │       ├── bower-4a0bda47031b9d2074b0c77c3b447df71ed1ca95
│       │   │       ├── bower-5a27823c7964c6549ed5e74fd09e20c6d8650c53
│       │   │       ├── bower-5c2bce1ee4c1f3a91451b7d4b4f84c4708b51518
│       │   │       ├── bower-6afe1c66735b96dd45303b67152917cbbfa4d087
│       │   │       ├── bower-6c2445b82237de27ad26164e51197445abd856b9
│       │   │       ├── bower-6e8da117ea81168ac8d3b12206a20fad73f8e3d8
│       │   │       ├── bower-6fcd2cf28ee111f8aadcd42a1b8d43d6f7a5c0ba
│       │   │       ├── bower-70b4cd4d470d31c1b44bb6412d1146a4b9ed48a7
│       │   │       ├── bower-711ae3e5a8820bea1b35a67a98546a75861a448f
│       │   │       ├── bower-8579f56b86f78accbaf03c28d44be35ca1e346a5
│       │   │       ├── bower-88442b35ea76ef8923dde15ee9909ea482a794d6
│       │   │       ├── bower-9c2c236cf29b3e78b635f2ba3c588174336d9228
│       │   │       ├── bower-9e6df14484e1ca4ca1aaafcd403b488ddba6fd20
│       │   │       ├── bower-9ff37e85bc2fa2350475c4a7fa60aa20cd211481
│       │   │       ├── bower-a76f4bcbc4b2c9f6677fbcf2d5bdee8871c84db6
│       │   │       ├── bower-b63baffc42eca7833af60322ebd4575b2c9b83b2
│       │   │       ├── bower-b656c5b61b05d2a479b69b20de5bc01b837a43c5
│       │   │       ├── bower-b8f06eef3ccf9b8009607f30d47f66133670afc2
│       │   │       ├── bower-ba392f1c9c1f7a05d1b89a5e49cbd0610face768
│       │   │       ├── bower-bb776eb7e7be594fa77d5598e6f89d96029a8bac
│       │   │       ├── bower-c40c5c0abaf42b35139cdf97569b1ef1fad3a3d9
│       │   │       ├── bower-c40c7287eadc31e341ebbf0c02352eb55b9cbc48
│       │   │       ├── bower-c533c154ade0d641bf0815b76c7ff70ce96421ab
│       │   │       ├── bower-c95fe993f91e1da2069a26d84eaa372835842286
│       │   │       ├── bower-d180082aa1ba98c85f85b2c4eebbfa195fd25613
│       │   │       ├── bower-d90a0d180495635e8dd97a770e7ab8b3c4ee6d53
│       │   │       ├── bower-d9ebcf6ce4be6bd8642a10c633fe950c0c0f0a9d
│       │   │       ├── bower-da0a365b45b3040219a83c5abb5fcd3a51d7ed89
│       │   │       ├── bower-da1a274cefa18a52a0519ac7ffe8e8d31e950eae
│       │   │       ├── bower-dc1039e8b08fee22aca2003c4559530ce111f947
│       │   │       ├── bower-dd44bc88e7728cf9fdc509a98b58b99aa619de98
│       │   │       ├── bower-dffa7d6dcb9f279b6df93407f7a76f7044528933
│       │   │       ├── bower-e4663d15120fc820407f72a17dd958e885735ace
│       │   │       ├── bower-ebd3493bfbe032aa568c3574546402a60edd3ce5
│       │   │       ├── bower-f29e2b535028bde8e1135deb65cb5ed2e081cf39
│       │   │       ├── bower-f2c086411d2557fc485c47afb3cecfa6c1de9ee2
│       │   │       ├── bower-f44d5deec804c72fe85da31819b18bdcdad26f65
│       │   │       ├── bower-f48d10463039a23469e65cc4b5c0b4409e8fb596
│       │   │       └── bower-faf19625822fbd54765d26baac3154cd132769d1
│       │   ├── bestiejs
│       │   │   └── punycode.js
│       │   │       ├── bower-38c8d3131a82567bfef18da09f7f4db68c84f8a3
│       │   │       ├── bower-40e15ef43a44fdcb2b60fb631384168ef8e0181f
│       │   │       └── bower-de452f89aea23f126f7b219f576abda1c0823825
│       │   ├── jquery
│       │   │   └── jquery-dist
│       │   │       ├── bower-0d5ec2d8ac94a419ee47a39319c43ff9a7326b50
│       │   │       ├── bower-1472290917f17af05e98007136096784f9051fab
│       │   │       ├── bower-16b079b164d62bd807c612806842a13bf9b04d17
│       │   │       ├── bower-17eeebb3c04c72e5d00520c191cce858844aedec
│       │   │       ├── bower-2c62b787b2cafb32af14edadc963b8ba3cb847b8
│       │   │       ├── bower-4dec426aa2a6cbabb1b064319ba7c272d594a688
│       │   │       ├── bower-5876377b700b1bd26390a0a6d81e978dd822af14
│       │   │       ├── bower-617d181a45cff58586888550955a9c7fe2eb8b41
│       │   │       ├── bower-6361fdf2f30e41f565a953eb120f795774c65c4e
│       │   │       ├── bower-6fc01e29bdad0964f62ef56d01297039cdcadbe5
│       │   │       ├── bower-7751e69b615c6eca6f783a81e292a55725af6b85
│       │   │       ├── bower-84dd5fbd2fd29e8fd174d0fd074ac87eaa15c084
│       │   │       ├── bower-869704ba067c9b444bb052140581a426a45baaf5
│       │   │       ├── bower-873bfd84860f946ddca86d4ac87e422abf19ec1d
│       │   │       ├── bower-8f2a9d9272d6ed7f32d3a484740ab342c02541e0
│       │   │       ├── bower-91cd1587ed4a1d4f3834227e8eb3cc30cb385409
│       │   │       ├── bower-935eb19d87063ec30b717b3d45368d3c73cb591d
│       │   │       ├── bower-9434e03193c45d51bbd063a0edd1a07a6178d33f
│       │   │       ├── bower-9690801db01709bfbff5f977d07fb7cc14472908
│       │   │       ├── bower-9e6393b0bcb52b15313f88141d0bd7dd54227426
│       │   │       ├── bower-a04f5ff9795fd6292117563623db44cf3f875868
│       │   │       ├── bower-a0a3e5ee7f8025a498ba6daf26c2823518e96b2e
│       │   │       ├── bower-a55c5eeb709b584f58a1f3d8d0bc9f1432cd998a
│       │   │       ├── bower-adc1841f8032c33c647d061815d4455d968baa2d
│       │   │       ├── bower-d71f6a53927ad02d728503385d15539b73d21ac8
│       │   │       ├── bower-efbdc6e3f0fa3d3cd4d3d8bfa37990b707f7c2e1
│       │   │       └── bower-f852e631ba85af7da4ad7594785e122504e7b233
│       │   ├── twbs
│       │   │   └── bootstrap
│       │   │       ├── bower-1409cde7e800ca83fd761f87e5ad8f0d259e38d1
│       │   │       ├── bower-16b48259a62f576e52c903c476bd42b90ab22482
│       │   │       ├── bower-16dbdbd7a2c6cfa3be4e5dcc52249e577c02c84a
│       │   │       ├── bower-81df608a40bf0629a1dc08e584849bb1e43e0b7a
│       │   │       ├── bower-9a7e365c2c4360335d25246dac11afb1f577210a
│       │   │       ├── bower-a10eb60bc0b07b747fa0c4ebd8821eb7307bd07f
│       │   │       ├── bower-a365d8689c3f3cee7f1acf86b61270ecca8e106d
│       │   │       ├── bower-bcf7dd38b5ab180256e2e4fb5da0369551b3f082
│       │   │       └── bower-c068162161154a4b85110ea1e7dd3d7897ce2b72
│       │   ├── twitter
│       │   │   └── typeahead.js
│       │   │       ├── bower-5ac126185a5d762407ae77cad3a21dc0e60ad0e6
│       │   │       ├── bower-5f198b87d1af845da502ea9df93a5e84801ce742
│       │   │       ├── bower-8daea184f4be3461712c56ea5ca7436b21a66f9c
│       │   │       ├── bower-99dfe14852f459faaa30b574b7cc19a3f3c6450f
│       │   │       ├── bower-d5402b3b62c3659a9107c014ba56322ff17ab170
│       │   │       └── bower-ec7ae83b2c61eaa9e3db82d64601aced1f41d416
│       │   └── yiisoft
│       │       └── jquery-pjax
│       │           ├── bower-3f20897307cca046fca5323b318475ae9dac0ca0
│       │           ├── bower-6818718408086db6bdcf33649cecb86b6b4f9b67
│       │           ├── bower-d35c0a8fca20c61c6c2bd7276ecd06b714a6bebc
│       │           ├── bower-f07ce95f6098c0bd5421789a20789f39a19be73b
│       │           └── bower-fb92be865c0fd6583714475cb7d629020749d73f
│       ├── https---bower.herokuapp.com-packages
│       │   ├── bootstrap-3c71cc99d2fc1c12a3d3e1b27e448ca612a89a1d-package.json
│       │   ├── jquery-6f2ab963b5a51d155d69ac091e52e506d1055057-package.json
│       │   ├── jquery.inputmask-b8e5e0ff9fbec8c146a9c92c6cc82b6f1b82ec99-package.json
│       │   ├── punycode-ffb47d11fa9966e57dadaa196f53e7184de53477-package.json
│       │   ├── typeahead.js-665dbadca05dcd772922b7ef32a1a6a407597cac-package.json
│       │   └── yii2-pjax-44573c3d154e0699e14e713b6ef655231e2a63e1-package.json
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
│       │   ├── provider-bower-asset$bootstrap.json
│       │   ├── provider-bower-asset$jquery.inputmask.json
│       │   ├── provider-bower-asset$jquery.json
│       │   ├── provider-bower-asset$punycode.json
│       │   ├── provider-bower-asset$yii2-pjax.json
│       │   ├── provider-cebe$markdown.json
│       │   ├── provider-ezyang$htmlpurifier.json
│       │   ├── provider-fxp$composer-asset-plugin.json
│       │   ├── provider-fzaninotto$faker.json
│       │   ├── provider-phpspec$php-diff.json
│       │   ├── provider-swiftmailer$swiftmailer.json
│       │   ├── provider-yiisoft$yii2-app-advanced.json
│       │   ├── provider-yiisoft$yii2-bootstrap.json
│       │   ├── provider-yiisoft$yii2-codeception.json
│       │   ├── provider-yiisoft$yii2-composer.json
│       │   ├── provider-yiisoft$yii2-debug.json
│       │   ├── provider-yiisoft$yii2-faker.json
│       │   ├── provider-yiisoft$yii2-gii.json
│       │   ├── provider-yiisoft$yii2-swiftmailer.json
│       │   └── provider-yiisoft$yii2.json
│       └── https---registry.npmjs.org
├── composer.json
├── composer.lock
├── config.json
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
