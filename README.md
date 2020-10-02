<h1 align="center">
  <br>
  <a href="https://webtorrent.io"><img src="https://github.com/frani/express-power-up/raw/master/images/logo.png" alt="Express-power-up-logo" width="200"></a>
  <br>
	Express power up <i>Snippets</i>
  <br>
  <br>
</h1>

<h4 align="center">The best tool to create ExpressJS APIs.</h4>

<p align="center">
  <a href="https://discord.gg/sYjKHC8"><img alt="Discord" src="https://img.shields.io/discord/759780590962212866"></a>
  <a href="https://marketplace.visualstudio.com/items?itemName=frani.express-power-up"><img src="https://img.shields.io/visual-studio-marketplace/v/frani.express-power-up?style=flat&logo=visual-studio-code&logoColor=blue" alt="VSCode-ext"></a>
  <a href="https://marketplace.visualstudio.com/items?itemName=frani.express-power-up"><img alt="Visual Studio Marketplace Installs" src="https://img.shields.io/visual-studio-marketplace/i/frani.express-power-up"></a>
</p>

# Demo

<p align="center">
  <img width="600" alt="Express Power Up - Demo" src="https://raw.githubusercontent.com/frani/express-power-up/master/images/demo.gif">
</p>

# About EPUs

- 100+ snippets
- Supports es6 syntax
- [airbnb javascript style](https://github.com/airbnb/javascript)

# Install

### Install with VScode:

To install the extension, open the Extensions view on sidenav, search for `express power up` to filter results and select `Express power up Snippets` authored by [Frani](https://github.com/frani).

### Install with Terminal:

```bash
code --install-extension frani.express-power-up
```

in case you have `code` command disable [see this link to enable it](https://code.visualstudio.com/docs/editor/command-line#_common-questions)

# Following Porject Structure

this snippets are thought to apply on ExpressJS with the next folder structure

| Folder       | Suffix Extention | description                                                                            |
| ------------ | ---------------- | -------------------------------------------------------------------------------------- |
| /config      | \*.conf.js       | Environment variables and configuration related things                                 |
| /routers     | \*.router.js     | Routers                                                                                |
| /controllers | \*.controller.js | route controller ( controller layer)                                                   |
| /services    | \*.service.js    | business logic, incluye intertal or externla servicies as SDK (service layer)          |
| /middlewares | \*.mid.js        | custom express middlewares                                                             |
| /validations | \*.validation.js | Request data validation schemas                                                        |
| /schemas     | \*.schema.js     | Mongoose models/schemas (data layer)                                                   |
| /dbs         | \*.db.js         | Function to manage Mongoose schemas                                                    |
| /helpers     | \*.helper.js     | Helpful functions that can be used in many places but is not necesary a business logic |
| /tests       | \*.test.js       | well... just tests for your API                                                        |


also http response follow the next structure:

```json
// Example:
// GET /v1/users/frani
{
  "success": true,
  "message": "User @frani found",
  "body": {
    "name": "frani",
    "email": "hi@frani.me",
    "github": "https://github.com/frani"
  }
}
```

# Snippets

**Application Snippets**

| Snippet                       | Description              |
| ----------------------------- | ------------------------ |
| `ep-app`                      | App Variable             |
| `ep-app-all`                  | All HTTP Requests        |
| `ep-app-get`                  | HTTP GET Requests        |
| `ep-app-post`                 | HTTP POST Requests       |
| `ep-app-put`                  | HTTP PUT Requests        |
| `ep-app-delete`               | HTTP DELETE Requests     |
| `ep-app-patch`                | HTTP PATCH Requests      |
| `ep-app-disable`              | App Disable              |
| `ep-app-disabled`             | App Disabled             |
| `ep-app-enable`               | App Enable               |
| `ep-app-enabled`              | App Enabled              |
| `ep-app-engine`               | App Engine               |
| `ep-app-param`                | App Param                |
| `ep-app-path`                 | App Path                 |
| `ep-app-render`               | App Render               |
| `ep-app-route`                | App Route                |
| `ep-app-set`                  | App Set                  |
| `ep-app-listen`               | App Listen               |
| `ep-app-listen-with-callback` | App Listen With Callback |
| `ep-app-use`                  | App Use                  |

**Examples Snippets**

| Snippet                 | Description      |
| ----------------------- | ---------------- |
| `ep-example-helloworld` | Hello World      |
| `ep-example-controller` | \*.controller.js |
| `ep-example-service`    | \*.service.js    |
| `ep-example-db`         | \*.db.js         |
| `ep-example-helper`     | \*.helper.js     |
| `ep-example-middleware` | \*.mid.js        |
| `ep-example-router`     | \*.router.js     |
| `ep-example-schema`     | \*.schema.js     |
| `ep-example-validation` | \*.validation.js |

The other example snippets are preparing...

**Handlers Snippets**

| Snippet          | Description     |
| ---------------- | --------------- |
| `ep-404-handler` | 404 - Not Found |
| `ep-500-handler` | 500 - Error     |

**Middleware Snippets**

| Snippet                   | Description                        |
| ------------------------- | ---------------------------------- |
| `ep-mid-helmet`           | Middleware Helmet                  |
| `ep-mid-morgan`           | Middleware Morgan                  |
| `ep-mid-compress`         | Middleware Compression             |
| `ep-mid-body-parser-json` | Middleware Body Parser Json        |
| `ep-mid-body-parser-url`  | Middleware Body Parser Url Encoded |
| `ep-mid-method-override`  | Middleware Method Override         |
| `ep-mid-static-file`      | Middleware Static File             |

**Module Snippets**

| Snippet        | Description                                  |
| -------------- | -------------------------------------------- |
| `ep-require`   | Require ExpressJs 4 Module or Another Module |
| `ep-namespace` | ExpressJs 4 Namespace                        |

**Request Snippets**

| Snippet                    | Description               |
| -------------------------- | ------------------------- |
| `ep-req-accepts`           | Request Accepts           |
| `ep-req-accepts-charsets`  | Request Accepts Charsets  |
| `ep-req-accepts-languages` | Request Accepts Languages |
| `ep-req-get`               | Request Get               |
| `ep-req-is`                | Request Is                |
| `ep-req-range`             | Request Range             |

**Response Snippets**

| Snippet                            | Description                        |
| ---------------------------------- | ---------------------------------- |
| `ep-res-append`                    | Response Append                    |
| `ep-res-attachment`                | Response Attachment                |
| `ep-res-cookie`                    | Response Cookie                    |
| `ep-res-cookie-with-options`       | Response Cookie With Options       |
| `ep-res-clear-cookie`              | Response Clear Cookie              |
| `ep-res-clear-cookie-with-options` | Response Clear Cookie With Options |
| `ep-res-download`                  | Response Download                  |
| `ep-res-end`                       | Response End                       |
| `ep-res-format`                    | Response Format                    |
| `ep-res-get`                       | Response Get                       |
| `ep-res-json`                      | Response Json                      |
| `ep-res-jsonp`                     | Response Jsonp                     |
| `ep-res-links`                     | Response Links                     |
| `ep-res-location`                  | Response Location                  |
| `ep-res-redirect`                  | Response Redirect                  |
| `ep-res-redirect-with-status`      | Response Redirect With Status      |
| `ep-res-render`                    | Response Render                    |
| `ep-res-send`                      | Response Send                      |
| `ep-res-send-file`                 | Response Send File                 |
| `ep-res-send-status`               | Response Send Status               |
| `ep-res-set`                       | Response Set                       |
| `ep-res-status`                    | Response Status                    |
| `ep-res-rss`                       | Response Rss                       |
| `ep-res-type`                      | Response Type                      |
| `ep-res-vary`                      | Response Vary                      |

**Router Snippets**

| Snippet            | Description                 |
| ------------------ | --------------------------- |
| `ep-router`        | ExpressJs 4 Router Variable |
| `ep-router-all`    | Router All                  |
| `ep-router-get`    | Router GET                  |
| `ep-router-post`   | Router POST                 |
| `ep-router-put`    | Router PUT                  |
| `ep-router-delete` | Router DELETE               |

**Test Snippets**

| Snippet                   | Description                                 |
| ------------------------- | ------------------------------------------- |
| `ep-test-describe-get`    | Create Describe and 'it' with GET method    |
| `ep-test-describe-post`   | Create Describe and 'it' with POST method   |
| `ep-test-describe-put`    | Create Describe and 'it' with PUT method    |
| `ep-test-describe-delete` | Create Describe and 'it' with DELETE method |
| `ep-test-it-get`          | Create 'it' test with GET method            |
| `ep-test-it-post`         | Create 'it' test with POST method           |
| `ep-test-it-put`          | Create 'it' test with PUT method            |
| `ep-test-it-delete`       | Create 'it' test with DELETE method         |

# Contributors

# Inspiration

- [expressjs4-snippets](https://github.com/gurayyarar/expressjs4-snippets)

# License

MIT © [Frani](http://github.com/frani)
