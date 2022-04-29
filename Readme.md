# TODO-Highlight-Example
An Example of How you could use the 
[VSCode TODO-Highlight Extension
](https://marketplace.visualstudio.com/items?itemName=wayou.vscode-todo-highlight) Efficiency, Making a better DEV by configuring custom TODO Hilight Settings Into your/team Project.

## STEPS
* Craete .vscode folder in the root of your project folder.
* Create a json file named "settings.json" and insert this little spices into it.
```
// settings.json 
{
    "todohighlight.defaultStyle": {
        // overall style
        "color": "#fff",
        "backgroundColor": "#82A284",   
        "cursor": "pointer",
        "isWholeLine": false,
        //other styling properties goes here ... 
    },
    "todohighlight.isEnable": true,
    "todohighlight.isCaseSensitive": true,
    "todohighlight.keywords": [
        "DEBUG:",
        "REVIEW:",
        {
            "text": "NOTE:",
            "backgroundColor": "#DA121A",
        },
        {
            "text": "HACK:",
            "backgroundColor": "#009B3A",
            "isWholeLine": false,
        },
        {
            "text": "MEMBER:",
            "backgroundColor": "#FED100",
        },
        {
            "text": "SECTION:",
            "backgroundColor": "#525E75",
            "isWholeLine": true,
        },
        {
            "text": "SUBSECTION:",
            "backgroundColor": "#78938A",
            "isWholeLine": true,
        }
        
    ],
    /**
    // UnComment to enable todohighlight in all even defualt style TODO & FIXME keywords
    "todohighlight.keywordsPattern": "TODO:|FIXME:|\\(([^)]+)\\)", //highlight `TODO:`,`FIXME:` or content between parentheses
    */
    "todohighlight.include": [
        "**/*.js",
        "**/*.jsx",
        "**/*.ts",
        "**/*.tsx",
        "**/*.html",
        "**/*.php",
        "**/*.css",
        "**/*.scss"
    ],
    "todohighlight.exclude": [
        "**/node_modules/**",
        "**/bower_components/**",
        "**/dist/**",
        "**/build/**",
        "**/.vscode/**",
        "**/.github/**",
        "**/_output/**",
        "**/*.min.*",
        "**/*.map",
        "**/.next/**"
    ],
    "todohighlight.maxFilesForSearch": 5120,
    "todohighlight.toggleURI": false
}
```
* start modifying it the way you like!
## Check TODO-Highlight official [Todo Highlight Documentations](https://github.com/wayou/vscode-todo-highlight)