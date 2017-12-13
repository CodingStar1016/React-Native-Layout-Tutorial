### This repository is currently under development and the information provided may be subject to changes.

# react-sidenav [![build status](https://travis-ci.org/trendmicro-frontend/react-sidenav.svg?branch=master)](https://travis-ci.org/trendmicro-frontend/react-sidenav) [![Coverage Status](https://coveralls.io/repos/github/trendmicro-frontend/react-sidenav/badge.svg?branch=master)](https://coveralls.io/github/trendmicro-frontend/react-sidenav?branch=master)

[![NPM](https://nodei.co/npm/@trendmicro/react-sidenav.png?downloads=true&stars=true)](https://nodei.co/npm/@trendmicro/react-sidenav/)

React SideNav

Demo: https://trendmicro-frontend.github.io/react-sidenav

## Installation

1. Install the latest version of [react](https://github.com/facebook/react) and [react-sidenav](https://github.com/trendmicro-frontend/react-sidenav):

  ```
  npm install --save react @trendmicro/react-sidenav
  ```

2. At this point you can import `@trendmicro/react-sidenav` and its styles in your application as follows:

  ```js
  import SideNav, { Toggle, Nav, NavItem, NavIcon, NavText } from '@trendmicro/react-sidenav';

  // Be sure to include styles at some point, probably during your bootstraping
  import '@trendmicro/react-sidenav/dist/react-sidenav.css';
  ```

## Usage

```js
<SideNav>
    <SideNav.Toggle />
    <SideNav.Nav defaultSelected="home">
        <NavItem eventKey="home">
            <NavIcon>
                <i className="fa fa-fw fa-home" style={{ fontSize: '1.75em' }} />
            </NavIcon>
            <NavText>
                Home
            </NavText>
        </NavItem>
        <NavItem eventKey="charts">
            <NavIcon>
                <i className="fa fa-fw fa-line-chart" style={{ fontSize: '1.75em' }} />
            </NavIcon>
            <NavText>
                Charts
            </NavText>
            <NavItem eventKey="charts/linechart">
                <NavText>
                    Line Chart
                </NavText>
            </NavItem>
            <NavItem eventKey="charts/barchart">
                <NavText>
                    Bar Chart
                </NavText>
            </NavItem>
        </NavItem>
    </SideNav.Nav>
</SideNav>
```

## API

### Properties

## License

MIT
