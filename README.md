### WebDriverAgent
---
https://github.com/facebook/WebDriverAgent/wiki/Starting-WebDriverAgent

```
./Scripts/bootstrap.sh
```

```
By.xpath('//XCUIElementTypeTable') ->
By.className('XCUIElementTypeTable')

By.xpath('//XCUIElementTypeTable[@name="table"]') ->
By.accessibilityId('table')

By.xpath() ->
By.predicate()

dstElement = driver.findElement(
  By.xpath('//XCUIElementTypeTable[@name="table"]//XCUIElementTypeTextField[@visible="true"]')) ->
tableEl = driver.findElement(By.accessibilityId('table'));
dstElement =tableEl.findElement(
  By.predicate('type == "XCUIElementTypeTextField" AND visible == 1'))
```

```
```
