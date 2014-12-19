docker-protractor
=================

Docker File for Protractor (http://angular.github.io/protractor/)

Usage example:
'''bash
 docker run -it -v /home/username:/app 7982ac828f72 protractor /app/conf.js
'''

conf.js should contain link to slenium server runnig.
It is not included but works fine with https://github.com/SeleniumHQ/docker-selenium
Example below starts selenium server and firefox webdriver

'''bash
docker run -d -p 4444:4444 --name selenium-hub selenium/hub:2.44.0
docker run -d -p 4444:4444 --name selenium-hub selenium/node-chrome:2.44.0
'''

This is enough for defaul protractor conf.
Protractor conf

See also: http://angular.github.io/protractor/#/toc
