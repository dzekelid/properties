swagger: "2.0"
x-collection-name: Steem
x-complete: 1
info:
  title: Interactive Steem API
  description: interactive-steem-api-lets-you-interact-with-steem-blockchain-and-make-a-request-get-output-and-start-implementing-new-apps-apis-have-default-parameters-set-to-get-you-started-and-see-how-request-works--api-list-is-compiled-from-steem-githubhttpsgithub-comsteemitsteem-1httpsgithub-comsteemitsteemtreemasterlibrariesappincludesteemitappapi-hpp-and-2httpsgithub-comsteemitsteemtreemasterlibrariesappincludesteemitappdatabase-api-hpp--if-you-want-to-contribute-documenting-detail-of-properties-and-output-contact-goodkarmahttpssteemit-chatdirectgoodkarma--you-can-also-check-full-list-here-steem-jshttpssteemjs-com
  version: 1.0.0
host: api.steemjs.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /get_chain_properties:
    get:
      summary: get chain properties
      description: get chain properties
      operationId: get-chain-properties
      x-api-path-slug: get-chain-properties-get
      responses:
        200:
          description: OK
      tags:
      - Get
      - Chain
      - Properties
  /get_dynamic_global_properties:
    get:
      summary: get_dynamic_global_properties
      description: get_dynamic_global_properties
      operationId: get-dynamic-global-properties
      x-api-path-slug: get-dynamic-global-properties-get
      responses:
        200:
          description: OK
      tags:
      - Get
      - Dynamic
      - Global
      - Properties