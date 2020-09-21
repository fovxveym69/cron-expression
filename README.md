# cron-expression
Calculate the next run date a CRON expression. Support years and seconds (计算crontab表达式下一个执行日期，支持年和秒)

Installing
==========

Add the dependency to your project:

```bash
composer require han-xuefeng/cron-expression
```

Usage
=====
```php
<?php

require_once '/vendor/autoload.php';


$cron = Cron\Cronexpr::parse('* * * * *');

echo $cron->next()->format('Y-m-d H:i:s');

```

Requirements
============
- PHP 7.1+
