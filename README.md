# Cordova sqlite evcore-extbuild-free PhoneGap Build Windows 10 ARM test app

PhoneGap Build test app with `cordova-sqlite-evcore-extbuild-free` for Windows 10 ARM architecture

**AUTHOR:** [@brodybits (Christopher J. Brody aka Chris Brody)](https://github.com/brodybits)

**LICENSE:** [CC0 1.0 (public domain)](https://creativecommons.org/publicdomain/zero/1.0/)

**NOTE:** This project includes JQuery (2.2.4) and Bootstrap (3.3.6) under the MIT license. Otherwise there is no code copied from other sources.

**IMPORTANT:** Whitelist and intent items are omitted from this test app.

## Dependencies

- Bootstrap (3.3.6) - included (MIT license)
- JQuery (2.2.4) - included (MIT license)
- `cordova-plugin-dialogs` - specified in `config.xml` (Apache license)
- `cordova-sqlite-evcore-extbuild-free` (GPL or commercial license terms)

NOTE: `cordova-plugin-dialogs` and `cordova-sqlite-evcore-extbuild-free` were added using the `--save` flag to ensure that these plugin would be automatically installed. It is recommended to use the `--save` flags to add any other plugins rather than adding such plugins to git.

## To add another plugin

```shell
cordova plugin add my-plugin-id --save
```

## Functionality

- Upon startup: open a database and CREATE the test table
- Native alert dialog test
- Echo test
- Self test
- Location reload
- String test 1
- String test 2 (string as a SQL parameter)
- Show record
- Add record
- Add 100 records from JavaScript object after delay
- Delete all records
- Follow link to page 2
- Change window.location to page 2

## Multi-page test

It is possible to switch between two pages using "follow link" buttons. The main page also has a button to go to page 2 by changing `window.location`. There is also a button on both pages to try `location.reload()`.

The sqlite plugin should continue to work after the user changes to another page or triggers `location.reload()`.
