FROM node:16-slim

# RUN apk add --no-cache --virtual build-dependencies build-base

# RUN  apk --no-cache add ca-certificates wget bash gcompat

# RUN apk add --update python3 make g++\
#    && rm -rf /var/cache/apk/*  

WORKDIR /app

COPY package*.json /app/
RUN npm install
# COPY . /app/

# RUN npm test

# RUN ldconfig /lib /usr/glibc-compat/lib
RUN ldd /app/node_modules/@pact-foundation/pact/node_modules/@pact-foundation/pact-core/build/Release/libpact_ffi.so