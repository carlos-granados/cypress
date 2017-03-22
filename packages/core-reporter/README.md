# Cypress Core Reporter

![Reporter](https://cloud.githubusercontent.com/assets/1157043/17947006/bffba412-6a18-11e6-86ee-af7e9c9d614e.png)

The reporter shows the running results of the tests. It includes the following:

- A button to focus the list of test files
- Stats for number of tests passed, failed, and pending
- The total test run duration
- Control for toggling auto-scrolling
- Controls for various states (running, paused, stopped, etc.)
- A command log, showing:
  * suites
  * tests
  * hooks
  * commands and assertions with detailed information
  * any failures/errors
- Toggle-able auto-scrolling of command log


## Development

### Building

#### For development

```bash
npm run build-dev
```

#### For production

```bash
npm run build-prod
```

### Watching

- Runs `*.js` and `*.jsx` through babel and bundles with browserify into single `dist/reporter.js`
- Runs associated unit test of file saved and outputs to terminal
- Compiles `*.scss` files to single `dist/reporter.css`

```bash
npm run watch-dev
```

### Testing

```bash
npm test-once
```


## Changelog

#### 0.3.1 - *(10/13/16)*
- ensure command.renderProps is an object

#### 0.3.0 - *(10/03/16)*
- snapshot pinning

#### 0.2.0 - *(09/23/16)*
- handle being resized to any width
- fix issues with scrolling cutting off commands

#### 0.1.7 - *(09/13/16)*
- ensure direct dependencies get installed

#### 0.1.6 - *(09/07/16)*
- cleanup npm dist

#### 0.1.5 - *(08/30/16)*
- bump node, guard against logs which cannot be found

#### 0.1.4 - *(08/26/16)*
- minify prod css

#### 0.1.3 - *(08/26/16)*
- get font-awesome from npm instead of bower

#### 0.1.0 - *(08/23/16)*
- initial release