# Usage

Add service.

    define ['angular', 'lib/aseed-service-queryparams/queryparams-service'], (angular, queryparams) ->
      'use strict'
      module = angular.module('template.services', [])
      module.value('version', '0.1')
      
      module.factory 'queryparams', ->
        return queryparams
      
      return module
