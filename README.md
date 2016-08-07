# Progressive Enhancement resources

A comprehensive collection of resources on Progressive Enhancement. From concept and strategies to feature detection and testing methods. Complete with a list of (code) examples.


## Table of Contents

* [The concept](#the-concept)
* [Strategies](#strategies)
* [Feature detection](#feature-detection)
* [Support tables](#support-tables)
* [Testing methods](#testing-methods)
* [Examples](#examples)
* [Related articles](#related-articles)


## The concept

Progressive enhancement means gradually improving the user experience after verifying the target environment (e.g. browser) is capable of it. Start with content and ensure you maintain functionality & accessibility.

* [Progressive Enhancement: It's about the content](http://cognition.happycog.com/article/progressive-enhancement-its-about-the-content): sharing content is the core of the web. Progressive Enhancement ensures access to content.
* [The Role of Enhancement in Web Design](https://www.nngroup.com/articles/enhancement/): from the concept of enhancement to the criteria and rules for enriching the user interface.
* [Understanding Progressive Enhancement](http://alistapart.com/article/understandingprogressiveenhancement): apply technologies in an intelligent way, layer-upon-layer, to craft an amazing experience.
* [Designing with Progressive Enhancment](https://www.filamentgroup.com/dwpe/) *The book* (400+ pages) on Progressive Enhancement.
* [Adaptive Web Design](http://adaptivewebdesign.info/2nd-edition/) book on Progressive Enhancement from content to design and interaction.
* [Detecting (HTML5) features](http://diveinto.html5doctor.com/detect.html): intro to different feature detection techniques with examples and demos. 
* [Progressive Web Apps](https://infrequently.org/2015/06/progressive-apps-escaping-tabs-without-losing-our-soul/): enhancing web sites into native-like apps (progressive, not hybrid).


## Strategies

You can apply Progressive Enhancement in different ways:

* [The Content-out Approach](https://articles.uie.com/progressive_enhancement/): provide wide access to content without technological restrictions.
* [Make the page usable with only HTML](https://www.gov.uk/service-manual/technology/using-progressive-enhancement#make-the-page-usable-with-only-html): this sets the baseline for every device and browser.
* [Test Driven Progressive Enhancement](http://alistapart.com/article/testdriven): core functional experience enhanced after testing capabilities.
* [Cut the mustard](http://responsivenews.co.uk/post/18948466399/cutting-the-mustard): set a threshold for collection of enhancements.
* [Grade components, not browsers](https://www.filamentgroup.com/lab/grade-the-components.html
): component level feature tests and enhancements.
* [Feature vs Browser vs Form factor detection](http://www.html5rocks.com/en/tutorials/detection/) as different strategies to tune your app to its environment.
* [Server-side device detection](https://www.smashingmagazine.com/2014/07/server-side-device-detection-with-javascript/): use user-agent and other HTTP header info combined with a device database to conditionally serve files.
* [Writing polyfills](https://addyosmani.com/blog/writing-polyfills/) - if your baseline is still too high for some browsers, consider [polyfills](https://remysharp.com/2010/10/08/what-is-a-polyfill) (aka [Regressive Enhancement](https://twitter.com/SlexAxton/status/25600963629)).
* [Application Shell Architecture](https://medium.com/google-developers/instant-loading-web-apps-with-an-application-shell-architecture-7c0c2f10c73): a setup for instant loading web apps.


## Feature detection

Before you try to enhance the experience, you need to ensure the environment is capable of the enhancement. You test this by performing feature detections:

* [CSS feature queries](https://www.sitepoint.com/an-introduction-to-css-supports-rule-feature-queries/) ([`CSS.supports()`](https://developer.mozilla.org/en/docs/Web/API/CSS/supports) & [`@supports()`](https://developer.mozilla.org/en-US/docs/Web/CSS/@supports)) natively test if specific CSS feature is supported using JS method or CSS declaration.
* [Feature Detect ES6](https://www.npmjs.com/package/feature-detect-es6) detect which ES2015 features are available.
* [SVG requiredFeatures](https://developer.mozilla.org/en-US/docs/Web/SVG/Attribute/requiredFeatures) render SVG elements only if their `[requiredFeatures]` evaluate to true.
* [Modernizr](https://modernizr.com/) is an extensive feature detection suite (supports custom builds).
* [Feature.js](http://featurejs.com/) is a lightweight feature detection suite.
* ~~[has.js](https://github.com/phiggins42/has.js)~~ (note: not actively maintained)
* [Conditioner.js](http://conditionerjs.com/) conditionally load JS modules based on directives in HTML attributes.
* [EnhanceJS](https://www.filamentgroup.com/lab/introducing-enhancejs-smarter-safer-apply-progressive-enhancement.html) lets you asynchronously load CSS & JS after a set pre-defined feature tests.


## Support tables

Different environments (platforms, browsers, versions) have different capabilities. Support tables tell you what capabilities each environment has. Knowing the level of support can help you weigh an enhancement against the effort and impact of its implementation.

* [The Web Platform](https://platform.html5.org/) overview of browser technologies with links to docs and test suites.
* [Can I use ...?](http://caniuse.com/) compare feature implementations and limitations across desktop & mobile browsers.
* [I want to use ...](http://www.iwanttouse.com/) figure out the browser support of combinations of features.
* [HTML5 Test](http://html5test.com/) test and compare HTML5 feature support across browsers.
* [CSS3 Test](http://css3test.com/) fine-grained tests for CSS3 feature support of your current browser.
* [Font Family Reunion](http://fontfamily.io/) compatibility tables for default local (system) fonts.
* [What web can do today](https://whatwebcando.today/) lists and checks modern web APIs like access to device system, sensors and actuators.
* [HTML5 Worker test](https://nolanlawson.github.io/html5workertest/) compare which APIs are supported in Web Workers and Service Workers across browsers.
* [HTML5 Please](http://html5please.com/) explore features with recommendations and links to polyfills.
* [API Catalog](https://developer.microsoft.com/en-us/microsoft-edge/platform/catalog/) let's you compare implementation of API specifications in major desktop browsers.
* [Kangax's ECMAScript compatibility table](http://kangax.github.io/compat-table/) overview of JavaScript feature across browsers and other runtimes.
* [Is ServiceWorker ready?](https://jakearchibald.github.io/isserviceworkerready/) overview of support for all features involved in the core technology behind Progressive Web Apps.
* [Is WebRTC ready yet?](http://iswebrtcreadyyet.com/) overview of support for the different browser features behind real time communication. 
* [Chrome Platform Status](https://www.chromestatus.com/features)
* [Edge Platform Status](https://developer.microsoft.com/en-us/microsoft-edge/platform/status/)
* [Firefox Platform Status](https://platform-status.mozilla.org/)
* [Webkit Platform Status](https://webkit.org/status/) (Safari)
* [MDN Compatibility tables](https://developer.mozilla.org/en-US/docs/MDN/Contribute/Structures/Compatibility_tables) MDN's web technology documentation has a browser compatibility table end the end of each article. 


## Testing methods

With progressive enhancement you support different experiences in different environments. These are some ways to test all these variations:

* [Open Device Lab](https://opendevicelab.com/) let's you *test manually on actual devices* (for free).
* [Text browsers](https://en.wikipedia.org/wiki/Text-based_web_browser) like [Lynx](http://lynx.browser.org/) are a good way to test if your content is accessible at the baseline.
* [Testing in Opera Mini](https://dev.opera.com/articles/making-sites-work-opera-mini/#testing-in-opera-mini) download the app, emulate on desktop, setup to test local websites. (Opera Mini accounts for over 5% browser usage world wide)
* [cURL](https://curl.haxx.se/docs/manual.html) a web page to see the pre-rendered source code of a page.
* [Browserling](https://www.browserling.com/) let's you manually test web pages in different versions of browsers on Windows and Android platforms.
* [Run Internet Explorer using Virtual Machines](https://developer.microsoft.com/en-us/microsoft-edge/tools/vms/mac/) to test IE browsers on other platforms.
* [Configure *Desired Capabilities* in Selenium](https://github.com/SeleniumHQ/selenium/wiki/DesiredCapabilities) to run automated browser tests in different scenarios.
* Continuously run automated tests in different browsers using [BrowserStack](https://www.browserstack.com/), [Saucelabs](https://saucelabs.com/) or other alternatives.
* [Lighthouse](https://github.com/GoogleChrome/lighthouse): audit and meassure performance of Progressive Web Apps (via cli or [Chrome extension](https://chrome.google.com/webstore/detail/lighthouse/blipmdconlkpinefehnmjammfjpmpbjk)).
* [Progressive Enhancement checklist (1st edition, HTML)](http://adaptivewebdesign.info/1st-edition/read/chapter-6.html#the-progressive-enhancement-checklist), [Checklist of 2nd edition (PDF)](http://adaptivewebdesign.info/2nd-edition/checklist.pdf): actionable list to check you've applied Progressive Enhancement best practices. Part of [Adaptive Web Design book](http://adaptivewebdesign.info/).


## Examples

### Custom form elements

* [Fancy radio buttons](https://www.sitepoint.com/replacing-radio-buttons-without-replacing-radio-buttons/) based on HTML radio buttons, visually enhanced using CSS pseudo classes and elements.
* [Checkboxes & radio buttons](https://www.filamentgroup.com/dwpe/checkbox-radiobutton/) with custom focus, hover and checked state. Enhanced asynchronously.
* [Toggle switch](https://ghinda.net/css-toggle-switch/) Checkbox or radios, visually enhanced to sliding toggle switches using CSS only.
* [5-star rating](http://lea.verou.me/2011/08/accessible-star-rating-widget-with-pure-css/) bsed on HTML radio buttons, visually enhanced using CSS pseudo classes and elements.
* [jQuery slider](https://github.com/filamentgroup/jQuery-Slider) Accessible, custom slider widget based on a standard HTML select.
* [jQuery custom file input](https://www.filamentgroup.com/lab/jquery-custom-file-input-book-designing-with-progressive-enhancement.html) (article and library).

### Data visualisations

* [Timeline](https://css-tricks.com/progressive-enhancement-data-visualizations/) from definition list to SVG illustration (article with demos).
* [Charts](https://www.filamentgroup.com/lab/update-to-jquery-visualize-accessible-charts-with-html5-from-designing-with.html) from data table to themed charts using HTML5 canvas (article and library).

### Images

* [Responsive Carousel](http://filamentgroup.github.io/responsive-carousel/test/functional/fade-auto.html) list of images enhanced into responsive carousel with various behaviour options.
* [Lazy Progressive Enhancement](https://github.com/tvler/lazy-progressive-enhancement) lazy load images inside `<noscript>` tags. (note: Evergreen browsers only)


### Menus

* [Progressive hamburger menu](http://heydonworks.com/practical_aria_examples/#hamburger) list of links in footer enhanced to off-canvas menu.


## Related articles

* [Make the web work for everyone](https://hacks.mozilla.org/2016/07/make-the-web-work-for-everyone/) A plea to developers to consider browser differences and build a resilient web.
* [How many people are missing out on JavaScript enhancement?](https://gds.blog.gov.uk/2013/10/21/how-many-people-are-missing-out-on-javascript-enhancement/) Research on why in 1.1% of page visits JavaScript isn't loaded. 

---

## License

[![CC0](http://mirrors.creativecommons.org/presskit/buttons/88x31/svg/cc-zero.svg)](https://creativecommons.org/publicdomain/zero/1.0/)

[Jasper Moelker](https://twitter.com/jbmoelker) waives all rights to this work worldwide under copyright law, including all related and neighboring rights, to the extent allowed by law.

You can copy, modify, distribute and perform the work, even for commercial purposes, all without asking permission.
