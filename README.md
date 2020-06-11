### HTML5 Azure Form Recognizer Layout API Results Formatter

View an interactive demo [here](https://davideker.github.io/layout/).

![alt text](https://raw.githubusercontent.com/davideker/layout/d341b262ce50e0ba6a2955cc448c345908dd3f1f/example.png)

> **HTML5** utility that makes the **JSON** results of the [**Azure Form Recognizer Layout API**]("https://docs.microsoft.com/en-us/azure/cognitive-services/form-recognizer/quickstarts/python-layout") more comprehensible. Features include toggling read and page layout layers and tooltips that show the predictions and confidence level of each highlighted element. New features include inline editing documents, document preview and saving edits. 

To format the results of an API call, manually or programatically, replace the original and blank image source with a link to your document and a blank document respectively...

```html
<img id="original" class="img" src="contoso-invoice.png" onload="initialize(this)" />
<img id="blank" class="img hidden" src="contoso-invoice-b
```

 ... and update the path to the **JSON** results returned by the API. 
 ```javascript
 const json = "Invoice_1.pdf.ocr.json";
```

>This utility supports and has been tested with **PNG** files. However, a list of file types supported by the &lt;img/&gt; element can be found [**here**](https://developer.mozilla.org/en-US/docs/Web/Media/Formats/Image_types) and should work as well. The subset of document image formats supported by the **Azure Form Recognizer Layout API** can be found [**here**](https://docs.microsoft.com/en-us/azure/cognitive-services/form-recognizer/overview). 
---


You **MUST** use links to resources served from an **HTTP** compatible web server, local file system references <ins>**will not**</ins> work. To run a simple HTTP server locally use:
```javascript
npx http-server
```