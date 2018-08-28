swagger: "2.0"
x-collection-name: ChainGenie
x-complete: 1
info:
  title: ChainGenie = DLT + Blockchain + Magic
  description: chaingenie-is-here-to-help-companies-enjoy-the-benefits-of-blockchain-technology-distributed-tamper-proof-record-keeping-consensus-between-distrusting-nodes-when-you-do-not-have-the-expensive-blockchain-resources-chaingenie-offers-a-hook-to-connect-your-existing-it-applications-to-popular-blockchain-networks-like-ethereum-bitcoin-blockchain-etc-with-great-ease---want-to-know-how-chaingenie-works-under-the-hood-download-our-flyer--httpchaingenie-comchaingenieflyer-pdfthe-following-is-only-teaser-documentation--for-full-information-email--a-hrefmailtomagicchaingenie-commagicchaingenie-comahrupdate-09262016-brullibanking-micro-services-addedliliapikey-is-required-for-invoking-any-micro-serviceliulemail-a-hrefmailtomagicchaingenie-commagicchaingenie-coma-for-your-sandbox-apikey-hrcoming-soon-brmagic-canvas--drag-and-drop-microservices-to-create-a-blockchain-application---iblockchain-made-easyihrwant-to-connect-with-me-on-linkedin-send-me-an-invite--a-hrefhttplinkedin-cominupriya-target-blankhttplinkedin-cominupriyaahrscript----function-i-s-o-g-r-a-m---------igoogleanalyticsobject--r-ir--ir--function--------------ir-q--ir-q---pusharguments---------ir-l--1--new-date-a--s-createelemento--m--s-getelementsbytagnameo0-a-async--1-a-src--g-m-parentnode-insertbeforea-m----window-document-script-httpswww-googleanalytics-comanalytics-js-ga----gacreate-ua825523031-auto----gasend-pageviewscript
  version: "1.0"
host: api.chaingenie.com
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /ethledger/sendcert:
    post:
      summary: Send document using hash (min fn; no return)
      description: Route the document to a recipient.  The document history and status
        is updated for querying.  The API call does not return any document properties.  This
        is a <b>minimalistic function</b> for stringing with other functions
      operationId: EthledgerSendcertPost
      x-api-path-slug: ethledgersendcert-post
      parameters:
      - in: header
        name: ApiKey
      - in: formData
        name: recipient
      - in: formData
        name: strHash
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Send
      - Document
      - Using
      - Hash
      - (min
      - Fn;
      - "No"
      - Return)
  /ethledger/sendforsign:
    post:
      summary: Send document
      description: Route the document for signature.  The document history and status
        is updated for querying.
      operationId: EthledgerSendforsignPost
      x-api-path-slug: ethledgersendforsign-post
      parameters:
      - in: header
        name: ApiKey
      - in: formData
        name: files
      - in: formData
        name: recipient
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Send
      - Document