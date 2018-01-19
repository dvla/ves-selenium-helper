# VES Selenium Helper
---

A handy extension to Selenium web tests which helps generate and organise screenshots of your automated web tests. Build to aid the documentation of the [Vehicle Enquiry Service](https://vehicleenquiry.service.gov.uk/). Uses the test method name and namespace to automatically create a folder structure to organise your screenshots - great for quickly and automatically documenting your service.

## Prerequisites

Requires FireFox browser to be installed. We use [Firefox v47](https://ftp.mozilla.org/pub/firefox/releases/47.0/) as this allows Selenium to take full page screenshots like [this](https://raw.githubusercontent.com/dvla/ves-screenshot-helper/master/SampleScreenshots/GovUkHomePageTest.png).


## How to use
* Add a reference to the `ScreenshotHelper` project to your test project
* Ensure your test class inherits the `ScreenshotManager` class
* Run your test 
* Call the `TakeScreenshot();` method

Screenshots will be then be saved in the root directory as specified in the `app.config` file, using the test namespace and method name to create a folder structure.

Checkout the **SampleTests** project for examples and more info