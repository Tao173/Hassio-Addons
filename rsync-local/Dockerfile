ARG BUILD_FROM
FROM $BUILD_FROM AS RUNNING

RUN apk update && \
    apk add --no-cache \
		'rsync=3.1.3-r3' \
		'coreutils=8.32-r0'

COPY run.sh /
RUN chmod a+x /run.sh
ENTRYPOINT [ "/run.sh" ]

