### HTML5 Azure Form Recognizer Layout API Results Formatter

![alt text](https://raw.githubusercontent.com/davideker/layout/d341b262ce50e0ba6a2955cc448c345908dd3f1f/example.png)

> **HTML5** utility that makes the **JSON** results of the [**Azure Form Recognizer Layout API**]("https://docs.microsoft.com/en-us/azure/cognitive-services/form-recognizer/quickstarts/python-layout") more comprehensible. The new version supports toggling read and page layout layers and tooltips that show the predictions and confidence level of each highlighted element.

To format the results of an API call, manually or programatically, replace the image source with a link to your document ...

```html
<img class='img' src="https://docs.microsoft.com/en-us/azure/cognitive-services/form-recognizer/media/contoso-invoice.png" onload="Initialize(this)"/>
```

 ... and update the path to the **JSON** results returned by the API. 
 ```javascript
 const json = "https://raw.githubusercontent.com/Azure-Samples/cognitive-services-REST-api-samples/master/curl/form-recognizer/Invoice_1.pdf.ocr.json";
```

>This utility only supports **JPG**, **PNG** or **TIFF** formats. For the best results use a **JPEG** or **PNG** of your document to perform the layout analysis. A list of file types supported by the &lt;img/&gt; element can be found [**here**](https://developer.mozilla.org/en-US/docs/Web/Media/Formats/Image_types). The subset of document image formats supported by the **Azure Form Recognizer Layout API** can be found [**here**](https://docs.microsoft.com/en-us/azure/cognitive-services/form-recognizer/overview). 
---


You **MUST** use links to resources served from an **HTTP** compatible web server, local file system references <ins>**will not**</ins> work. To run a simple HTTP server locally use:
```javascript
npx http-server
```


