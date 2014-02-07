RznViewFilesPath
================

A ZF2 module allows you to change paths to view files (css, js, images) easily.

## Basic Using

There is the part of layout from skeleton application:

```	
        <?php echo $this->headLink(array('rel' => 'shortcut icon', 'type' => 'image/vnd.microsoft.icon', 'href' => $this->viewFilesPath('/img/favicon.ico')))
                        ->prependStylesheet($this->viewFilesPath('/css/bootstrap.min.css')) ?>


        <?php echo $this->headScript()
            ->prependFile($this->viewFilesPath() . '/js/bootstrap.min.js')
            ->prependFile($this->viewFilePath() . '/js/jquery.min.js')
        ; ?>
```

## Installation via Composer

### Steps 

#### 1. Add to composer.
```
    "require" : {
        "andydune/rzn-view-files-path": "dev-master"
    }
```

#### 2. Copy config file (`rzn-view-files-path.global.php`) to your application autoload dir if you need to change basic configuration.

#### 3. Add module to application config (/config/application.config.php)
```
   ...
   'modules' => array(
        'RznViewFilesPath',
   ),
   ...
```
