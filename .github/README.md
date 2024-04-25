# Umbraco Forms sanitiser

[![Downloads](https://img.shields.io/nuget/dt/Umbraco.Community.Sanitiser.Forms?color=cc9900)](https://www.nuget.org/packages/Umbraco.Community.Sanitiser.Forms/)
[![NuGet](https://img.shields.io/nuget/vpre/Umbraco.Community.Sanitiser.Forms?color=0273B3)](https://www.nuget.org/packages/Umbraco.Community.Sanitiser.Forms)
[![GitHub license](https://img.shields.io/github/license/richarth/sanitiser.forms?color=8AB803)](https://github.com/richarth/sanitiser.forms/blob/main/LICENSE)

When enabled, this package will delete form submissions and files uploaded as part of form submissions.

Umbraco versions supported: v10.8.5+

Umbraco Forms versions supported: v10.5.5+

## Installation

Add the package to your Umbraco website from nuget:

`dotnet add package Umbraco.Community.Sanitiser.Forms`

## Configuration

To enable the package, add the following to your `appsettings.json`:

```json
{
  "Sanitiser": {
    "Enabled": true
  }
}
```

### Umbraco Forms Submissions

To enable the deletion of form submissions, add the following to your `appsettings.json`:

```json
{
    "Sanitiser": {
        "Enabled": true,
        "UmbracoFormsSanitiser": {
            "Enable": true
        }
    }
}
```

> [!WARNING]
> N.B. This package is not intended to be run on production sites, only enable sanitization on a development or staging
> environment. Before enabling please ensure you have a backup of your data and a backup of your backup.
>
>If there is a lot of data then the startup of your site may be delayed. Only enable when necessary.

## Acknowledgements

### Logo

The package logo uses the [form](https://thenounproject.com/icon/form-6440981/)
(by [Icogenix](https://thenounproject.com/creator/asmahameed743/)) icon from
the [Noun Project](https://thenounproject.com), licensed
under [CC BY 3.0 US](https://creativecommons.org/licenses/by/3.0/us/).

## License

MIT License
