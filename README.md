# NRS Gateway
360NRS Gateway services integration.
This library allows you to use the SMS Push service from 360NRS Gateway.

## Quick Start
Just put in your username and password for the NRSGateway control panel, specify the recipients in array format and send it.
```php
use efidatansantana\nrsgateway\SMSService;

$nrs = new SMSService('username', 'password');
$nrs->to   = ['xxxxxxxxxxxxx', 'yyyyyyyyyyyyy'];
$nrs->from = 'Sender';
$nrs->msg  = 'This is a test message.';
$nrs->send();
```

