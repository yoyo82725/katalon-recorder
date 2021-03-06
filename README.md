# BDDWebRecorder
透過Chrome擴充功能安裝 (chrome://extensions/)
載入未封裝項目

API劫持需將 apitrack/BDDWebRecorder-sw.js 檔案放置專案根目錄

基於Katalon Recorder修改
感謝Katalon團隊與所有參與人的貢獻

測試報告展示：
[瀏覽商品.html](http://htmlpreview.github.io/?https://github.com/yoyo82725/BDDWebRecorder/blob/master/demoPic/%E7%80%8F%E8%A6%BD%E5%95%86%E5%93%81.html "瀏覽商品.html")
[優惠券.html](http://htmlpreview.github.io/?https://github.com/yoyo82725/BDDWebRecorder/blob/master/demoPic/%E5%84%AA%E6%83%A0%E5%88%B8.html "優惠券.html")

內容截圖：
![Alt text](/demoPic/pic1.png "page6")
![Alt text](/demoPic/pic2.png "page6")
![Alt text](/demoPic/pic3.png "page6")
![Alt text](/demoPic/pic4.png "page6")
![Alt text](/demoPic/pic5.png "page6")
![Alt text](/demoPic/pic6.png "page6")
![Alt text](/demoPic/pic7.png "page6")
![Alt text](/demoPic/pic8.png "page6")
![Alt text](/demoPic/pic9.png "page6")

# Katalon Recorder

## How to add new formatter

Add to `panel\index.html` (replace `sample` with the formatter name):

```
<option value="new-formatter-sample">Sample for new formatters</option>
```

Sample implementation:
```
panel\js\katalon\newformatters\sample.js
```

References:
* Implement New Relic Synthetics formatter #16
* Add protractor typescript template #23

## Resources

https://github.com/katalon-studio/katalon-recorder-helper

https://github.com/katalon-studio/katalon-recorder-samples

https://github.com/katalon-studio/katalon-recorder-sample-plugin

## For Mozilla Reviewers

The file `atoms.js` was built from https://github.com/SeleniumHQ/selenium/tree/selenium-3.141.59.

Build steps:
```
./go build
./go //javascript/selenium-atoms
# output: build/javascript/selenium-atoms/selenium-atoms.js
```

The use of CSP and eval is necessary for a record & playback tool (including inject JavaScript PER user commands). There is no other way to do this so please don't disable our add on again.

## Acknowledgments

We would like to take this opportunity to express our warmest thanks to Katalon Recorder users and other open-source projects, especially:

* Selenium IDE Project - [http://www.seleniumhq.org](http://www.seleniumhq.org/).

* SideeX - https://github.com/SideeX/sideex.

* Robot Framework Formatter Project - https://github.com/ngocbv/Robot-Framework-Formatter.

* Formatter for C# with MSTest is provided by [Mark Gibson](https://forum.katalon.com/discussion/4209/export-to-c-with-webdriver-and-mstest).

* @[Patrick Groot](https://github.com/pgroot91), @Piotr, @Mark_Gibson and other active members who have provided a lot of valuable suggestions and bug reports. Please forgive us if your name is missing here.

* Plugin developers:

  * Jan Esser - PHPUnit formatter for Katalon Recorder ([Chrome](https://chrome.google.com/webstore/detail/phpunit-formatter-for-kat/gelokgfkbnkkcdbokielchgpfnphoalk?utm_source=chrome-ntp-icon))

  * Sam Kirkland - Puppeteer exporter for Katalon Recorder (https://github.com/SamKirkland/Puppeteer-exporter-for-Katalon-Recorder)

## License

Refer to NOTICE and KATALON RECORDER CONTRIBUTION LICENSE AGREEMENT for Katalon Recorder.

Refer to APACHE LICENSE 2.0 for SideeX.

Please inform us if you found any unlicensed part of source code.
