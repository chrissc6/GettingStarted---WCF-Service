# GettingStarted---WCF-Service

Tutorial: Get started with Windows Communication Foundation applications
https://docs.microsoft.com/en-us/dotnet/framework/wcf/getting-started-tutorial

service's page:
http://localhost:8000/GettingStarted/CalculatorService

Services such as this one require the proper permission to register HTTP addresses on the machine for listening. 
Administrator accounts have this permission, but non-administrator accounts must be granted permission for 
HTTP namespaces. 

using the ServiceModel Metadata Utility tool (Svcutil.exe) to generate the proxy class file
(svcutil.exe /language:cs /out:generatedProxy.cs /config:app.config http://localhost:8000/GettingStarted/CalculatorService)
run in the Developer Command Prompt for VS 

To start the service: 
-Open a command prompt as an administrator, and then navigate to your Visual Studio solution directory.
-Enter GettingStartedHost\bin\Debug\GettingStartedHost.exe.

To start the client: 
-Open another command prompt, navigate to your Visual Studio solution directory.
=Enter GettingStartedClient\bin\Debug\GettingStartedClient.exe.
