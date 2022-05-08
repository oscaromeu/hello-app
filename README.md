# Hello Application example

[![CI](https://github.com/oscaromeu/hello-app/workflows/Build/badge.svg?branch=main&event=push)](https://github.com/oscaromeu/hello-app/actions?query=workflow%3Apublish) [![Docker pulls](https://img.shields.io/docker/pulls/oscaromeu/hello-app)](https://hub.docker.com/r/oscaromeu/hello-app/)

This example shows how to build and deploy a containerized Go web server
application using [Kubernetes](https://kubernetes.io).


This directory contains:

- `main.go` contains the HTTP server implementation. It responds to all HTTP
  requests with a  `Hello, world!` response.
- `Dockerfile` is used to build the Docker image for the application.

This application is available as two Docker images, which respond to requests
with different version numbers:

- `.../hello-app:1.0`
- `.../hello-app:2.0`

The original source of this repository is [google hello app](https://github.com/GoogleCloudPlatform/kubernetes-engine-samples/tree/main/hello-app)