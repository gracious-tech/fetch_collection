# Official fetch(bible) collection

These are the source files for the [official collection](https://v1.fetch.bible) of Bible translations for the [fetch(bible) platform](https://fetch.bible).

A fetch(bible) collection has a `sources` dir (original formats) and a `dist` dir (conversions to various formats). This repository only represents the `sources` dir, as the `dist` dir is too large to host on Github. But all the `dist` files can be generated from the files in `sources`.

To get all the `dist` files you can either generate them yourself using the [collector CLI](https://fetch.bible/access/collections/) or you can download them from the S3 bucket using the AWS CLI. You don't need an access key to do this:

`aws s3 sync --no-sign-request s3://fetch-collection-v1 <local dir>`

You can browse individual `dist` files at https://v1.fetch.bible
