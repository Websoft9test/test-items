# Initial Installation

If you have completed the Test deployment on Cloud Platform, the following steps is for you to start use it quikly

## Preparation

1. Get the **Internet IP** on your Cloud Platform
2. Check you **[Inbound of Security Group Rule](https://support.websoft9.com/docs/faq/tech-instance.html)** of Cloud Console to ensure the TCP:8161 is allowed
3. Make a domain resolution on your DNS Console if you want to use domain for Test

## Test Installation Wizard

1. Using local Chrome or Firefox to visit the URL *http://DNS:15672* or *http://Internet IP:15672*, you will enter installation wizard of Test
   ![](https://libs.websoft9.com/Websoft9/DocsPicture/zh/test/test-login-websoft9.png)

2. Log in to Test web console([Don't have password?](/stack-accounts.md#test))  
   ![](https://libs.websoft9.com/Websoft9/DocsPicture/zh/test/test-bk-websoft9.png)

3. Set you new password from: 【Users】>【Admin】>【Permissions】>【Update this user】
   ![](https://libs.websoft9.com/Websoft9/DocsPicture/zh/test/test-pw-websoft9.png)

> More useful Test guide, please refer to [Test Documentation](https://www.test.com/documentation.html)

## Q&A

#### I can't visit the start page of Test?

Your TCP:15672 of Security Group Rules is not allowed so there no response from Chrome or Firefox

#### Test service can't start? 