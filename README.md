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
  "version":"1.0.0.0",
  "name":"...",
  "authors":[
    "lastname, firstname",
    "lastname, firstname"
  ],
  "yearOfPublication":"....",
  "audienceLanguage":"...",
  "subjectLanguages":{
    {
      "glottolog":<glottolog-code>,
      "iso639-1":<iso639-1>,
      "iso639-2":<iso639-2>,
      "iso639-3":<iso639-3>,
      "iso639-5":<iso639-5>,
      "endonyms":[<exonym>, <exonym>],
      "exonyms":[<exonym>, <exonym>]
    }
  },
  "texts":[
  ]
}
```

The format for an interlinear text is:

```
{
  "type":"interlinear",
  "version":"1.0.0.0",
  "name":"...",
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
{"nw":<non-interlinear-characters>}
{"wd":[<layer-value>,<layer-value>,<layer-value>]}
```
