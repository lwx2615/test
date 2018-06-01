# yii2-mywalker
本例子只做示例用，用于创建一个yii2的扩展。结合composer管理！
将websocket的相关代码作为第三方扩展，用composer进行管理，
页面部分及数据处理部分作为yii的APP，放在componets中。以后在扩展中丰富
各种功能，只接受yii处理好的数据格式。

>yiiapplication/  **项目根目录**  
    assets/ <br/>
    runtime/  <br/>
    views/ <br/>
    config/ <br/>
    models/ <br/>
        User.php   <br/>    
    modules/   <br/>
        chat/  <br/>
    web/
    controlloers/
    packages.json
    widgets/
    composer.json
    vender/
        autoload.php
        phpdocumentor/
        swiftmailer/
        workerman/
            gateway-worker/
            workerman/
        yiisoft/
            yii2/
            yii2-jui/
            yii2-swiftmailer/
        testyiislft/
            yii2-mywalker/
                Applications/
                composer.json
                start.php
                LICENSE
                README.md
                
        
