## `nordselect-bash`
A `bash` script to select a NordVPN server with the lowest load. 

Intended as a lightweight (i.e. `cargo`-less) alternative to [nordselect](https://github.com/editicalu/nordselect). It also tries to embed filters in the NordVPN API request, so that we're not downloading the whole list of servers. As a result, this script is noticeably faster compared to `nordselect`.

Runtime dependencies: `bash`, `curl`, `jq`

Notable missing features:
- Pinging servers to determine the one with the lowest latency (won't add)
