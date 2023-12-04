# ProtoSpaceのER図

## users テーブル##

|  column             | Type           |  options               |
|  email              |  string        |   null:false           |
|  encrypted_password |  string        |   null:false           |
|  name               |  string        |   null:false           |
|  profile            |  text          |   null:false           |
|  occupation         |  text          |   null:false           |
|  position           |  text          |   null:false           |




## commentsテーブル

|  column       |  Type        |  options                          |
|  content      |  text        |  null :false                      |
|  prototype    |  references  |  null :false  foreign_kye: true   |
|  user         |  references  |  null :false  foreign_kye: true   |

## prototypesテーブル

|  column      |  Type        |  options                           |
|  title       |  string      |  null:false                        |
|  catch_copy  |  text        |  null:false                        |
|  concept     |  text        |  null:false                        |
|  user        |  references  |  null:false   foreign_kye: true     |