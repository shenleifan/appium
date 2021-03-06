# Get Element Text

Returns visible text for element
## Example Usage

```java
// Java
MobileElement element = (MobileElement) driver.findElementByClassName("SomeClassName");
let elText = element.getText();

```

```python
# Python
el = self.driver.find_element_by_accessibility_id('SomeAccessibilityID')
text = el.text

```

```javascript
// Javascript
// webdriver.io example
driver.getText("~SomeAccessibilityId");



// wd example
let element = await driver.elementByAccessibilityId("SomeAccessibilityID");
await element.submit();

```

```ruby
# Ruby
element = @driver.find_element :accessibility_id, "SomeAccessibilityID"
element.text

```

```php
# PHP
$el = $this->byAccessibilityId('SomeAccessibilityID');
$text = $el->text();

```

```csharp
// C#
// TODO C# sample

```


## Description

Returns the visible text for the element.


## Support

### Appium Server

|Platform|Driver|Platform Versions|Appium Version|Driver Version|
|--------|----------------|------|--------------|--------------|
| iOS | [XCUITest](/docs/en/drivers/ios-xcuitest.md) | 9.3+ | 1.6.0+ | All |
|  | [UIAutomation](/docs/en/drivers/ios-uiautomation.md) | 8.0 to 9.3 | All | All |
| Android | [UiAutomator2](/docs/en/drivers/android-uiautomator2.md) | ?+ | 1.6.0+ | All |
|  | [UiAutomator](/docs/en/drivers/android-uiautomator.md) | 4.2+ | All | All |
| Mac | [Mac](/docs/en/drivers/mac.md) | ?+ | 1.6.4+ | All |
| Windows | [Windows](/docs/en/drivers/windows.md) | 10+ | 1.6.0+ | All |

### Appium Clients

|Language|Support|Documentation|
|--------|-------|-------------|
|[Java](https://github.com/appium/java-client/releases/latest)| All |  [seleniumhq.github.io](https://seleniumhq.github.io/selenium/docs/api/java/org/openqa/selenium/WebElement.html#getText--)  |
|[Python](https://github.com/appium/python-client/releases/latest)| All |  [selenium-python.readthedocs.io](http://selenium-python.readthedocs.io/api.html)  |
|[Javascript (WebdriverIO)](http://webdriver.io/index.html)| All |  [webdriver.io](http://webdriver.io/api/property/getText.html)  |
|[Javascript (WD)](https://github.com/admc/wd/releases/latest)| All |  [github.com](https://github.com/admc/wd/blob/master/lib/commands.js#L1832)  |
|[Ruby](https://github.com/appium/ruby_lib/releases/latest)| All |  [www.rubydoc.info](http://www.rubydoc.info/gems/selenium-webdriver/Selenium/WebDriver/Element#text-instance_method)  |
|[PHP](https://github.com/appium/php-client/releases/latest)| All |  [github.com](https://github.com/appium/php-client/)  |
|[C#](https://github.com/appium/appium-dotnet-driver/releases/latest)| All |  [github.com](https://github.com/appium/appium-dotnet-driver/)  |

## HTTP API Specifications

### Endpoint

`GET /wd/hub/session/:session_id/element/:element_id/text`

### URL Parameters

|name|description|
|----|-----------|
|session_id|ID of the session to route the command to|
|element_id|ID of the element to get the text from|

### JSON Parameters

None

### Response

null

## See Also

* [W3C Specification](https://www.w3.org/TR/webdriver/#dfn-get-element-text)
* [JSONWP Specification](https://github.com/SeleniumHQ/selenium/wiki/JsonWireProtocol#sessionsessionidelementidtext)
