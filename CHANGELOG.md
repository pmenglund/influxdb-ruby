# Changelog

For the full commit log, [see here](https://github.com/influxdata/influxdb-ruby/commits/master).

## v0.3.1, released 2016-05-26

- Fixed #130 (again). Integer values are now really written as Integers to InfluxDB.

## v0.3.0, released 2016-04-24

- Write queries are now checked against 204 No Content responses, in accordance with the official documentation (#128).
- Async options are now configurabe (#107).

## v0.2.6, released 2016-04-14

- Empty tag keys/values are now omitted (#124).

## v0.2.5, released 2016-04-14

- Async writer now behaves when stopping the client (#73).
- Update development dependencies and started enforcing Rubocop styles.

## v0.2.4, released 2016-04-12

- Added `InfluxDB::Client#version`, returning the server version (#117).
- Fixed escaping issues (#119, #121, #135).
- Integer values are now written as Integer, not as Float value (#131).
- Return all result series when querying multiple selects (#134).
- Made host cycling thread safe (#136).

## v0.2.3, released 2015-10-27

- Added `epoch` option to client constructor and write methods (#104).
- Added `#list_user_grants` (#111), `#grant_user_admin_privileges` (#112) and `#alter_retention_policy` (#114) methods.

## v0.2.2, released 2015-07-29

- Fixed issues with Async client (#101)
- Avoid usage of `gsub!` (#102)

## v0.2.1, released 2015-07-25

- Fix double quote tags escaping (#98)

## v0.2.0, released 2015-07-20

- Large library refactoring (#88, #90)
  - Extract config from client
  - Extract HTTP functionality to separate module
  - Extract InfluxDB management functions to separate modules
  - Add writer concept
  - Refactor specs (add cases)
  - Add 'denormalize' option to config
  - Recognize SeriesNotFound error
  - Update README
  - Add Rubocop config
  - Break support for Ruby < 2
- Added support for InfluxDB 0.9+ (#92)

## v0.1.9, released 2015-07-04

- last version to support InfluxDB 0.8.x
