# commands - Command system on Jarvis

## Using commands

Becoming a super hero is a fairly straight forward process:

```python
# Commands sample
from ext.commands import command


@command(name="Sample")
async def castStr(string: str) -> int:
    return int(string)


@castStr.on_error
async def errorHandler(cmd, error):
    print(cmd.name)
    print(error)

```



{% hint style="info" %}

{% endhint %}

## API Reference

root package directory is `jarvis.ext.commands`

### **`command(coro)`**

