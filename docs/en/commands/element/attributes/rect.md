# Get Element Rect

Gets dimensions and coordinates of an element
## Example Usage

```java
// Java
List<MobileElement> element = (MobileElement) driver.findElementByAccessibilityId("SomeAccessibilityID");
Rectangle rect = element.getRect();

```

```python
# Not supported
```

```javascript
// Javascript
// webdriver.io example
let rect = driver.elementIdRect("~SomeAccessibilityId");



// wd example
let element = await driver.elementByAccessibilityId("SomeAccessibilityID");
let rect = await element.getRect();

```

```ruby
# Ruby
element = @driver.find_element :accessibility_id, "SomeAccessibilityID"
element.rect

```

```php
# PHP
// TODO PHP sample

```

```csharp
// C#
// TODO C# sample

```



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
|[Java](https://github.com/appium/java-client/releases/latest)| All |  [seleniumhq.github.io](https://seleniumhq.github.io/selenium/docs/api/java/org/openqa/selenium/WebElement.html#getRect--)  |
|[Python](https://github.com/appium/python-client/releases/latest)| All |  |
|[Javascript (WebdriverIO)](http://webdriver.io/index.html)| All |  [webdriver.io](http://webdriver.io/api/protocol/elementIdRect.html)  |
|[Javascript (WD)](https://github.com/admc/wd/releases/latest)| All |  |
|[Ruby](https://github.com/appium/ruby_lib/releases/latest)| All |  [www.rubydoc.info](http://www.rubydoc.info/gems/selenium-webdriver/Selenium/WebDriver/Element#rect-instance_method)  |
|[PHP](https://github.com/appium/php-client/releases/latest)| All |  [github.com](https://github.com/appium/php-client/)  |
|[C#](https://github.com/appium/appium-dotnet-driver/releases/latest)| All |  [github.com](https://github.com/appium/appium-dotnet-driver/)  |

## HTTP API Specifications

### Endpoint

`GET /wd/hub/session/:session_id/elements/:element_id/rect`

### URL Parameters

|name|description|
|----|-----------|
|session_id|ID of the session to route the command to|
|element_id|ID of the element to get the rect of|

### JSON Parameters

None

### Response

|name|type|description|
|----|----|-----------|
| x | `number` | X coordinate |
| y | `number` | Y coordinate |
| height | `number` | Height of the bounding rectangle |
| weight | `number` | Width of the bounding rectangle |

## See Also

* [W3C Specification](https://www.w3.org/TR/webdriver/#dfn-get-element-rect)
