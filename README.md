tslint
------------
 
PGS standard tslint rules.

`tslint.json` file contains general rules for any TypeScript project.

`tslint-other-with-rxjs` file contains general rules for any TypeScript project with RxJS.

`tslint-angular.json` file contains general rules for any angular projects.


Optional rules
------------
`interface-name` - forces interfaces to start with "I" prefix. It helps in some situations but it's not mandatory.

`no-string-literal` - there might be an issue with testing private methods etc.

`object-literal-sort-keys` - nice to have, but no auto fix -> time consuming

`ter-arrow-body-style` - there might be an issue with code line length 
(moving code to new line might not be nice when it comes to aesthetic)

`trailing-comma` - can be set as the cfg below if you don't like trailing commas.

    {
      true,
      {
        "multiline": "never",
        "singleline": "never"
      }
    }
    
`naming-convention` - can be slightly adjusted per project depending on devs preferences

How to use
------------
Verify which version you need from the 3 versions available (`tslint.json`, `tslint-rxjs.json`, `tslint-angular.json`)

Update your project `tslint.json` to extend rules from previously selected file.

Update `tslint.json` rules to overwrite optional official rules or add unofficial ones if needed.
