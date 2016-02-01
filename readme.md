## Sitecore Experience Editor Reset CSS

This css class can be used to "reset" the Sitecore Experience Editor styles when using a framework like bootstrap.

Save the css file into your assets folder. Then add the following to your layouts (or wherever you add your CSS).

```csharp
@if (Sitecore.Context.PageMode.IsPageEditor()) {
    <link href="/assets-path/ee-reset-{version}.css" rel="stylesheet" />
}
```

As we find more issues that need resetting, they will be added to this repository.

Select the correct CSS file to use based on the framework and version based on the chart below:

|Reset Version    |Foundation    |Bootstrap     |Sitecore      |
|-----------------|--------------|--------------|--------------|
|v1               |              |         3.3.0|     8.1-8.1u1|



Credits to [@jammykam](https://twitter.com/jammykam) & @jrodsmitty for the Slack conversation that started this off and @jammykam for the initial CSS fixes!