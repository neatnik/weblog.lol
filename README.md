# weblog.lol GitHub Action

This repository holds the weblog.lol GitHub Action. All other omg.lol material (including weblog.lol stuff) can be found in the [omg.lol repository](http://github.com/neatnik/omg.lol/).

## Setting up the action

1. First, create a GitHub repo to hold your weblog content.

2. Add the file `.github/workflows/main.yml` with this content in it:

```
on: [push]

jobs:
  weblog_import:
    runs-on: ubuntu-latest
    name: weblog.lol
    steps:
      - uses: actions/checkout@v3
        with:
          fetch-depth: 2
      - id: weblog_import
        uses: neatnik/weblog.lol@v1
        env:
          ADDRESS: your-address-here
          WEBLOG_API_KEY: ${{ secrets.WEBLOG_API_KEY }}
```

3. Change the `your-address-here` value above to your own omg.lol address (just the address itself, e.g. `foobar`).

4. In your repo settings, click **Secrets**, and then **Actions**. Click **New repository secret**, and add the following:

  - Name: `WEBLOG_API_KEY`
  - Secret: _your omg.lol API key_ (you can find this on [your omg.lol account page](https://home.omg.lol/account), at the very bottom)

5. Add a folder to your repo called `weblog`. You can store your posts here, using whatever directory structure you’d like.

6. _Optional:_ Add a folder to your repo called `configuration`. In that folder, you can store your `template.html` file and your `weblog.conf` file if you’d like to manage your template and configuration through your repo.