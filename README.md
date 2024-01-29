# MapleDB

MapleDB is a simple key/value store module with a very simple API that can be ran in-memory or persisted to disk . 

* get(key: String) -> String
* set(key: String, value: Any, ttl: Number -> Optional) -> Nil
* del(key: String) -> Nil
* contains(key: String) -> Boolean
* keys() -> List<String>
* values() -> List
* items() -> List<List>

When setting keys with a TTL, the TTL value given should be the number of seconds this value should live for.

## Usage

```cs
from "db.du" import DB;

const db = DB();

db.set("name", "Brian Downs");
db.set("wife_name", "Jane Doe");
const name = db.get("name");

print(name); // "Brian Downs"
print(db.len()); // 2
print(db.items()); // [["name", "Brian Downs"], ["wife_name", "Jane Doe"]]
print(db.keys()); // ["name", "wife_name"]
print(db.values()); // ["Brian Downs", "Jane Doe"]
print(db.contains("name")); // true

db.close();
```

## Contributions

* File Issue with details of the problem, feature request, etc.
* Submit a pull request and include details of what problem or feature the code is solving or implementing.

## Contact

Brian Downs [@bdowns328](http://twitter.com/bdowns328)

## License

MapleDB source code is available under the Apache 2 [License](/LICENSE).

## Server

(under construction)

By default, the server persists to memory unless a db name is given at startup on the CLI.

## Client

(under construction)
