# Python Service Broker Sample - Getting Started
 The repository contains code for a very simple broker, our sample broker. Once deployed as a Bluemix app, it can be used to create/delete a broker, provision a sample Fido service through that broker, bind and unbind it to/from an application, and to delete the service again. Neither our code nor the instructions below will touch topics such as managing service plans or how to enable certain service plans to organizations.


[![Deploy to Bluemix](https://bluemix.net/deploy/button.png)](https://bluemix.net/deploy?repository=https://github.com/Mike-msoh/Python-Service-Broker-Sample.git)

# Procedure
0. Change the hostname of manifest.yml
1. Change Service.name in python-service-broker.py to your unique name. (default : py-auth-service)
2. Deploy your app (ex. cf push)
3. Register Service Broker (ex. cf create-service-broker Your-Broker-Name py-user py-pwd https://YourHost.mybluemix.net --space-scoped)
4. List if the broker registered properly. (ex. cf service-brokers)
5. Provision a service (ex. cf create-service py-auth-service fidoplan-a Fido-Service)
6. Execute Bind, Unbind and Unprovision on Bluemix dashboard

# Contribute / Contact Information
If you have found errors or some instructions are not working anymore, then please open an GitHub issue or, better, create a pull request with your desired changes.


