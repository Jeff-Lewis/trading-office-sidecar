# To be removed

To make an exact duplicate, you need to perform both a bare-clone and a mirror-push.

Open up the command line, and type these commands:
```
git clone --bare https://github.com/spolnik/trading-office-service-template.git
# Make a bare clone of the repository

cd trading-office-service-template.git
git push --mirror https://github.com/spolnik/trading-office-<new service name>.git
# Mirror-push to the new repository

cd ..
rm -rf trading-office-service-template.git
# Remove our temporary local repository
```

# Trading Office - Template Service
[![Build Status](https://travis-ci.org/spolnik/trading-office-template-service.svg?branch=master)](https://travis-ci.org/spolnik/trading-office-template-service) [![codecov.io](https://codecov.io/github/spolnik/trading-office-template-service/coverage.svg?branch=master)](https://codecov.io/github/spolnik/trading-office-template-service?branch=master) [![Sonar Coverage](https://img.shields.io/sonar/https/sonar-nprogramming.rhcloud.com/trading-office-template-service/coverage.svg)](https://sonar-nprogramming.rhcloud.com/dashboard/index/1) [![Sonar Tech Debt](https://img.shields.io/sonar/https/sonar-nprogramming.rhcloud.com/trading-office-template-service/tech_debt.svg)](https://sonar-nprogramming.rhcloud.com/dashboard/index/1)

Trading Office is reference implementation of microservices architecture, based on Spring Boot. It's modeling part of post trade processing, mainly focused on receiving Fixml message and preparing confirmation for it.

- [Trading Office](#trading-office)
- [Template Service](#template-service)
- [Notes](#notes)

## Trading Office

- [Trading Office](https://github.com/spolnik/trading-office)

## Template Service
- spring boot web application

Heroku: http://template-service.herokuapp.com/swagger-ui.html

![Component Diagram](https://raw.githubusercontent.com/spolnik/trading-office-template-service/master/design/template_service.png)

## Notes
- checking if [dependencies are up to date](https://www.versioneye.com/user/projects/56ad39427e03c7003ba41427)