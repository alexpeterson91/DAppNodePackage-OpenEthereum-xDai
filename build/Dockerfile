ARG UPSTREAM_VERSION

FROM nethermind/nethermind:${UPSTREAM_VERSION}

ENTRYPOINT [ "sh", "-c", "exec openethereum --chain xdai --jsonrpc-port 8545 --jsonrpc-interface all --jsonrpc-hosts all --jsonrpc-cors all --ws-interface 0.0.0.0 --ws-port 8546 --ws-hosts all --ws-max-connections 1000 --metrics --metrics-interface=all ${EXTRA_OPTS}"]
