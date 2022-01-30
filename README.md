# srpg-modloader
official mod loader for simplerpg, currently for version ```2.2a```!  
support for newest stable version ```2.2a``` is here!  
It also brings actual file patching ( merging ), so you can stack mods!  

clone and do ```python3 modloader.py``` now!  

## How to create a mod?
First, see [modrepo](https://github.com/reversee-dev/srpg-modrepo) for examples.  
Next, clone supported version of SimpleRPG and modify it!  
When you are done, create a folder and recreate file and folder structure for modded files!   
Then create ```modmeta.json``` file in the root. Put the example below, and fill it!
```json
{
    "name": "My mod",
    "modver": "1.0",
    "srpgver": "m2.2a",
    "patchmode": "append / replace",
    
    "files":
    [
        "lib\\file1.py",
        "lib\\file2.py",
    ]
}
```  

**Note: "append" will append everything in modded files, so if you are using it.   
Make sure to delete all original content, and leave only modded!**   
  
**Note2: If you are both appending, and replacing, you need to break the mod into 2 pieces!** 
