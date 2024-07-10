# LanguageBack
Data relating to native languages, intended for native linguists

## File Naming Conventions

```
<informant>_<linguist>_<year-of-publication>.json
```

## Data File Format
The overall format for the file is:

```
{
  "name":"...",
  "comments":"...",
  "authors":"lastname, firstname; lastname, firstname",
  "yearOfPublication":"....",
  "audienceLanguage":"...",
  "subjectLanguages":{
    "abbreviation":"full name of language",
    "abbreviation":"full name of language",
    ...
    "abbreviation":"full name of language"
  },
  "texts":[
  ]
}
```

The format for an interlinear text is:

```
{
  "type":"interlinear_v1",
  "name":"...",
  "comments":"...",
  "layers":[
    <layer-name>,
    <layer-name>,
    <layer-name>
  ],
  "elements":[
  ]
}
```

Interlinear elements take the following form:

```
{"pg":<new-page-number>}
{"ln":<new-line-number>}
{"i":[<layer-value>,<layer-value>,<layer-value>]}
```
