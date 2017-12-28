# Admin Panel Nodes SSO 🔑
[![Swift Version](https://img.shields.io/badge/Swift-3-brightgreen.svg)](http://swift.org)
[![Vapor Version](https://img.shields.io/badge/Vapor-2-F6CBCA.svg)](http://vapor.codes)
[![Circle CI](https://circleci.com/gh/nodes-vapor/sugar/tree/master.svg?style=shield)](https://circleci.com/gh/nodes-vapor/sugar)
[![codebeat badge](https://codebeat.co/badges/fa667bac-85c1-4776-aaef-fdfea294e2c9)](https://codebeat.co/projects/github-com-nodes-vapor-admin-panel-nodes-sso-master)
[![codecov](https://codecov.io/gh/nodes-vapor/admin-panel-nodes-sso/branch/master/graph/badge.svg)](https://codecov.io/gh/nodes-vapor/admin-panel-nodes-sso)
[![Readme Score](http://readme-score-api.herokuapp.com/score.svg?url=https://github.com/nodes-vapor/admin-panel-nodes-sso)](http://clayallsopp.github.io/readme-score?url=https://github.com/nodes-vapor/admin-panel-nodes-sso)
[![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)](https://raw.githubusercontent.com/nodes-vapor/admin-panel-nodes-sso/master/LICENSE)

## 📦 Installation

Update your `Package.swift` file.
```swift
.Package(url: "https://github.com/nodes-vapor/admin-panel-nodes-sso.git", majorVersion: 0, minorVersion: 4)
```

## 🚀 Getting started

```swift
import AdminPanelNodesSSO
```

Add the Provider:

```swift
try addProvider(AdminPanelNodesSSO.Provider.self)
```

The `nodes.png` goes into `Public/images/`.

## 🔧 Configurations

Make sure configs are added to `adminpanel-sso-nodes.json`:

| Key            | Example value                         | Required | Description                              |
| -------------- | ------------------------------------- | -------- | ---------------------------------------- |
| `redirectUrl`  | `http://provider.com/sso/my-web-site` | Yes      | The url used for opening up the SSO login. |
| `salt`         | `som3Rand0mS4lt`                      | Yes      | The salt to use for the hasher.          |
| `loginPath`    | `/admin/sso/login`                    | No       | The project path to start the SSO flow.  |
| `callbackPath` | `/admin/sso/callback`                 | No       | The project path after user has logged in using SSO. |

## 🏆 Credits

This package is developed and maintained by the Vapor team at [Nodes](https://www.nodes.dk).
The package owner for this project is [Steffen](https://github.com/steffendsommer).

## 📄 License

This package is open-sourced software licensed under the [MIT license](http://opensource.org/licenses/MIT)
