# Logging

---

Logging is a method that you need to develop in software development. You should be logging everything that happens in
your application so that you can debug issues in production. You should be logging things like errors, warnings, and
informational messages. You should also be logging things like request and response times, and resource usage. You can
use tools like ELK, Splunk, Sumo Logic, etc to log your application.

When something goes wrong in production and you can not replicate it the logs are going to be the only way you'll be
able to figure out what is happening in production.

If you are using a cloud provider like AWS, Azure, GCP, etc you can use their logging services to log your application.

If you're using Laravel you can easily use the Log facade to output the logs to a file, you can also use Monolog to
output the logs to a file or a service like AWS CloudWatch.

Here is an example of how you can use the Log facade in Laravel:

```php
Log::debug('This is a debug message');
Log::info('This is an informational message');
Log::warning('This is a warning message');
Log::error('This is an error message');
```
