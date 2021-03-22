# Journalctl proxy

This app exposes your systemd logs to web via web interface.

- Serves as a proxy that reroutes new messages on journalctl to web interface.
- When you load the page all available running services are listed in dropdown.
- You can switch between them and previous logs are still being preserved.
- Once you switch to another service you will stop receiving updates from the previous one.


![Screencast](https://user-images.githubusercontent.com/296714/111937816-df564f80-8ac8-11eb-82f3-d988a720f17a.gif)

## Usage

There are two prebuild binaries available for ARM and AMD64 under [release tab](https://github.com/mitjafelicijan/journalctl-proxy/releases).

Once you unzip downloaded application you can set port on which the server is running at'

```sh
$ ./journalctl-proxy -help
Usage of ./journalctl-proxy:
  -p int
    	Server port number (default 8000)

$ ./journalctl-proxy -p 8000

```
