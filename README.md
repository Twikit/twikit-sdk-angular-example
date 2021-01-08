# Twikit SDK - Angular Example

This repository contains instructions to create a minimal Angular example that uses the Twikit SDK and Angular material design.

[Screenshot of this project](docs/TwikitAngularExampleApp.png)

## Installation
The installation instructions require the latest version of (Npm)[https://www.npmjs.com/get-npm] and Angular client `npm install -g @angular/cli` to be installed.

Before getting started, make sure you have the latest web plugin url that links to your products. If you don't have a web plugin URL yet and would just like to try the SDK, the following plugin URL can be used: https://sites.twikit.com/AutoDemo/production-2020-12-23-165832114/plugin-script.js.

1. Create a new Angular project with a chosen `appName`.
```
cd <your_project_folder>
ng new <appName>App --directory ./
```
2. Add the Angular material design page and choose the appropriate theme. Answer yes to the posed questions.

```
ng add @angular/material
```
3. Add web plugin module with the actual pluginUrl filled in.
```
npm set registry https://npm.twikit.com
ng add @twikit/angular-configurator --pluginUrl "<pluginUrl>" --name "<appName>"
```
4. Set the correct product key in the `ProductConfiguratorComponent`. If you are using the test plugin url provided above, one of the available product keys is 'wheel'. The path to the component file is `<your_project_folder>/src/app/product-configurator/configurator-component/product-configurator.component.ts`.
5. Now you can test the application and open it in the browser `http://localhost:4200/`.
```
npm start
```

Enjoy developing!

## Support

Contact our support team for questions, bug reports and feature suggestions at (support.twikit.com)[support.twikit.com].

## About Twikit

Twikit enables companies to digitally manufacture individualized products on-demand at a large scale. The Twikbot subscription based software works end-to-end across industries to revolutionize the customer experience.

Visit our website for more information: (https://www.twikit.com)[https://www.twikit.com].
