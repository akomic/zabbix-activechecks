# zabbixactivechecks

Simple python module implementing Zabbix Agent Active checks protocol.  
Retrieves all active check items for given host.

## Install

The latest version [is available on PyPI](https://pypi.python.org/pypi/zabbixactivechecks).

With `pip`:

    pip3 install zabbixactivechecks


## Usage

```python
#!/usr/bin/env python3

''' import module '''
from zabbixactivechecks import ItemList

itemList = ItemList(host='activetest')
response = itemList.get(
    server='127.0.0.1',
    port=10051
)

print(response.data)
```
