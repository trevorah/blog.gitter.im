---
layout: post
title: 'One Shot London: What you missed'
date: '2014-07-20 20:11:36'
---

troupeSet:PRIMARY> use gitter
switched to db gitter
troupeSet:PRIMARY> db.troupes.findOne({uri: 'gitterHQ/gitter'})
{
  "_id" : ObjectId("52a5c50d240dde3715db6260"),
  "__v" : 88,
  "_nonce" : 97489,
  "_tv" : 137,
  "bans" : [
    {
      "_id" : ObjectId("53849305137985eb2bd09c73"),
      "bannedBy" : ObjectId("52939da9240dde3715db3ec9"),
      "userId" : ObjectId("52a5c1ff240dde3715db6240"),
      "dateBanned" : ISODate("2014-05-27T13:28:37.246Z")
    },
    {
      "_id" : ObjectId("53849a749994c32263b94456"),
      "bannedBy" : ObjectId("52939838240dde3715db3e98"),
      "userId" : ObjectId("52d52158240dde3715db7bb7"),
      "dateBanned" : ISODate("2014-05-27T14:00:20.435Z")
    },
    {
      "_id" : ObjectId("53849f34e0ffcd56100316e4"),
      "bannedBy" : ObjectId("52939838240dde3715db3e98"),
      "userId" : ObjectId("52d51c13240dde3715db7b95"),
      "dateBanned" : ISODate("2014-05-27T14:20:36.893Z")
    },
    {
      "_id" : ObjectId("53849f3de0ffcd56100316e6"),
      "bannedBy" : ObjectId("52939838240dde3715db3e98"),
      "userId" : ObjectId("52d51c2b240dde3715db7b97"),
      "dateBanned" : ISODate("2014-05-27T14:20:45.588Z")
    },
    {
      "_id" : ObjectId("5385b8d9e9e8c6e829ea8572"),
      "bannedBy" : ObjectId("52939838240dde3715db3e98"),
      "userId" : ObjectId("529f0a49240dde3715db5a34"),
      "dateBanned" : ISODate("2014-05-28T10:22:17.110Z")
    }
  ],
  "dateLastSecurityCheck" : ISODate("2014-04-08T16:01:46.130Z"),
  "githubType" : "REPO",
  "lcUri" : "gitterhq/gitter",
  "security" : "PUBLIC",
  "topic" : "internal chat about Gitter code",
  "uri" : "gitterHQ/gitter",
  "users" : [
    {
      "_id" : ObjectId("53906c18b5d421d26b6b51a4"),
      "userId" : ObjectId("538e22a60fc77353691c65e8"),
      "lurk" : true
    },
    {
      "_id" : ObjectId("539f1a5b2d8397146354654c"),
      "userId" : ObjectId("538e1f5b0fc77353691c65e5"),
      "lurk" : true
    },
    {
      "_id" : ObjectId("53b3ed3d8eb74ec00cac64e2"),
      "userId" : ObjectId("53a01e4b0fc77353691c84fc")
    },
    {
      "_id" : ObjectId("53cfd78b0faf698d13b9f436"),
      "userId" : ObjectId("53ce9bed08bff487a487f277")
    },
    {
      "_id" : ObjectId("53f227dba467fd4709da0650"),
      "userId" : ObjectId("538f04610fc77353691c66b4")
    },
    {
      "_id" : ObjectId("53f22868a467fd4709da065c"),
      "userId" : ObjectId("538e01dd56ae71556e907e20")
    },
    {
      "_id" : ObjectId("5409ecd0bbaf5440565b64d7"),
      "userId" : ObjectId("5409ecc6f041918da300a488"),
      "lurk" : true
    },
    {
      "_id" : ObjectId("542be86efa485ebd5bb2d210"),
      "userId" : ObjectId("542be78f37820e5fe6f3c3b6")
    },
    {
      "_id" : ObjectId("54327327492e690d1bbd195b"),
      "userId" : ObjectId("542d86fa37820e5fe6f3e34e")
    },
    {
      "_id" : ObjectId("54342341a4e9f75a756f74dd"),
      "userId" : ObjectId("54342266b08a3197a1b334df")
    }
  ],
  "tags" : [
    "internal",
    "chat",
    "gitter",
    "code",
    "discuss",
    "file"
  ],
  "userCount" : 10
}


use local

db.oplog.rs.find({op: 'd', 'o._id': ObjectId("538e1f5b0fc77353691c65e5")}).pretty()
{
  "ts" : Timestamp(1412681319, 592),
  "h" : NumberLong("275502729493949725"),
  "v" : 2,
  "op" : "d",
  "ns" : "gitter.users",
  "b" : true,
  "o" : {
    "_id" : ObjectId("538e1f5b0fc77353691c65e5")
  }
}

db.oplog.rs.find({op: 'd', 'o._id': ObjectId("53a01e4b0fc77353691c84fc")}).pretty()
{
  "ts" : Timestamp(1412681319, 4974),
  "h" : NumberLong("4309553771536506940"),
  "v" : 2,
  "op" : "d",
  "ns" : "gitter.users",
  "b" : true,
  "o" : {
    "_id" : ObjectId("53a01e4b0fc77353691c84fc")
  }
}
