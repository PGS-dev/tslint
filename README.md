# tslint
------------
 
PGS standard tslint rules.

In `tslint-angular` directory there are general rules for any angular 2+ projects.

In `tslint-other` directory there are general rules for any kind of projects.

In `tslint-other-with-rxjs` directory there are general rules for any kind of projects with rxjs.


Optional rules
------------
`interface-name` - forces interfaces to start with "I" prefix. It helps in some situations but it's not mandatory.

`no-string-literal` - there might be an issue with testing private methods etc.

`object-literal-sort-keys` - nice to have, but no auto fix === time consuming

`ter-arrow-body-style` - there might be an issue with code line length 
(moving code to new line might not be nice when it comes to aesthetic)

`ter-padded-blocks` - can be set as [true, "never"] but it's kind of bugged 
(falsely triggers error when there is none when comments are added is specific places)

`trailing-comma` - can be set as the cfg below if you don't like trailing commas.

    {
      true,
      {
        "multiline": "never",
        "singleline": "never"
      }
    }