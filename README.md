# Bundle Assets

Mods Entry Template
```
[
  {
    name:String [required] (name of category)
    icon:String [optional] (icon of category)
    entries:{
      enabled:Boolean [optional: default false] (whether or not the mod is enabled by default)
      id:String [required] (the internal id of mod)
      name:String [required] (display name of mod)
      version:String [required] (mod version - does not need to follow semver specification however it does need to match what is in mcmod.info)
      description:String [optional] (description of mod)
      download:String [optional: won't download if empty] (download url - link shorteners are not allowed because the download links could be changed to unverified jars)
      icon:String [optional: will use creator icon] (local repo image path to icon e.g. "isxander.png" is "https://github.com/Forgery-Client/Forgery-Client-Assets/assets/images/isxander.png")
      creator:String [optional: will use unknown creator entry] (id of creator from creators.json)
      links:{
        name:String [required] (name of link)
        url:String [required] (url)
      } [optional] (links of mod)
      warning:[String] [optional] (lines of a warning message)
      mods:[String] [optional] (required mod ids)
      packs:[String] [optional] (required pack ids)
      files:[String] [optional] (files to download from mcdir folder)
    } [required] (mod entries)
  }
]
```
