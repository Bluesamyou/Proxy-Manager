# **Proxy Manager V1.0**

![enter image description here](https://lh3.googleusercontent.com/_yjXu_pVZgAFpFeJbcvaya5PjwNvtJHniX8clmIlKtYhROVB_I0sGrJjBkUWQLQWaTI7aljdhVG0VQ)

**Credit to Alex Gompper (@alxgmpr) for creating the initial code in his Shopify Bot (https://github.com/alxgmpr/Shopify2Open)**

Proxy manager for python request sessions. Allows users to easily add proxies to sessions without the need to re-code logic for proxy management and use

## Usage

- Install required module `pip install termcolor`

- Import into code using `from proxymanager import ProxyManager`

- Make call to method to get next proxy `proxy = ProxyManager().get_next_proxy()`

- assign proxy to session (`request.Session().proxies = proxy`)

|Params|Use | Values |
|--|--|--|
| Random Proxy |Set to `True` to randomly pick a proxy from the list| Boolean |
| Index  |Pass in a line number to recieve a specific proxy from the list | Integer |

## Features

- [x] Preformatting proxys for use with requests

- [x] Handling of unsupported formats

- [ ] Handling server assigned proxies (e.g Copped regional proxies)

- [ ] IP auth proxies
