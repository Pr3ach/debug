## Presentation
Small python2/3 library that helps printing/writing debug messages.\
Here is the set of available methods of the main `Debug()` class.

```python
def info(msg):
def debug(msg):
def warning(msg):
def error(msg):
def critical(msg):
```

## Usage

```python
import debug

dbg = debug.Debug("MyApp")

dbg.info("Process started")
dbg.error("Specified file not found")
```
The above example creates a log file `MyApp_1559916329.log` with the following content:
```
2019/06/07 16:05:54 INFO     Process started
2019/06/07 16:06:03 ERROR    Specified file not found
```
If no parameter or empty string is provided to the constructor, stdout is used.
