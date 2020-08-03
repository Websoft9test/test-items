# Deployment

**Deployment is to copy the Test pre-packaged online to your Cloud Server**. For example, after the user subscribe Test on the Cloud Platform, the Platform will automatically copy the Test to the corresponding Cloud Server.

- If Test has been deployed, go to [Initial Installation](/zh/stack-installation.md) to complete the operation.
- If Test is not deployed, you need to deploy Test to your cloud server first.

We offer two deployment Test scenarios (the deployment results are the same):

## Deploy by Image

**Deploy by Image** means starting instance from Test images. **Test Image** provide OS and software environment needed for Test.

For users with experience with cloud servers, Deploy by Image equated with "one-click deployment".

Websoft9 published [Test image](https://apps.websoft9.com/test) on Cloud Platform, three methods for your deployment:

* When **Create New Instance** , select the Test image as the system boot template.
* When **Subscribe Test** on Marketplace, the system will promote you to create a new instance for this image at the same time.
* When **Re-install OS** for you instance, you can replace the existing image with a Test image.

## Deploy by Script

**Deploy by Script** means running a script on your cloud instance to pull the pre-packages online to your instance and configure it at the same time.

Websoft9 provide the [Test ansbile automation script](https://github.com/Websoft9/ansible-test) on Github. If you are familiar with Ansible, you can deploy the Test to the instance automaticly.

## Comparison

Although the results of the **deploy by image** are consistent with the results of **deploy by script**, what is the difference between the two deployment methods?

Suggest you read the document [Deploy by Image vs Deploy by Script](https://support.websoft9.com/docs/faq/bz-product.html#deployment-comparison)