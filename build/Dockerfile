ARG UPSTREAM_VERSION

FROM openethereum/openethereum:${UPSTREAM_VERSION}
USER root
RUN ln -s /home/openethereum/openethereum /usr/local/bin/openethereum
USER openethereum

ENTRYPOINT [ "sh", "-c", "exec openethereum --chain xdai --jsonrpc-port 8545 --jsonrpc-interface all --jsonrpc-hosts all --jsonrpc-cors all --ws-interface 0.0.0.0 --ws-port 8546 --ws-hosts all --ws-max-connections 1000 --metrics --metrics-interface=all ${EXTRA_OPTS}"]
