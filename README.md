## Automated web tests using Serenity, Cucumber and Maven

A simple example of some BDD-style automated acceptance criteria, running against http://etsy.com. 

Run the tests like this:

```
mvn clean verify
```

By default, the tests run with chrome, to run run on firefox change the value of the driver property in the serenity.properties file.
By default paths to Mac drivers are enabled. If you are using Windows, comment out the mac drivers and enable the windows drivers in the serenity.properties file.

Drivers are in the test/resources/drivers folde. You will have to manually update them if your browser version does not match.
```
mvn clean verify -Dwebdriver.driver=firefox
```

The reports will be generated in `target/site/serenity`.
