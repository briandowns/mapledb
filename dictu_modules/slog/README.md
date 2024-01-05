# slog

A structured logger for Dictu.

## Examples

Import the module

```cs
from "slog.du" import Log;
```

Create the logger. If no args given to the class initiaizer, output is written to STDOUT. A file path can be provided and written to.

```cs
const logger = Log();
```

Write an info level line

```cs
logger.info("Starting app");
```

```json
{"msg": "Starting app", "timestamp": 1702879940, "level": "info"}
```

## Contributions

* File Issue with details of the problem, feature request, etc.
* Submit a pull request and include details of what problem or feature the code is solving or implementing.
