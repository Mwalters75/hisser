# meower.py
Python library for interacting with the Meower API
## Commands
- `meower.repair_mode()` - Checks if the server is in repair mode
- `meower.scratch_deprecated()` - Checks if Scratch clients are now deprecated
- `meower.find_post(num)` - Downloads home, then finds the post number
- `meower.get_home()` - Downloads home, in JSON format
- `meower.home_len()` - Shows the number of posts on home
- `meower.get_post(str)` - Gets the specified post, and shows in `username: post` format
- `meower.page_len()` - Shows the number of home pages
- `meower.current_page()` - Returns the current page number
- `meower.change_page(num)` - Changes the page
- `meower.ping()` - "Pings" the Meower API, by timing `requests` to fetch the root page 
- `meower.argo_tunnel()` - Checks if there is a Argo Tunnel error on the API
## Installing
`meower.py` is now on [PyPI](https://pypi.org/project/meower/) (Python Package Index)! That means that you can use `pip3`, or `pip` to install it, now!
```
pip3 install meower
```
## Usage
To import, just simply use the following:
```python
import meower
```
## Building
Before you build, you'd might want to double-check that you have all of the dependencies:
```
pip3 install -r requirements.txt
```
Run the `build` command:
```
python3 -m build
```
## Upgrading
`meower.py` is a ongoing project, so you'd might want to check for updates regularly. You can update the package like this:
```
pip3 install --upgrade meower
```
## Demo Client
```python
import meower

for i in range(0, meower.home_len()):
	print(meower.get_post(meower.find_post(i)))
```
## Licence
### `meower.py`
`meower.py` is licenced under the MEOW Licence, meaning that you can do the following to the source code:
```
* You are free to change, remove, or modify the above copyright notice.
* You are free to use the software in private or commercial forms.
* You are free to use, copy, modify, and/or distribute the software for any purpose.
* You are free to distribute this software with or without fee.
* Absolutely no patent use is permitted.
```
### Demo Client
The demo client is licenced under the Unlicence licence, meaning that you can do the following to the source code:
```
* Lorem ispum dolor sit amet
```
