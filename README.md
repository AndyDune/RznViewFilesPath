RznViewFilesPath
================

A ZF2 module allows you to change the paths to view files (css, js, images) easily.

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
