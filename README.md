# Layout API Formatter

A small HTML5 utility for making the JSON results of the [Azure Form Recognizer Layout API]("https://docs.microsoft.com/en-us/azure/cognitive-services/form-recognizer/quickstarts/python-layout") more comprehensible .
---

Replace the image source

```html
<img class='img' src="https://docs.microsoft.com/en-us/azure/cognitive-services/form-recognizer/media/contoso-invoice.png" onload="Initialize(this)"/>
```

 And update the link to the layout.ocr.json file
 ```javascript
 addLayout("https://raw.githubusercontent.com/Azure-Samples/cognitive-services-REST-api-samples/master/curl/form-recognizer/Invoice_1.pdf.ocr.json");
```

![alt text](https://raw.githubusercontent.com/davideker/layout/master/example.png)

