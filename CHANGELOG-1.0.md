CHANGELOG
=========

This changelog references the relevant changes done in minor version updates.

1.0.0 (2016-03-18)
------------------

All issues and pull requests under this release may be found under the
[1.0.0](https://github.com/alcaeus/mongo-php-adapter/issues?q=milestone%3A1.0.0)
milestone.

 * [#74](https://github.com/alcaeus/mongo-php-adapter/pull/74) fixes running an
 aggregation command and returning a result document instead of a result cursor.
 This bug was fixed in the underlying mongo-php-library.
 * [#71](https://github.com/alcaeus/mongo-php-adapter/pull/71) adds checks to
 all class files to prevent class declarations when `ext-mongo` is already
 loaded and not using an autoloader.
 * [#72](https://github.com/alcaeus/mongo-php-adapter/pull/72) fixes wrong
 argument order in the constructor for the `Timestamp` type.
 * [#75](https://github.com/alcaeus/mongo-php-adapter/pull/75) adds a warning to
 `MongoCursor::timeout` to let people now cursor timeouts are no longer supported.
 * [#77](https://github.com/alcaeus/mongo-php-adapter/pull/77) adds support for
 the `update` option in `findAndModify` calls.

1.0.0-BETA1 (2016-02-17)
------------------------

All issues and pull requests under this release may be found under the
[1.0.0-BETA1](https://github.com/alcaeus/mongo-php-adapter/issues?q=milestone%3A1.0.0-BETA1)
milestone.

 * [#52](https://github.com/alcaeus/mongo-php-adapter/pull/52) fixes behavior of
 `MongoCollection::update` when no update operators have been given.
 * [#53](https://github.com/alcaeus/mongo-php-adapter/pull/53) fixes an error
 where some operations would send an invalid query to the MongoDB server,
 causing command failures.
 * [#54](https://github.com/alcaeus/mongo-php-adapter/pull/54) and
 [#55](https://github.com/alcaeus/mongo-php-adapter/pull/55) fix the handling of
 documents with numeric keys.
 * [#56](https://github.com/alcaeus/mongo-php-adapter/pull/56) fixes the
 behavior of `MongoGridFS::findOne` when no results are found.
 * [#59](https://github.com/alcaeus/mongo-php-adapter/pull/59) adds handling for
 the `includeSystemCollections` parameter in `MongoDB::getCollectionInfo` and
 `MongoDB::getCollectionNames`.
 * [#62](https://github.com/alcaeus/mongo-php-adapter/pull/62) removes the
 manual comparison of index options to rely on the MongoDB server to decide
 whether an index already exists.
 * [#63](https://github.com/alcaeus/mongo-php-adapter/pull/63) prevents
 serialization of driver classes which are not serializable.

0.1.0 (2016-02-06)
------------------

Initial development release.