# build-recipes-specification
A draft.

## Recipe list
A recipe file corresponds to a JSON file with the following format:
```
{
    <name>: <recipe>,
    <name>: <recipe>,
    <name>: <recipe>,
    ...
}
```

**name**: recipe's name.

**recipe**: a recipe object.

## A recipe object
A recipe object corresponds to an object with the following format:
```
{
    "type": <string>
    "includes": [<string>, ...],
    "files": [<string>, ...],
    "output": {
        "type": <string>, 
        "name": <string>,
        "folder": <string>
    }
}
```

**type**: "C" or "C++"

**includes**: list of folders with headers. optional.

**files**: list of files to compile.

**output** > **type**: output type (binary, static or dynamic).

**output** > **name**: output name.

**output** > **folder**: output folder.
