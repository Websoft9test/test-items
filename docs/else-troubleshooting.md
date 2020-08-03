# Troubleshooting

We collect the most common troubleshooting of using Test for your reference:

> Instance troubleshooting is closely related to the Instance provider that is Cloud Platform, refer to [Cloud Platform Documentation](https://support.websoft9.com/docs/faq/tech-instance.html)

#### How can I use the logs?

You can find the keywords **Failed** or **error** from the logs directory: `/data/logs`

#### Test service can't start?

Insufficient disk space and memory, incorrect configuration file may cause the failure to start the service. 

It is recommended to first check through the command.

```shell
# restart Test service
systemctl status test
journalctl -u test

# view disk space
df -lh

# view memory rate
free -lh
```

#### Error in Chrome when modify password?

This error is not attribute to Test server, once you have upgraded you local Chrome, it solved

![chrome error of Test](https://libs.websoft9.com/Websoft9/DocsPicture/zh/test/test-chromeerror-websoft9.png)
