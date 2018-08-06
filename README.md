# docker-openmq

[![Build Status](https://secure.travis-ci.org/stocksoftware/docker-openmq.png?branch=master)](http://travis-ci.org/stocksoftware/docker-openmq)

A minimal docker image designed to provide a openmq message broker useful for testing.

### Usage

Example:

    docker run --name openmq -e IMQ_PORTMAPPER_PORT=7676 -e IMQ_JMS_TCP_PORT=40000 -e IMQ_ADMIN_TCP_PORT=50000 -p 7676:7676 -p 40000:40000 -p 50000:50000 -d --restart=unless-stopped crendon/openmq:latest
