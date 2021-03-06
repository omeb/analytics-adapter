# analytics-adapter

[![Build Status](https://travis-ci.org/D-Mobilelab/analytics-adapter.svg?branch=master&v=1)](https://travis-ci.org/D-Mobilelab/analytics-adapter)
[![Coverage Status](https://coveralls.io/repos/github/D-Mobilelab/analytics-adapter/badge.svg?branch=master&v=1)](https://coveralls.io/github/D-Mobilelab/analytics-adapter?branch=master)
[![npm version](https://badge.fury.io/js/analytics-adapter.svg)](https://badge.fury.io/js/analytics-adapter)
[![Bower version](https://badge.fury.io/bo/analytics-adapter.svg)](https://badge.fury.io/bo/analytics-adapter)
[![GitHub version](https://badge.fury.io/gh/D-Mobilelab%2Fanalytics-adapter.svg?v=1)](https://badge.fury.io/gh/D-Mobilelab%2Fanalytics-adapter)

analytics-adapter is a interface for Google Analytics to tracking events, pageviews and custom dimensions

## Usage
```
// init Analytics and set 'User' custom dim to slot #3 and 'Valuable' to slot #4
AnalyticsAdapter.init({
	enabled: true,
	logger: console,
	dimensions: {
		User: 3,
		Valuable: 4
	}
});

// set 'User' custom dim, without re-specify the slot
AnalyticsAdapter.setDimension({
	User: 'logged'
});

// track pageview
AnalyticsAdapter.trackPage({
	page: '/home',
	title: 'Home Page',
	dimensions: {
		Valuable: false
	}
});

// track event
AnalyticsAdapter.trackEvent({
	category: 'Social',
	action: 'Click',
	label: 'Facebook',
	value: 3,
	dimensions: {
		Valuable: true
	}
});
```

## Installation

### NPM
```
npm install --save analytics-adapter
```
You can found the library ready for production on <i>node_modules/analytics-adapter/dist/dist.js</i>

### Bower
```
bower install --save analytics-adapter
```
You can found the library ready for production on <i>bower_components/analytics-adapter/dist/dist.js</i>

## Documentation

To read documentation, go to:

[http://d-mobilelab.github.io/analytics-adapter/1.0.0](http://d-mobilelab.github.io/analytics-adapter/1.0.0)

Replace <i>1.0.0</i> with the version of the documentation you want to read.
