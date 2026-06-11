# Tomat0 Syntax Highlighting
A syntax highlighting vscode extension for my custom programming language Tomat0. The extension enables syntax highlighting for .tmt files and editor support such as bracket pairing. 

## Installing the Extension
You can find the extension under my publishing name "christiantomato" on the vscode marketplace.

## Using the Custom Tomat0 Settings (Optional):
To use the custom tomat0 color theme, copy and paste the following into your 
vscode user settings json file. A dark theme for vscode is recommended with these settings. 

```json
//custom token colors for tomat0
"editor.tokenColorCustomizations": {
    "textMateRules": [
        {
            "scope": "keyword.control.tomat0",
            "settings": {
                "foreground": "#ff7272"
            }
        },
        {
            "scope": "string.quoted.double.tomat0",
            "settings": {
                "foreground": "#a8ff78"
            }
        },
        {
            "scope": "constant.numeric.tomat0",
            "settings": {
                "foreground": "#e2ee9b"
            }
        },
        {
            "scope": "comment.line.tomat0",
            "settings": {
                "foreground": "#746587",
                "fontStyle": "italic"
            }
        }
    ]
},
//specific configurations for tomat0
"[tomat0]": {
    //disabled bracket pair colors
    "editor.bracketPairColorization.enabled": false
}
```