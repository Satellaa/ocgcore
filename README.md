## How to use cores in this repo?

You can add the following structure to the `config/user_configs.json` file (create one if it doesn't exist).
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
Then go to the `config/configs.json` file and set `has_core` to `false`.

That's all! Just restart EDOPro and enjoy!

## Note
Currently, to use constants from `script/extra_constant.lua`, you must add `Duel.LoadScript("extra_constant.lua")` to the cards that use those constants. This issue will be fixed in the upcoming version of EDOPro, which will allow you to utilize `init.lua` in the repository.