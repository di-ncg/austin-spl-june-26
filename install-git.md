# git Installation Instructions

You'll need git version 2.11 or later (2.13 is the latest).

If you already have git, then make sure it's a recent enough version by doing a `git --version` at the command line.
If you have 2.11 or later, then skip to setting up the configuration section below.

## Set Up Configuration

It's important to have git configuration with your name and email.

```
git config --global user.name "Mona Lisa"

git config --global user.email "mona.list@example.com"
```

## Verify Configuration

Make sure that the configuration is correct by doing:

```
git config --global user.name

git config --global user.email
```

and making sure the output matches what you set above.
