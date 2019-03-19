# AspectizeRTC Documentation
Aspectize Real Time Communication Extension Documentation

# 1 - Download

Download extension package from aspectize.com:
- in the portal, goto extension section
- browse extension, and find AspectizeRTC
- download package and unzip it into your local WebHost Applications directory; you should have a AspectizeRTC directory next to your app directory.

# 2 - Configuration

Add AspectizeRTC as Shared Application in your application configuration file.
In your Visual Studio Project, find the file Application.js in the Configuration folder.

Add AspectizeRTC in the Directories list :
```javascript
app.Directories = "AspectizeRTC";
```

Add a new configured service in your Application

In your Visual Studio Project, find the file Services.js in the Configuration folder.

```javascript
var myRTCService = Aspectize.ConfigureNewService("MyRTCService", aas.ConfigurableServices.AspectizeRTCMessaging);
myRTCService.AccountId = "MyDataService";
myRTCService.AccountSecret = "MyFileService";
```

The Configurable Service has the following parameters:
AccountId: this is your unique ID of your account in aspectize portal.
AccountSecret:
