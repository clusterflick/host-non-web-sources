# host-non-web-sources

> **[Clusterflick](https://clusterflick.com)** is a free, open-source site
> listing every film showing in London, from 450+ venues in one search.
>
> This repository holds hand-transcribed listings for venues with nothing on the
> web to read. See the
> [Clusterflick organisation](https://github.com/clusterflick) for how the
> pieces fit together.

Some venues publish their programme as an annual PDF poster or a monthly email
to subscribers, and some small festivals run only a night or two a year. Their
listings are typed up here, and the
[scripts](https://github.com/clusterflick/scripts) pipeline fetches them from
this repository like any other source.

- **One file per venue**, named after the venue's id in `scripts` (or, for a
  venue whose listings arrive by email, the address they are sent to).
- **`festivals.json`** holds the programmes of small festivals. It is validated
  on retrieve, so a typo fails the pipeline rather than reaching the site.
