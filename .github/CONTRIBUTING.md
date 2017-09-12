# How to become a contributor and submit your own code

**Table of contents**

* [Contributor License Agreements](#contributor-license-agreements)
* [Contributing a patch](#contributing-a-patch)
* [Running the tests](#running-the-tests)
* [Releasing the library](#releasing-the-library)

## Contributor License Agreements

We'd love to accept your sample apps and patches! Before we can take them, we
have to jump a couple of legal hurdles.

Please fill out either the individual or corporate Contributor License Agreement
(CLA).

  * If you are an individual writing original source code and you're sure you
    own the intellectual property, then you'll need to sign an [individual CLA]
    (https://developers.google.com/open-source/cla/individual).
  * If you work for a company that wants to allow you to contribute your work,
    then you'll need to sign a [corporate CLA]
    (https://developers.google.com/open-source/cla/corporate).

Follow either of the two links above to access the appropriate CLA and
instructions for how to sign and return it. Once we receive it, we'll be able to
accept your pull requests.

## Contributing A Patch

1. Submit an issue describing your proposed change to the repo in question.
1. The repo owner will respond to your issue promptly.
1. If your proposed change is accepted, and you haven't already done so, sign a
   Contributor License Agreement (see details above).
1. Fork the desired repo, develop and test your code changes.
1. Ensure that your code adheres to the existing style in the sample to which
   you are contributing. Refer to the
   [Google Cloud Platform Samples Style Guide]
   (https://github.com/GoogleCloudPlatform/Template/wiki/style.html) for the
   recommended coding standards for this organization.
1. Ensure that your code has an appropriate set of unit tests which all pass.
1. Submit a pull request.

## Running the tests

1.  [Prepare your environment for Node.js setup][setup].
1.  Install [SemistandardJS](https://github.com/Flet/semistandard).

        npm install -g semistandard

1.  Install dependencies:

        npm install

1.  Run the tests:

        export GCLOUD_PROJECT=your-project-id
        export GOOGLE_APPLICATION_CREDENTIALS=/path/to/keyfile.json
        npm test

[setup]: https://cloud.google.com/nodejs/docs/setup

## Releasing the library

1.  Run the tests, see above.
1.  Bump the version in `package.json`.
1.  Commit and push changes. Commit message should be the new version number.
1.  Publish to `npm`:

        npm publish .

1.  Run the release script:

        npm run release

    You will need access to the `cloud-docs-samples` project to run this script.
