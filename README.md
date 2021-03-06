# Resque Bundle

A bundle for managing jobs with php-resque

[![Latest Stable Version](https://poser.pugx.org/mcfedr/resque-bundle/v/stable.png)](https://packagist.org/packages/mcfedr/resque-bundle)
[![License](https://poser.pugx.org/mcfedr/resque-bundle/license.png)](https://packagist.org/packages/mcfedr/resque-bundle)
[![Build Status](https://travis-ci.org/mcfedr/resque-bundle.svg?branch=master)](https://travis-ci.org/mcfedr/resque-bundle)
[![SensioLabsInsight](https://insight.sensiolabs.com/projects/22b1fb48-5b0d-4737-8022-4ac0759d5537/mini.png)](https://insight.sensiolabs.com/projects/22b1fb48-5b0d-4737-8022-4ac0759d5537)

## Requirements

You will need a Redis server

You can try something like 

    apt-get install redis-server
    
Or
    
    brew install redis

## Install

### Composer

    php composer.phar require mcfedr/resque-bundle

### AppKernel

Include the bundle in your AppKernel

    public function registerBundles()
    {
        $bundles = array(
            ...
            new Mcfedr\ResqueBundle\McfedrResqueBundle(),

### Configuration

Your configuration should be something like this

    mcfedr_resque:
        host: 127.0.0.1
        port: 6379
        default_queue: default

## Tests

    ./vendor/bin/phpunit
    
