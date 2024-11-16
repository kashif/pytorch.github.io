# pytorch.org site

[https://pytorch.org](https://pytorch.org)

A static website built in [Jekyll](https://jekyllrb.com/) and [Bootstrap](https://getbootstrap.com/) for [PyTorch](https://pytorch.org/), and its tutorials and documentation.

## Prerequisites

Install the following packages before attempting to setup the project:

- [rbenv](https://github.com/rbenv/rbenv)
- [ruby-build](https://github.com/rbenv/ruby-build)
- [nvm](https://github.com/creationix/nvm)

On OSX, you can use:

```bash
brew install rbenv ruby-build nvm
```

## Setup

#### Install required Ruby version:

```bash
#### You only need to run these commands if you are missing the needed Ruby version.
rbenv install `cat .ruby-version`
gem install bundler -v 2.5.23
rbenv rehash

bundle install
rbenv rehash
```

#### Install Node

```bash
nvm install
nvm use
```

#### Install Yarn

```bash
brew install yarn --ignore-dependencies
yarn install
```

## Local Development

To run the website locally for development:

```bash
make serve
```

Then navigate to [localhost:4000](localhost:4000).

To build the static website from source:

```bash
make build
```

This will build the static site at `./_site`. This directory is not tracked in git.

## Deployments

The website is hosted on [Github Pages](https://pages.github.com/) at [https://pytorch.org](https://pytorch.org).

To deploy changes, merge your latest code into the `site` branch. A build will be automatically built and committed to the `master` branch via a CircleCI job.

To view the status of the build visit [https://circleci.com/gh/pytorch/pytorch.github.io](https://circleci.com/gh/pytorch/pytorch.github.io).

## Contributing to PyTorch Documentation and Tutorials
* You can find information about contributing to PyTorch documentation in the 
PyTorch repo [README.md](https://github.com/pytorch/pytorch/blob/master/README.md) file. 
* Information about contributing to PyTorch Tutorials can be found in the 
tutorials [README.md](https://github.com/pytorch/tutorials/blob/master/README.md).
* Additional contribution information can be found in [PyTorch CONTRIBUTING.md](https://github.com/pytorch/pytorch/blob/master/CONTRIBUTING.md).
