[![Jovo Framework](https://www.jovo.tech/img/github-logo.png)](https://www.jovo.tech)

<p align="center">Typescript Sample Voice App for the <a href="https://github.com/jovotech/jovo-framework-nodejs">Jovo Framework</a> ⭐️</p>

<p align="center">
<a href="https://www.jovo.tech/docs/"><strong>Documentation</strong></a> -
<a href="https://github.com/jovotech/jovo-cli"><strong>CLI </strong></a> - <a href="https://github.com/jovotech/jovo-templates"><strong>Templates </strong></a> -<a href="https://github.com/jovotech/jovo-framework/blob/master/.github/CONTRIBUTING.md"><strong>Contributing</strong></a> - <a href="https://twitter.com/jovotech"><strong>Twitter</strong></a></p>
<br/>

# Typescript Sample Voice App for Jovo

```javascript
app.setHandler({
    LAUNCH() {
        this.toIntent('HelloWorldIntent');
    },

    HelloWorldIntent() {
        this.ask('Hello World! What\'s your name?', 'Please tell me your name.');
    },

    MyNameIsIntent() {
        this.tell('Hey ' + this.$inputs.name.value + ', nice to meet you!');
    },
});
```

[Jovo](https://www.jovo.tech "Jovo's website") is a development framework for cross-platform voice apps. Use this repository as a starting point to create a voice application for Amazon Alexa and Google Assistant in Typescript.

> 🚀 Join our newsletter for free courses on voice app development: www.jovo.tech/newsletter 



## Getting Started

In this guide, you will learn how to create a "Hello World" voice app for both Amazon Alexa and Google Assistant.

### Install the Jovo CLI

The [Jovo CLI](https://github.com/jovotech/jovo-cli) is the best way to get started with Jovo development:

```sh
$ npm install -g jovo-cli
```

To learn more, please find the [Getting Started Guide](https://www.jovo.tech/framework/docs/installation) in the Jovo Framework Docs.

### Clone this repository

```sh
$ git clone https://github.com/jovotech/jovo-sample-voice-app-typescript.git

$ cd jovo-sample-voice-app-typescript

$ npm install
```


### Run the Code

```sh
# Compile Typescript
$ npm tsc

# Run Jovo development server (./dist/index.js)
$ jovo run
```