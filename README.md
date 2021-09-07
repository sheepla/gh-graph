<div align="right">
    <img src="https://img.shields.io/static/v1?label=Language&message=shell&color=blue&style=flat-square"/>
    <img src="https://img.shields.io/static/v1?label=License&message=MIT&color=blue&style=flat-square"/>
</div>


# 🟩 gh-graph

**gh-graph** is a wrapper command for [kawarimidoll/deno-github-contributions-api](https://github.com/kawarimidoll/deno-github-contributions-api).

Let's draw contribution graph on your terminal! 🌳

## Screenshot

<img src="./screenshot.png"/>

## Demo on asciinema.org

> [gh-graph-cli - asciinema.org](https://asciinema.org/a/432861)

## Usage

```
gh-graph -- a github-contribution-api wrapper command

USAGE
    gh-graph MODE USERNAME [PARAMS...]
    gh-graph --help|--version

    * MODE: output mode
        t, term   print data as a colored pixels graph
        j, json   print data as a JSON
        x, text   print data as a table-styled text
        s, svg    print data as a SVG image
    * USERNAME: username on GitHub
    * PARAMS: 
        parameters for the API 
        syntax is
            name1=value1 name2=value2 ...
        to know parameters, run
            curl https://github-contributions-api.deno.dev/{{USERNAME}}

EXAMPLES
    gh-graph term sheepla scheme=pink
    gh-graph json sheepla flat=true

THANKS
    This tool utilises this API. Thanks!
    https://github.com/kawarimidoll/deno-github-contributions-api
```

## Install as an Command

Requires `curl`

Just download and add executable permission

```bash
curl -O https://raw.githubusercontent.com/sheepla/gh-graph/master/gh-graph && chmod +x gh-graph
```

## Install as an Extension for GitHub CLI

Requires `curl` and GitHub CLI v2.0.0+

> [cli/cli - GitHub](https://github.com/cli/cli)

```bash
gh extension install sheepla/gh-graph
```

## Thanks

This command utilises this API. Thanks!✨

>  [kawarimidoll/deno-github-contributions-api](https://github.com/kawarimidoll/deno-github-contributions-api)

## Development

Issue and PR is welcome!
