# git Installation Instructions

You'll need git version 2.14.1 or later.

If you already have git, then make sure it's a recent enough version by doing a `git --version` at the command line.

## Download and Install git

If you haven't already installed `git`, go to [this site](https://git-scm.com) to download and install.

## Visa Setup

There is additional information found on this page:

https://visawiki.trusted.visa.com/display/VDP/New+Developer+Onboarding+Checklist

**Note:** Search the page for "Git Config"

## Set Up Configuration

It's important to have git configuration with your name and email.

```
git config --global user.name "Mona Lisa"

git config --global user.email "mona.lisa@example.com"
```

## Verify Configuration

Make sure that the configuration is correct by doing:

```
git config --global user.name

git config --global user.email
```

and making sure the output matches what you set above.
