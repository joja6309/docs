all: SoapClientFormatterSinkProvider_CreateSink_Client.dll SoapClientFormatterSinkProvider_CreateSink_Server.dll SoapClientFormatterSinkProvider_CreateSink_Shared.dll soapclientformattersinkprovider_customprovider.dll

SoapClientFormatterSinkProvider_CreateSink_Client.dll: SoapClientFormatterSinkProvider_CreateSink_Client.cs SoapClientFormatterSinkProvider_CreateSink_Shared.dll soapclientformattersinkprovider_customprovider.dll
	csc /t:library SoapClientFormatterSinkProvider_CreateSink_Client.cs /r:SoapClientFormatterSinkProvider_CreateSink_Shared.dll /r:soapclientformattersinkprovider_customprovider.dll
SoapClientFormatterSinkProvider_CreateSink_Server.dll: SoapClientFormatterSinkProvider_CreateSink_Server.cs SoapClientFormatterSinkProvider_CreateSink_Shared.dll
	csc /t:library SoapClientFormatterSinkProvider_CreateSink_Server.cs /r:SoapClientFormatterSinkProvider_CreateSink_Shared.dll 
SoapClientFormatterSinkProvider_CreateSink_Shared.dll: SoapClientFormatterSinkProvider_CreateSink_Shared.cs
        csc /t:library SoapClientFormatterSinkProvider_CreateSink_Shared.cs  
soapclientformattersinkprovider_customprovider.dll: soapclientformattersinkprovider_customprovider.cs SoapClientFormatterSinkProvider_CreateSink_Shared.dll
		csc /t:library soapclientformattersinkprovider_customprovider.cs /r:SoapClientFormatterSinkProvider_CreateSink_Shared.dll 

