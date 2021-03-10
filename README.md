# .NET Core HTML to Image Converter

## Convert HTML string to image bytes
```
var converter = new HtmlConverter();
var html = "<div><strong>Hello</strong> World!</div>";
var bytes = converter.FromHtmlString(html);
File.WriteAllBytes("image.jpg", bytes);
```
            
## Convert URL to image bytes
```
var converter = new HtmlConverter();
var bytes = converter.FromUrl("http://google.com");
File.WriteAllBytes("image.jpg", bytes);
```

## Optional parameters
1. width - output document width. Default is 1024. -1 is smart width.
2. format - output image format. Default is Jpg.
3. quality - output image quality from 1 to 100. Default is 100.

## Roadmap
* Async methods
* Non-Windows support

## More about this library
This is a fork of Andrei M's net-core-html-to-image (https://github.com/andrei-m-code/net-core-html-to-image), I've added support for smart width.

## MIT License

Copyright (c) 2020 Gaurav Gohel

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
