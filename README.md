# bbparse

This library parses a PCAPng file which contains black box records, such as the
PCAPng files produced by [tcplog_dumper](https://github.com/Netflix/tcplog_dumper).

## TCP_LOG_BUFFER v6 Support
This bbparse is patched to force the version conversion from 6 to 9(If you run on FreeBSD 13). For basic TCP debugging propose, this should work fine. However its not guranteed that it will work on all scenarios.

In addition, to properly run tcplog\_dumper on FreeBSD 12.1, a kernel patch,
that adds the tcp log event enums used in dumper, is required.

## Usage example

This library is a build dependency of [read_bbrlog](https://github.com/Netflix/read_bbrlog).
