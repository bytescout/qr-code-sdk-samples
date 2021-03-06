## How to command line use in VBScript and VB6 and ByteScout QR Code

### The tutorial below will demonstrate how to command line use in VBScript and VB6

We made thousands of pre-made source code pieces for easy implementation in your own programming projects. ByteScout QR Code can command line use. It can be used from VBScript and VB6. ByteScout QR Code is QR Code generation library. It provides full control on the quality, features and encoding. Can embed logo image right into QR Code itself. Batch barcode generation, and many special features like vCard or URL encoding are also supported.

The SDK samples like this one below explain how to quickly make your application do command line use in VBScript and VB6 with the help of ByteScout QR Code. In your VBScript and VB6 project or application you may simply copy & paste the code and then run your app! Enjoy writing a code with ready-to-use sample codes in VBScript and VB6.

ByteScout free trial version is available for download from our website. It includes all these programming tutorials along with source code samples.

## REQUEST FREE TECH SUPPORT

[Click here to get in touch](https://bytescout.zendesk.com/hc/en-us/requests/new?subject=ByteScout%20QR%20Code%20Question)

or just send email to [support@bytescout.com](mailto:support@bytescout.com?subject=ByteScout%20QR%20Code%20Question) 

## ON-PREMISE OFFLINE SDK 

[Get Your 60 Day Free Trial](https://bytescout.com/download/web-installer?utm_source=github-readme)
[Explore SDK Docs](https://bytescout.com/documentation/index.html?utm_source=github-readme)
[Sign Up For Online Training](https://academy.bytescout.com/)


## ON-DEMAND REST WEB API

[Get your API key](https://pdf.co/documentation/api?utm_source=github-readme)
[Explore Web API Documentation](https://pdf.co/documentation/api?utm_source=github-readme)
[Explore Web API Samples](https://github.com/bytescout/ByteScout-SDK-SourceCode/tree/master/PDF.co%20Web%20API)

## VIDEO REVIEW

[https://www.youtube.com/watch?v=A5hB9ul3tX0](https://www.youtube.com/watch?v=A5hB9ul3tX0)




<!-- code block begin -->

##### ****GenerateQRCode.vbs:**
    
```
if WScript.Arguments.Count < 1 Then
    WScript.Echo "Set barcode value as command line parameter: " & vbCRLF & vbCRLF & "GenerateQRCode.vbs <value>"
    WScript.Quit 0
End If

' Create and activate QRCode instance
Set barcode = CreateObject("Bytescout.BarCode.QRCode")
barcode.RegistrationName = "demo"
barcode.RegistrationKey = "demo"

' Set barcode value from the command line parameter
barcode.Value = WScript.Arguments(0)

' Save barcode image to file
barcode.SaveImage("result.png")

Set barcode = Nothing

```

<!-- code block end -->    

<!-- code block begin -->

##### ****run.bat:**
    
```
REM running from the command line
cscript.exe GenerateQRCode.vbs "ABCDEFGHIJKLMNOP1234567890"
pause
```

<!-- code block end -->