## Where Do the Cores in This Repository Come From?

The cores in this repository are built from [Satellaa/ygopro-core](https://github.com/Satellaa/ygopro-core.git), with customizations to facilitate the creation of custom cards. Additionally, [Satellaa/ygopro-core](https://github.com/Satellaa/ygopro-core.git) is open to new feature requests and suggestions via issues.

## How To Use Cores in This Repository

To use the cores in this repository, follow these steps:

1. Add the following structure to the `config/user_configs.json` file. If the file does not exist, create it.

```json
{
	"repos": [
		{
			"url": "https://github.com/Satellaa/ocgcore.git",
			"repo_name": "OCG-core",
			"repo_path": "./repositories/OCG-core",
			"script_path": "script",
			"core_path": "bin",
			"has_core": true,
			"should_update": true,
			"should_read": true
		}
	]
}
```

2. Open the `config/configs.json` file and set `has_core` to `false`.

That's it! Simply restart EDOPro and enjoy your new setup.

## Note
Currently, to use constants from `script/extra_constant.lua`, you must add `Duel.LoadScript("extra_constant.lua")` to the cards that use those constants. This issue will be fixed in the upcoming version of EDOPro, which will allow you to utilize `init.lua` in the repository.