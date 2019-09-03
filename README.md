tslint
------------
 
PGS standard tslint rules.

In `tslint-angular` directory there are general rules for any angular 2+ projects. (Rxjs rules are for rxjs v.6+ so might be removed for lower versions)

In `tslint-other` directory there are general rules for any kind of projects.

In `tslint-other-with-rxjs` directory there are general rules for any kind of projects with rxjs.


Optional rules
------------
`interface-name` - forces interfaces to start with "I" prefix. It helps in some situations but it's not mandatory.

`no-string-literal` - there might be an issue with testing private methods etc.

`object-literal-sort-keys` - nice to have, but no auto fix === time consuming

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
Verify which version you need from the 3 versions available
- `tslint-angular/tslint.json`
- `tslint-other/tslint.json`
- `tslint-other-with-rxjs/tslint.json`

Update project `package.json` file with proper libraries from repo version of `package.json`

Create file `pgs-lint.json` right beside project `tslint.json` file.

Copy-paste content from repo `tslint.json` to your newly created `pgs-lint.json`

Update your project `tslint.json` as below:

    {
      "extends": "./tslint-pgs.json",
      "rules": {}
    }
    
Update `pgs-lint.json` file only when changes are pushed to official repo.

Update `tslint.json` rules to overwrite optional official rules or add unofficial additional ones.
