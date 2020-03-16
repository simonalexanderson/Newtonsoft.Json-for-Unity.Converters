# Unity Converters for Newtonsoft.Json

[![CircleCI](https://img.shields.io/circleci/build/gh/jilleJr/Newtonsoft.Json-for-Unity.Converters/master?logo=circleci&style=flat-square)](https://circleci.com/gh/jilleJr/Newtonsoft.Json-for-Unity.Converters)
[![Codacy grade](https://img.shields.io/codacy/grade/de7041b5f9f9415a8add975d1b8a9fcf?logo=codacy&style=flat-square)](https://www.codacy.com/manual/jilleJr/Newtonsoft.Json-for-Unity.Converters?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=jilleJr/Newtonsoft.Json-for-Unity.Converters&amp;utm_campaign=Badge_Grade)
[![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-v2.0%20adopted-ff69b4.svg?style=flat-square)](/CODE_OF_CONDUCT.md)

This package contains converters to and from common Unity types. Types such as
Vector2, Vector3, Matrix4x4, Quaternions, Color, and more.

The perfect complement to the [jilleJr/Newtonsoft.Json-for-Unity][jillejr.newtonsoft.json-for-unity] repo.

# ❌ NOT RELEASED YET ❌

Click the "Watch" button at the top to get an email when we release.

## Prerequisites

The Newtonsoft.Json library of the correct Major version added to your project.

Recommended to use the [jillejr.newtonsoft.json-for-unity][jillejr.newtonsoft.json-for-unity] package.

## Installation via Unity Package Manager

### If you already have the jilleJr/Newtonsoft.Json-for-Unity scoped registry configured

> If you have the jillejr.newtonsoft.json-for-unity package installed, then
> most probably yes, you have the scoped registry configured.

1. Open the Package Manager UI `Window > Package Manager`

    ![preview of where window button is](https://i.imgur.com/0FvA5W6.png)

2. Make sure you're viewing "All packages" and not just "In Project"

3. Search for `json`

4. Click the "Json .NET Converters of Unity types" package

    ![showing search results](https://i.imgur.com/1d7yoVE.png)

5. Click "Install"

    ![install button down at bottom right](https://i.imgur.com/uGZn64c.png)

### If you don't have the jilleJr/Newtonsoft.Json-for-Unity scoped registry configured

Open `<project>/Packages/manifest.json`, add scope for `jillejr`, then add the
package in the list of dependencies.

À la:

```json
{
  "scopedRegistries": [
    {
      "name": "Packages from jillejr",
      "url": "https://npm.cloudsmith.io/jillejr/newtonsoft-json-for-unity/",
      "scopes": ["jillejr"]
    }
  ],
  "dependencies": {
    "jillejr.newtonsoft.json-for-unity": "12.0.101",
    "jillejr.newtonsoft.json-for-unity.converters": "12.0.1",

    //...
  }
}
```

Done!

## Updating the package

### Updating via the UI

Open the Package Manager UI `Window > Package Manager`

![where to open package manager window](https://i.imgur.com/0FvA5W6.png)

Followed by pressing the "Update to x.x.x" button down at the lower right while
having the `jillejr.newtonsoft.json-for-unity.converters` package selected.

![outdated package in package list](https://i.imgur.com/plejYzI.png)
![update button](https://i.imgur.com/iJsGyFy.png)

## Versioning format

To use the package with Newtonsoft.Json, you must match the Major component of
the versions for it to compile. The rest of the components are reserved for
the iterations of this package, Newtonsoft.Json-for-Unity.Converts.

![explanation of version][version-explanation.png]

Where official Json.NET 12.0.1 becomes Newtonsoft.Json-for-Unity.Converters
12.*xx.xx*.

## Changelog

Please see the [CHANGELOG.md][changelog.md] file inside this package.

---

This package is licensed under The MIT License (MIT)

Copyright (c) 2019 Kalle Jillheden (jilleJr)  
<https://github.com/jilleJr/Newtonsoft.Json-for-Unity.Converters>

See full copyrights in [LICENSE.md][license.md] inside repository

[license.md]: /LICENSE.md
[changelog.md]: /CHANGELOG.md
[version-explanation.png]: /Doc/version-explanation.png
[jillejr.newtonsoft.json-for-unity]: https://github.com/jilleJr/Newtonsoft.Json-for-Unity#readme
