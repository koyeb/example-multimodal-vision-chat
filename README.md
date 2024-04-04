<div align="center">
  <a href="https://koyeb.com">
    <img src="https://www.koyeb.com/static/images/icons/koyeb.svg" alt="Logo" width="80" height="80">
  </a>
  <h3 align="center">Koyeb Serverless Platform</h3>
  <p align="center">
    Deploy a Multimodal Vision Chat application using LLaVA, Chainlit, and Replicate on Koyeb
    <br />
    <a href="https://koyeb.com">Learn more about Koyeb</a>
    ·
    <a href="https://koyeb.com/docs">Explore the documentation</a>
    ·
    <a href="https://koyeb.com/tutorials">Discover our tutorials</a>
  </p>
</div>

## About Koyeb and the example Multimodal Vision Chat application using LLaVA, Chainlit, and Replicate

Koyeb is a developer-friendly serverless platform to deploy apps globally. No-ops, servers, or infrastructure management.
This repository contains a Multimodal Vision Chat application clone you can deploy on the Koyeb serverless platform for testing.

This example application is designed to show how an application using LLaVA, Chainlit, and Replicate can be deployed on Koyeb.

## Getting Started

Follow the steps below to deploy and run the Multimodal Vision Chat application on your Koyeb account.

### Requirements

You need a Koyeb account to successfully deploy and run this application. If you don't already have an account, you can sign-up for free [here](https://app.koyeb.com/auth/signup).

### Deploy using the Koyeb button

The fastest way to deploy the Multimodal Vision Chat application is to click the **Deploy to Koyeb** button below.

[![Deploy to Koyeb](https://www.koyeb.com/static/images/deploy/button.svg)](https://app.koyeb.com/deploy?name=example-llava-chainlit&type=git&repository=koyeb%2Fexample-multimodal-vision-chat&branch=main&builder=buildpack&run_command=chainlit+run+app.py&env%5BREPLICATE_API_KEY%5D=CHANGE_ME&env%5BREPLICATE_MODEL%5D=yorickvp/llava-v1.6-mistral-7b&env%5BREPLICATE_MODEL_VERSION%5D=19be067b589d0c46689ffa7cc3ff321447a441986a7694c01225973c2eafc874&ports=8000%3Bhttp%3B%2F)

Clicking on this button brings you to the Koyeb App creation page with everything pre-set to launch this application.

_To modify this application example, you will need to fork this repository. Checkout the [fork and deploy](#fork-and-deploy-to-koyeb) instructions._

### Fork and deploy to Koyeb

If you want to customize and enhance this application, you need to fork this repository.

If you used the **Deploy to Koyeb** button, you can simply link your service to your forked repository to be able to push changes.
Alternatively, you can manually create the application as described below.

On the [Koyeb Control Panel](//app.koyeb.com/apps), click the **Create Web Service** button to go to the App creation page.

1. Select GitHub as your deployment method.
2. Choose the repository where your code resides. For example, ChatbotFastUI.
3. Under **Builder** configure your Run command by selecting Override and adding the command to run the application with public access: `chainlit run app.py`
4. Under **Environment variables**, click **Add variable** to add your Replicate API key named `REPLICATE_API_KEY` . Add also the `REPLICATE_MODEL` and `REPLICATE_MODEL_VERSION`.
5. In the Instance selection, click “Eco” and select "Free".
6. Under **App and Service names**, rename your App to whatever you’d like. For example, `vision-chat`. Note the name will be used to create the public URL for this app. You can [add a custom domain](https://www.koyeb.com/docs/run-and-scale/domains) later if you’d like.
7. Finally, click the Deploy button or hit **⌘**D.

You land on the deployment page where you can follow the build of your application. Once the build is completed, your application is being deployed and you will be able to access it via `<YOUR_APP_NAME>-<YOUR_ORG_NAME>.koyeb.app`.

## Contributing

If you have any questions, ideas or suggestions regarding this application sample, feel free to open an [issue](https://github.com/koyeb/example-multimodal-vision-chat/issues) or fork this repository and open a [pull request](https://github.com/koyeb/example-multimodal-vision-chat/pulls).

## Contact

[Koyeb](https://www.koyeb.com) - [@gokoyeb](https://twitter.com/gokoyeb) - [Slack](http://slack.koyeb.com/)
