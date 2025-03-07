# bulma-calendar
Bulma's extension to display a calendar. It can be used on page as large calendar with apointments or in modal/popup for datepicker.

# Installation/Development
- Install ruby version 2.6.10 from [Ruby 2.6.10](https://mirror.sjtu.edu.cn/github-release/oneclick/rubyinstaller2/releases/download/RubyInstaller-2.6.10-1/rubyinstaller-devkit-2.6.10-1-x64.exe)
- Make sure to run ridk install in the end of Ruby install
- Then run `gem install bundler`
- Then run `bundler install` from working dir
- Then make sure you are using node version 8 (nvm install 8)
- Then run `npm install` from working folder
- Then run `npm install -g gulp-cli` to install gulp
- Then to start the live site, run `gulp demo`

[![npm](https://img.shields.io/npm/v/bulma-calendar.svg)](https://www.npmjs.com/package/bulma-calendar)
[![npm](https://img.shields.io/npm/dm/bulma-calendar.svg)](https://www.npmjs.com/package/bulma-calendar)
[![Build Status](https://travis-ci.org/Wikiki/bulma-calendar.svg?branch=master)](https://travis-ci.org/Wikiki/bulma-calendar)

# Examples

### Date format

```js
var calendars = new bulmaCalendar('.bulmaCalendar', {
    dateFormat: 'dd.MM.yyyy' // 01.01.2021
});
```

where `dateFormat` is a string with a combination of this values:

```
d: short day (1-31)
dd: long day (00-31)
EEE: short weekday (es: Mon)
EEEE: long weekday (es: Monday)
M: short month (1-12)
MM: long month (01-12)
MMM: short month name (es: Jan, Feb)
MMMM: full month name (es: January)
yy: short year (18)
yyyy: full year (2018)
```

For more values take a look at the [date-fns 2.x format](https://date-fns.org/v2.21.3/docs/format).

### Language

```js

var calendars = new bulmaCalendar('.bulmaCalendar', {
    lang: 'it' // refer to date-fns locales
});
```

### Default Options

Here's the options object and the default values as appears on code. For more options, please see the documentation.

```js
var defaultOptions = {
    color: 'primary',
    isRange: false,
    allowSameDayRange: true,
    lang: 'en-US',
    startDate: undefined,
    endDate: undefined,
    minDate: null,
    maxDate: null,
    disabledDates: [],
    disabledWeekDays: undefined,
    highlightedDates: [],
    weekStart: 0,
    dateFormat: 'MM/dd/yyyy',
    enableMonthSwitch: true,
    enableYearSwitch: true,
    displayYearsCount: 50,
};
```

# Documentation & Demo

You can find the full Documentation and a demo [here](https://doc.mh-s.de/bulma-calendar)
