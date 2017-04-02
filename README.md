# api documentation for  [s3 (v4.4.0)](https://github.com/andrewrk/node-s3-client)  [![npm package](https://img.shields.io/npm/v/npmdoc-s3.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-s3) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-s3.svg)](https://travis-ci.org/npmdoc/node-npmdoc-s3)
#### high level amazon s3 client. upload and download files and directories

[![NPM](https://nodei.co/npm/s3.png?downloads=true)](https://www.npmjs.com/package/s3)

[![apidoc](https://npmdoc.github.io/node-npmdoc-s3/build/screen-capture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-s3_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-s3/build..beta..travis-ci.org/apidoc.html)

![package-listing](https://npmdoc.github.io/node-npmdoc-s3/build/screen-capture.npmPackageListing.svg)



# package.json

```json

{
    "author": {
        "name": "Andrew Kelley"
    },
    "bugs": {
        "url": "https://github.com/andrewrk/node-s3-client/issues"
    },
    "dependencies": {
        "aws-sdk": "~2.0.31",
        "fd-slicer": "~1.0.0",
        "findit2": "~2.2.3",
        "graceful-fs": "~3.0.5",
        "mime": "~1.2.11",
        "mkdirp": "~0.5.0",
        "pend": "~1.2.0",
        "rimraf": "~2.2.8",
        "streamsink": "~1.2.0"
    },
    "description": "high level amazon s3 client. upload and download files and directories",
    "devDependencies": {
        "mocha": "~2.0.1",
        "ncp": "~1.0.1"
    },
    "directories": {
        "test": "test"
    },
    "dist": {
        "shasum": "56a4f775515a7b6b9c8e5c6b1ab51f9037669f1f",
        "tarball": "https://registry.npmjs.org/s3/-/s3-4.4.0.tgz"
    },
    "engines": {
        "node": ">=0.10.20"
    },
    "gitHead": "8e9cd927cb40c121256c46bd321998bd2aa804d0",
    "homepage": "https://github.com/andrewrk/node-s3-client",
    "keywords": [
        "amazon",
        "s3",
        "sync",
        "folder",
        "directory",
        "retry",
        "limit",
        "stream",
        "async",
        "parallel",
        "multipart",
        "size"
    ],
    "license": "MIT",
    "main": "lib/index.js",
    "maintainers": [
        {
            "name": "superjoe",
            "email": "superjoe30@gmail.com"
        }
    ],
    "name": "s3",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/andrewrk/node-s3-client.git"
    },
    "scripts": {
        "test": "mocha"
    },
    "version": "4.4.0"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module s3](#apidoc.module.s3)
1.  [function <span class="apidocSignatureSpan">s3.</span>AWS.AutoScaling ()](#apidoc.element.s3.AWS.AutoScaling)
1.  [function <span class="apidocSignatureSpan">s3.</span>AWS.CloudFormation ()](#apidoc.element.s3.AWS.CloudFormation)
1.  [function <span class="apidocSignatureSpan">s3.</span>AWS.CloudFront ()](#apidoc.element.s3.AWS.CloudFront)
1.  [function <span class="apidocSignatureSpan">s3.</span>AWS.CloudSearch ()](#apidoc.element.s3.AWS.CloudSearch)
1.  [function <span class="apidocSignatureSpan">s3.</span>AWS.CloudSearchDomain ()](#apidoc.element.s3.AWS.CloudSearchDomain)
1.  [function <span class="apidocSignatureSpan">s3.</span>AWS.CloudTrail ()](#apidoc.element.s3.AWS.CloudTrail)
1.  [function <span class="apidocSignatureSpan">s3.</span>AWS.CloudWatch ()](#apidoc.element.s3.AWS.CloudWatch)
1.  [function <span class="apidocSignatureSpan">s3.</span>AWS.CloudWatchLogs ()](#apidoc.element.s3.AWS.CloudWatchLogs)
1.  [function <span class="apidocSignatureSpan">s3.</span>AWS.CodeDeploy ()](#apidoc.element.s3.AWS.CodeDeploy)
1.  [function <span class="apidocSignatureSpan">s3.</span>AWS.CognitoIdentity ()](#apidoc.element.s3.AWS.CognitoIdentity)
1.  [function <span class="apidocSignatureSpan">s3.</span>AWS.CognitoIdentityCredentials (params)](#apidoc.element.s3.AWS.CognitoIdentityCredentials)
1.  [function <span class="apidocSignatureSpan">s3.</span>AWS.CognitoSync ()](#apidoc.element.s3.AWS.CognitoSync)
1.  [function <span class="apidocSignatureSpan">s3.</span>AWS.Config (options)](#apidoc.element.s3.AWS.Config)
1.  [function <span class="apidocSignatureSpan">s3.</span>AWS.ConfigService ()](#apidoc.element.s3.AWS.ConfigService)
1.  [function <span class="apidocSignatureSpan">s3.</span>AWS.CredentialProviderChain (providers)](#apidoc.element.s3.AWS.CredentialProviderChain)
1.  [function <span class="apidocSignatureSpan">s3.</span>AWS.Credentials ()](#apidoc.element.s3.AWS.Credentials)
1.  [function <span class="apidocSignatureSpan">s3.</span>AWS.DataPipeline ()](#apidoc.element.s3.AWS.DataPipeline)
1.  [function <span class="apidocSignatureSpan">s3.</span>AWS.DirectConnect ()](#apidoc.element.s3.AWS.DirectConnect)
1.  [function <span class="apidocSignatureSpan">s3.</span>AWS.DynamoDB ()](#apidoc.element.s3.AWS.DynamoDB)
1.  [function <span class="apidocSignatureSpan">s3.</span>AWS.EC2 ()](#apidoc.element.s3.AWS.EC2)
1.  [function <span class="apidocSignatureSpan">s3.</span>AWS.EC2MetadataCredentials (options)](#apidoc.element.s3.AWS.EC2MetadataCredentials)
1.  [function <span class="apidocSignatureSpan">s3.</span>AWS.ELB ()](#apidoc.element.s3.AWS.ELB)
1.  [function <span class="apidocSignatureSpan">s3.</span>AWS.EMR ()](#apidoc.element.s3.AWS.EMR)
1.  [function <span class="apidocSignatureSpan">s3.</span>AWS.ElastiCache ()](#apidoc.element.s3.AWS.ElastiCache)
1.  [function <span class="apidocSignatureSpan">s3.</span>AWS.ElasticBeanstalk ()](#apidoc.element.s3.AWS.ElasticBeanstalk)
1.  [function <span class="apidocSignatureSpan">s3.</span>AWS.ElasticTranscoder ()](#apidoc.element.s3.AWS.ElasticTranscoder)
1.  [function <span class="apidocSignatureSpan">s3.</span>AWS.Endpoint (endpoint, config)](#apidoc.element.s3.AWS.Endpoint)
1.  [function <span class="apidocSignatureSpan">s3.</span>AWS.EnvironmentCredentials (envPrefix)](#apidoc.element.s3.AWS.EnvironmentCredentials)
1.  [function <span class="apidocSignatureSpan">s3.</span>AWS.FileSystemCredentials (filename)](#apidoc.element.s3.AWS.FileSystemCredentials)
1.  [function <span class="apidocSignatureSpan">s3.</span>AWS.Glacier ()](#apidoc.element.s3.AWS.Glacier)
1.  [function <span class="apidocSignatureSpan">s3.</span>AWS.HttpClient ()](#apidoc.element.s3.AWS.HttpClient)
1.  [function <span class="apidocSignatureSpan">s3.</span>AWS.HttpRequest (endpoint, region)](#apidoc.element.s3.AWS.HttpRequest)
1.  [function <span class="apidocSignatureSpan">s3.</span>AWS.HttpResponse ()](#apidoc.element.s3.AWS.HttpResponse)
1.  [function <span class="apidocSignatureSpan">s3.</span>AWS.IAM ()](#apidoc.element.s3.AWS.IAM)
1.  [function <span class="apidocSignatureSpan">s3.</span>AWS.ImportExport ()](#apidoc.element.s3.AWS.ImportExport)
1.  [function <span class="apidocSignatureSpan">s3.</span>AWS.KMS ()](#apidoc.element.s3.AWS.KMS)
1.  [function <span class="apidocSignatureSpan">s3.</span>AWS.Kinesis ()](#apidoc.element.s3.AWS.Kinesis)
1.  [function <span class="apidocSignatureSpan">s3.</span>AWS.Lambda ()](#apidoc.element.s3.AWS.Lambda)
1.  [function <span class="apidocSignatureSpan">s3.</span>AWS.MetadataService (options)](#apidoc.element.s3.AWS.MetadataService)
1.  [function <span class="apidocSignatureSpan">s3.</span>AWS.NodeHttpClient ()](#apidoc.element.s3.AWS.NodeHttpClient)
1.  [function <span class="apidocSignatureSpan">s3.</span>AWS.OpsWorks ()](#apidoc.element.s3.AWS.OpsWorks)
1.  [function <span class="apidocSignatureSpan">s3.</span>AWS.ParamValidator ()](#apidoc.element.s3.AWS.ParamValidator)
1.  [function <span class="apidocSignatureSpan">s3.</span>AWS.RDS ()](#apidoc.element.s3.AWS.RDS)
1.  [function <span class="apidocSignatureSpan">s3.</span>AWS.Redshift ()](#apidoc.element.s3.AWS.Redshift)
1.  [function <span class="apidocSignatureSpan">s3.</span>AWS.Request (service, operation, params)](#apidoc.element.s3.AWS.Request)
1.  [function <span class="apidocSignatureSpan">s3.</span>AWS.ResourceWaiter (service, state)](#apidoc.element.s3.AWS.ResourceWaiter)
1.  [function <span class="apidocSignatureSpan">s3.</span>AWS.Response (request)](#apidoc.element.s3.AWS.Response)
1.  [function <span class="apidocSignatureSpan">s3.</span>AWS.Route53 ()](#apidoc.element.s3.AWS.Route53)
1.  [function <span class="apidocSignatureSpan">s3.</span>AWS.Route53Domains ()](#apidoc.element.s3.AWS.Route53Domains)
1.  [function <span class="apidocSignatureSpan">s3.</span>AWS.S3 ()](#apidoc.element.s3.AWS.S3)
1.  [function <span class="apidocSignatureSpan">s3.</span>AWS.SAMLCredentials (params)](#apidoc.element.s3.AWS.SAMLCredentials)
1.  [function <span class="apidocSignatureSpan">s3.</span>AWS.SES ()](#apidoc.element.s3.AWS.SES)
1.  [function <span class="apidocSignatureSpan">s3.</span>AWS.SNS ()](#apidoc.element.s3.AWS.SNS)
1.  [function <span class="apidocSignatureSpan">s3.</span>AWS.SQS ()](#apidoc.element.s3.AWS.SQS)
1.  [function <span class="apidocSignatureSpan">s3.</span>AWS.STS ()](#apidoc.element.s3.AWS.STS)
1.  [function <span class="apidocSignatureSpan">s3.</span>AWS.SWF ()](#apidoc.element.s3.AWS.SWF)
1.  [function <span class="apidocSignatureSpan">s3.</span>AWS.SequentialExecutor ()](#apidoc.element.s3.AWS.SequentialExecutor)
1.  [function <span class="apidocSignatureSpan">s3.</span>AWS.Service (config)](#apidoc.element.s3.AWS.Service)
1.  [function <span class="apidocSignatureSpan">s3.</span>AWS.SharedIniFileCredentials (options)](#apidoc.element.s3.AWS.SharedIniFileCredentials)
1.  [function <span class="apidocSignatureSpan">s3.</span>AWS.SimpleDB ()](#apidoc.element.s3.AWS.SimpleDB)
1.  [function <span class="apidocSignatureSpan">s3.</span>AWS.StorageGateway ()](#apidoc.element.s3.AWS.StorageGateway)
1.  [function <span class="apidocSignatureSpan">s3.</span>AWS.Support ()](#apidoc.element.s3.AWS.Support)
1.  [function <span class="apidocSignatureSpan">s3.</span>AWS.TemporaryCredentials (params)](#apidoc.element.s3.AWS.TemporaryCredentials)
1.  [function <span class="apidocSignatureSpan">s3.</span>AWS.WebIdentityCredentials (params)](#apidoc.element.s3.AWS.WebIdentityCredentials)
1.  [function <span class="apidocSignatureSpan">s3.</span>Client (options)](#apidoc.element.s3.Client)
1.  [function <span class="apidocSignatureSpan">s3.</span>MultipartETag (options)](#apidoc.element.s3.MultipartETag)
1.  [function <span class="apidocSignatureSpan">s3.</span>createClient (options)](#apidoc.element.s3.createClient)
1.  [function <span class="apidocSignatureSpan">s3.</span>getPublicUrl (bucket, key, bucketLocation)](#apidoc.element.s3.getPublicUrl)
1.  [function <span class="apidocSignatureSpan">s3.</span>getPublicUrlHttp (bucket, key)](#apidoc.element.s3.getPublicUrlHttp)
1.  number <span class="apidocSignatureSpan">s3.</span>MAX_DELETE_COUNT
1.  number <span class="apidocSignatureSpan">s3.</span>MAX_MULTIPART_COUNT
1.  number <span class="apidocSignatureSpan">s3.</span>MAX_PUTOBJECT_SIZE
1.  number <span class="apidocSignatureSpan">s3.</span>MIN_MULTIPART_SIZE
1.  object <span class="apidocSignatureSpan">s3.</span>AWS
1.  object <span class="apidocSignatureSpan">s3.</span>AWS.AutoScaling.prototype
1.  object <span class="apidocSignatureSpan">s3.</span>AWS.CloudFormation.prototype
1.  object <span class="apidocSignatureSpan">s3.</span>AWS.CloudFront.prototype
1.  object <span class="apidocSignatureSpan">s3.</span>AWS.CloudSearch.prototype
1.  object <span class="apidocSignatureSpan">s3.</span>AWS.CloudSearchDomain.prototype
1.  object <span class="apidocSignatureSpan">s3.</span>AWS.CloudTrail.prototype
1.  object <span class="apidocSignatureSpan">s3.</span>AWS.CloudWatch.prototype
1.  object <span class="apidocSignatureSpan">s3.</span>AWS.CloudWatchLogs.prototype
1.  object <span class="apidocSignatureSpan">s3.</span>AWS.CodeDeploy.prototype
1.  object <span class="apidocSignatureSpan">s3.</span>AWS.CognitoIdentity.prototype
1.  object <span class="apidocSignatureSpan">s3.</span>AWS.CognitoIdentityCredentials.prototype
1.  object <span class="apidocSignatureSpan">s3.</span>AWS.CognitoSync.prototype
1.  object <span class="apidocSignatureSpan">s3.</span>AWS.Config.prototype
1.  object <span class="apidocSignatureSpan">s3.</span>AWS.Config.prototype.keys
1.  object <span class="apidocSignatureSpan">s3.</span>AWS.ConfigService.prototype
1.  object <span class="apidocSignatureSpan">s3.</span>AWS.CredentialProviderChain.prototype
1.  object <span class="apidocSignatureSpan">s3.</span>AWS.Credentials.prototype
1.  object <span class="apidocSignatureSpan">s3.</span>AWS.DataPipeline.prototype
1.  object <span class="apidocSignatureSpan">s3.</span>AWS.DirectConnect.prototype
1.  object <span class="apidocSignatureSpan">s3.</span>AWS.DynamoDB.prototype
1.  object <span class="apidocSignatureSpan">s3.</span>AWS.EC2.prototype
1.  object <span class="apidocSignatureSpan">s3.</span>AWS.EC2MetadataCredentials.prototype
1.  object <span class="apidocSignatureSpan">s3.</span>AWS.ELB.prototype
1.  object <span class="apidocSignatureSpan">s3.</span>AWS.EMR.prototype
1.  object <span class="apidocSignatureSpan">s3.</span>AWS.ElastiCache.prototype
1.  object <span class="apidocSignatureSpan">s3.</span>AWS.ElasticBeanstalk.prototype
1.  object <span class="apidocSignatureSpan">s3.</span>AWS.ElasticTranscoder.prototype
1.  object <span class="apidocSignatureSpan">s3.</span>AWS.Endpoint.prototype
1.  object <span class="apidocSignatureSpan">s3.</span>AWS.EnvironmentCredentials.prototype
1.  object <span class="apidocSignatureSpan">s3.</span>AWS.FileSystemCredentials.prototype
1.  object <span class="apidocSignatureSpan">s3.</span>AWS.Glacier.prototype
1.  object <span class="apidocSignatureSpan">s3.</span>AWS.HttpClient.prototype
1.  object <span class="apidocSignatureSpan">s3.</span>AWS.HttpRequest.prototype
1.  object <span class="apidocSignatureSpan">s3.</span>AWS.HttpResponse.prototype
1.  object <span class="apidocSignatureSpan">s3.</span>AWS.IAM.prototype
1.  object <span class="apidocSignatureSpan">s3.</span>AWS.ImportExport.prototype
1.  object <span class="apidocSignatureSpan">s3.</span>AWS.JSON
1.  object <span class="apidocSignatureSpan">s3.</span>AWS.JSON.Builder.prototype
1.  object <span class="apidocSignatureSpan">s3.</span>AWS.JSON.Parser.prototype
1.  object <span class="apidocSignatureSpan">s3.</span>AWS.KMS.prototype
1.  object <span class="apidocSignatureSpan">s3.</span>AWS.Kinesis.prototype
1.  object <span class="apidocSignatureSpan">s3.</span>AWS.Lambda.prototype
1.  object <span class="apidocSignatureSpan">s3.</span>AWS.MetadataService.prototype
1.  object <span class="apidocSignatureSpan">s3.</span>AWS.Model
1.  object <span class="apidocSignatureSpan">s3.</span>AWS.OpsWorks.prototype
1.  object <span class="apidocSignatureSpan">s3.</span>AWS.ParamValidator.prototype
1.  object <span class="apidocSignatureSpan">s3.</span>AWS.RDS.prototype
1.  object <span class="apidocSignatureSpan">s3.</span>AWS.Redshift.prototype
1.  object <span class="apidocSignatureSpan">s3.</span>AWS.Request.prototype
1.  object <span class="apidocSignatureSpan">s3.</span>AWS.ResourceWaiter.prototype
1.  object <span class="apidocSignatureSpan">s3.</span>AWS.Response.prototype
1.  object <span class="apidocSignatureSpan">s3.</span>AWS.Route53.prototype
1.  object <span class="apidocSignatureSpan">s3.</span>AWS.Route53Domains.prototype
1.  object <span class="apidocSignatureSpan">s3.</span>AWS.S3.prototype
1.  object <span class="apidocSignatureSpan">s3.</span>AWS.SAMLCredentials.prototype
1.  object <span class="apidocSignatureSpan">s3.</span>AWS.SES.prototype
1.  object <span class="apidocSignatureSpan">s3.</span>AWS.SNS.prototype
1.  object <span class="apidocSignatureSpan">s3.</span>AWS.SQS.prototype
1.  object <span class="apidocSignatureSpan">s3.</span>AWS.STS.prototype
1.  object <span class="apidocSignatureSpan">s3.</span>AWS.SWF.prototype
1.  object <span class="apidocSignatureSpan">s3.</span>AWS.SequentialExecutor.prototype
1.  object <span class="apidocSignatureSpan">s3.</span>AWS.Service.prototype
1.  object <span class="apidocSignatureSpan">s3.</span>AWS.SharedIniFileCredentials.prototype
1.  object <span class="apidocSignatureSpan">s3.</span>AWS.Signers
1.  object <span class="apidocSignatureSpan">s3.</span>AWS.Signers.Presign.prototype
1.  object <span class="apidocSignatureSpan">s3.</span>AWS.Signers.RequestSigner.prototype
1.  object <span class="apidocSignatureSpan">s3.</span>AWS.Signers.S3.prototype
1.  object <span class="apidocSignatureSpan">s3.</span>AWS.Signers.V2.prototype
1.  object <span class="apidocSignatureSpan">s3.</span>AWS.Signers.V3.prototype
1.  object <span class="apidocSignatureSpan">s3.</span>AWS.Signers.V3Https.prototype
1.  object <span class="apidocSignatureSpan">s3.</span>AWS.Signers.V4.prototype
1.  object <span class="apidocSignatureSpan">s3.</span>AWS.SimpleDB.prototype
1.  object <span class="apidocSignatureSpan">s3.</span>AWS.StorageGateway.prototype
1.  object <span class="apidocSignatureSpan">s3.</span>AWS.Support.prototype
1.  object <span class="apidocSignatureSpan">s3.</span>AWS.TemporaryCredentials.prototype
1.  object <span class="apidocSignatureSpan">s3.</span>AWS.WebIdentityCredentials.prototype
1.  object <span class="apidocSignatureSpan">s3.</span>AWS.XML
1.  object <span class="apidocSignatureSpan">s3.</span>AWS.XML.Builder.prototype
1.  object <span class="apidocSignatureSpan">s3.</span>AWS.XML.Parser.prototype
1.  object <span class="apidocSignatureSpan">s3.</span>AWS.util
1.  object <span class="apidocSignatureSpan">s3.</span>AWS.util.Buffer.prototype
1.  object <span class="apidocSignatureSpan">s3.</span>Client.prototype
1.  object <span class="apidocSignatureSpan">s3.</span>MultipartETag.prototype

#### [module s3.AWS](#apidoc.module.s3.AWS)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>AutoScaling ()](#apidoc.element.s3.AWS.AutoScaling)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>CloudFormation ()](#apidoc.element.s3.AWS.CloudFormation)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>CloudFront ()](#apidoc.element.s3.AWS.CloudFront)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>CloudSearch ()](#apidoc.element.s3.AWS.CloudSearch)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>CloudSearchDomain ()](#apidoc.element.s3.AWS.CloudSearchDomain)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>CloudTrail ()](#apidoc.element.s3.AWS.CloudTrail)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>CloudWatch ()](#apidoc.element.s3.AWS.CloudWatch)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>CloudWatchLogs ()](#apidoc.element.s3.AWS.CloudWatchLogs)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>CodeDeploy ()](#apidoc.element.s3.AWS.CodeDeploy)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>CognitoIdentity ()](#apidoc.element.s3.AWS.CognitoIdentity)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>CognitoIdentityCredentials (params)](#apidoc.element.s3.AWS.CognitoIdentityCredentials)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>CognitoSync ()](#apidoc.element.s3.AWS.CognitoSync)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>Config (options)](#apidoc.element.s3.AWS.Config)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>ConfigService ()](#apidoc.element.s3.AWS.ConfigService)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>CredentialProviderChain (providers)](#apidoc.element.s3.AWS.CredentialProviderChain)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>Credentials ()](#apidoc.element.s3.AWS.Credentials)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>DataPipeline ()](#apidoc.element.s3.AWS.DataPipeline)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>DirectConnect ()](#apidoc.element.s3.AWS.DirectConnect)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>DynamoDB ()](#apidoc.element.s3.AWS.DynamoDB)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>EC2 ()](#apidoc.element.s3.AWS.EC2)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>EC2MetadataCredentials (options)](#apidoc.element.s3.AWS.EC2MetadataCredentials)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>ELB ()](#apidoc.element.s3.AWS.ELB)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>EMR ()](#apidoc.element.s3.AWS.EMR)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>ElastiCache ()](#apidoc.element.s3.AWS.ElastiCache)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>ElasticBeanstalk ()](#apidoc.element.s3.AWS.ElasticBeanstalk)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>ElasticTranscoder ()](#apidoc.element.s3.AWS.ElasticTranscoder)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>Endpoint (endpoint, config)](#apidoc.element.s3.AWS.Endpoint)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>EnvironmentCredentials (envPrefix)](#apidoc.element.s3.AWS.EnvironmentCredentials)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>FileSystemCredentials (filename)](#apidoc.element.s3.AWS.FileSystemCredentials)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>Glacier ()](#apidoc.element.s3.AWS.Glacier)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>HttpClient ()](#apidoc.element.s3.AWS.HttpClient)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>HttpRequest (endpoint, region)](#apidoc.element.s3.AWS.HttpRequest)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>HttpResponse ()](#apidoc.element.s3.AWS.HttpResponse)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>IAM ()](#apidoc.element.s3.AWS.IAM)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>ImportExport ()](#apidoc.element.s3.AWS.ImportExport)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>KMS ()](#apidoc.element.s3.AWS.KMS)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>Kinesis ()](#apidoc.element.s3.AWS.Kinesis)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>Lambda ()](#apidoc.element.s3.AWS.Lambda)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>MetadataService (options)](#apidoc.element.s3.AWS.MetadataService)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>NodeHttpClient ()](#apidoc.element.s3.AWS.NodeHttpClient)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>OpsWorks ()](#apidoc.element.s3.AWS.OpsWorks)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>ParamValidator ()](#apidoc.element.s3.AWS.ParamValidator)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>RDS ()](#apidoc.element.s3.AWS.RDS)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>Redshift ()](#apidoc.element.s3.AWS.Redshift)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>Request (service, operation, params)](#apidoc.element.s3.AWS.Request)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>ResourceWaiter (service, state)](#apidoc.element.s3.AWS.ResourceWaiter)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>Response (request)](#apidoc.element.s3.AWS.Response)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>Route53 ()](#apidoc.element.s3.AWS.Route53)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>Route53Domains ()](#apidoc.element.s3.AWS.Route53Domains)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>S3 ()](#apidoc.element.s3.AWS.S3)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>SAMLCredentials (params)](#apidoc.element.s3.AWS.SAMLCredentials)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>SES ()](#apidoc.element.s3.AWS.SES)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>SNS ()](#apidoc.element.s3.AWS.SNS)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>SQS ()](#apidoc.element.s3.AWS.SQS)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>STS ()](#apidoc.element.s3.AWS.STS)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>SWF ()](#apidoc.element.s3.AWS.SWF)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>SequentialExecutor ()](#apidoc.element.s3.AWS.SequentialExecutor)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>Service (config)](#apidoc.element.s3.AWS.Service)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>SharedIniFileCredentials (options)](#apidoc.element.s3.AWS.SharedIniFileCredentials)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>SimpleDB ()](#apidoc.element.s3.AWS.SimpleDB)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>StorageGateway ()](#apidoc.element.s3.AWS.StorageGateway)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>Support ()](#apidoc.element.s3.AWS.Support)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>TemporaryCredentials (params)](#apidoc.element.s3.AWS.TemporaryCredentials)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>WebIdentityCredentials (params)](#apidoc.element.s3.AWS.WebIdentityCredentials)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>apiLoader (svc, version)](#apidoc.element.s3.AWS.apiLoader)
1.  object <span class="apidocSignatureSpan">s3.AWS.</span>EventListeners
1.  object <span class="apidocSignatureSpan">s3.AWS.</span>JSON
1.  object <span class="apidocSignatureSpan">s3.AWS.</span>Model
1.  object <span class="apidocSignatureSpan">s3.AWS.</span>Protocol
1.  object <span class="apidocSignatureSpan">s3.AWS.</span>Signers
1.  object <span class="apidocSignatureSpan">s3.AWS.</span>XML
1.  object <span class="apidocSignatureSpan">s3.AWS.</span>config
1.  object <span class="apidocSignatureSpan">s3.AWS.</span>events
1.  object <span class="apidocSignatureSpan">s3.AWS.</span>util
1.  string <span class="apidocSignatureSpan">s3.AWS.</span>VERSION

#### [module s3.AWS.AutoScaling](#apidoc.module.s3.AWS.AutoScaling)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>AutoScaling ()](#apidoc.element.s3.AWS.AutoScaling.AutoScaling)
1.  [function <span class="apidocSignatureSpan">s3.AWS.AutoScaling.</span>__super__ (config)](#apidoc.element.s3.AWS.AutoScaling.__super__)
1.  object <span class="apidocSignatureSpan">s3.AWS.AutoScaling.</span>apiVersions
1.  object <span class="apidocSignatureSpan">s3.AWS.AutoScaling.</span>services
1.  string <span class="apidocSignatureSpan">s3.AWS.AutoScaling.</span>serviceIdentifier

#### [module s3.AWS.AutoScaling.prototype](#apidoc.module.s3.AWS.AutoScaling.prototype)
1.  [function <span class="apidocSignatureSpan">s3.AWS.AutoScaling.prototype.</span>constructor ()](#apidoc.element.s3.AWS.AutoScaling.prototype.constructor)

#### [module s3.AWS.CloudFormation](#apidoc.module.s3.AWS.CloudFormation)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>CloudFormation ()](#apidoc.element.s3.AWS.CloudFormation.CloudFormation)
1.  [function <span class="apidocSignatureSpan">s3.AWS.CloudFormation.</span>__super__ (config)](#apidoc.element.s3.AWS.CloudFormation.__super__)
1.  object <span class="apidocSignatureSpan">s3.AWS.CloudFormation.</span>apiVersions
1.  object <span class="apidocSignatureSpan">s3.AWS.CloudFormation.</span>services
1.  string <span class="apidocSignatureSpan">s3.AWS.CloudFormation.</span>serviceIdentifier

#### [module s3.AWS.CloudFormation.prototype](#apidoc.module.s3.AWS.CloudFormation.prototype)
1.  [function <span class="apidocSignatureSpan">s3.AWS.CloudFormation.prototype.</span>constructor ()](#apidoc.element.s3.AWS.CloudFormation.prototype.constructor)

#### [module s3.AWS.CloudFront](#apidoc.module.s3.AWS.CloudFront)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>CloudFront ()](#apidoc.element.s3.AWS.CloudFront.CloudFront)
1.  [function <span class="apidocSignatureSpan">s3.AWS.CloudFront.</span>__super__ (config)](#apidoc.element.s3.AWS.CloudFront.__super__)
1.  object <span class="apidocSignatureSpan">s3.AWS.CloudFront.</span>apiVersions
1.  object <span class="apidocSignatureSpan">s3.AWS.CloudFront.</span>services
1.  string <span class="apidocSignatureSpan">s3.AWS.CloudFront.</span>serviceIdentifier

#### [module s3.AWS.CloudFront.prototype](#apidoc.module.s3.AWS.CloudFront.prototype)
1.  [function <span class="apidocSignatureSpan">s3.AWS.CloudFront.prototype.</span>constructor ()](#apidoc.element.s3.AWS.CloudFront.prototype.constructor)

#### [module s3.AWS.CloudSearch](#apidoc.module.s3.AWS.CloudSearch)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>CloudSearch ()](#apidoc.element.s3.AWS.CloudSearch.CloudSearch)
1.  [function <span class="apidocSignatureSpan">s3.AWS.CloudSearch.</span>__super__ (config)](#apidoc.element.s3.AWS.CloudSearch.__super__)
1.  object <span class="apidocSignatureSpan">s3.AWS.CloudSearch.</span>apiVersions
1.  object <span class="apidocSignatureSpan">s3.AWS.CloudSearch.</span>services
1.  string <span class="apidocSignatureSpan">s3.AWS.CloudSearch.</span>serviceIdentifier

#### [module s3.AWS.CloudSearch.prototype](#apidoc.module.s3.AWS.CloudSearch.prototype)
1.  [function <span class="apidocSignatureSpan">s3.AWS.CloudSearch.prototype.</span>constructor ()](#apidoc.element.s3.AWS.CloudSearch.prototype.constructor)

#### [module s3.AWS.CloudSearchDomain](#apidoc.module.s3.AWS.CloudSearchDomain)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>CloudSearchDomain ()](#apidoc.element.s3.AWS.CloudSearchDomain.CloudSearchDomain)
1.  [function <span class="apidocSignatureSpan">s3.AWS.CloudSearchDomain.</span>__super__ (config)](#apidoc.element.s3.AWS.CloudSearchDomain.__super__)
1.  object <span class="apidocSignatureSpan">s3.AWS.CloudSearchDomain.</span>apiVersions
1.  object <span class="apidocSignatureSpan">s3.AWS.CloudSearchDomain.</span>services
1.  string <span class="apidocSignatureSpan">s3.AWS.CloudSearchDomain.</span>serviceIdentifier

#### [module s3.AWS.CloudSearchDomain.prototype](#apidoc.module.s3.AWS.CloudSearchDomain.prototype)
1.  [function <span class="apidocSignatureSpan">s3.AWS.CloudSearchDomain.prototype.</span>constructor ()](#apidoc.element.s3.AWS.CloudSearchDomain.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">s3.AWS.CloudSearchDomain.prototype.</span>setupRequestListeners (request)](#apidoc.element.s3.AWS.CloudSearchDomain.prototype.setupRequestListeners)
1.  [function <span class="apidocSignatureSpan">s3.AWS.CloudSearchDomain.prototype.</span>updateRegion (request)](#apidoc.element.s3.AWS.CloudSearchDomain.prototype.updateRegion)
1.  [function <span class="apidocSignatureSpan">s3.AWS.CloudSearchDomain.prototype.</span>validateService ()](#apidoc.element.s3.AWS.CloudSearchDomain.prototype.validateService)

#### [module s3.AWS.CloudTrail](#apidoc.module.s3.AWS.CloudTrail)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>CloudTrail ()](#apidoc.element.s3.AWS.CloudTrail.CloudTrail)
1.  [function <span class="apidocSignatureSpan">s3.AWS.CloudTrail.</span>__super__ (config)](#apidoc.element.s3.AWS.CloudTrail.__super__)
1.  object <span class="apidocSignatureSpan">s3.AWS.CloudTrail.</span>apiVersions
1.  object <span class="apidocSignatureSpan">s3.AWS.CloudTrail.</span>services
1.  string <span class="apidocSignatureSpan">s3.AWS.CloudTrail.</span>serviceIdentifier

#### [module s3.AWS.CloudTrail.prototype](#apidoc.module.s3.AWS.CloudTrail.prototype)
1.  [function <span class="apidocSignatureSpan">s3.AWS.CloudTrail.prototype.</span>constructor ()](#apidoc.element.s3.AWS.CloudTrail.prototype.constructor)

#### [module s3.AWS.CloudWatch](#apidoc.module.s3.AWS.CloudWatch)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>CloudWatch ()](#apidoc.element.s3.AWS.CloudWatch.CloudWatch)
1.  [function <span class="apidocSignatureSpan">s3.AWS.CloudWatch.</span>__super__ (config)](#apidoc.element.s3.AWS.CloudWatch.__super__)
1.  object <span class="apidocSignatureSpan">s3.AWS.CloudWatch.</span>apiVersions
1.  object <span class="apidocSignatureSpan">s3.AWS.CloudWatch.</span>services
1.  string <span class="apidocSignatureSpan">s3.AWS.CloudWatch.</span>serviceIdentifier

#### [module s3.AWS.CloudWatch.prototype](#apidoc.module.s3.AWS.CloudWatch.prototype)
1.  [function <span class="apidocSignatureSpan">s3.AWS.CloudWatch.prototype.</span>constructor ()](#apidoc.element.s3.AWS.CloudWatch.prototype.constructor)

#### [module s3.AWS.CloudWatchLogs](#apidoc.module.s3.AWS.CloudWatchLogs)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>CloudWatchLogs ()](#apidoc.element.s3.AWS.CloudWatchLogs.CloudWatchLogs)
1.  [function <span class="apidocSignatureSpan">s3.AWS.CloudWatchLogs.</span>__super__ (config)](#apidoc.element.s3.AWS.CloudWatchLogs.__super__)
1.  object <span class="apidocSignatureSpan">s3.AWS.CloudWatchLogs.</span>apiVersions
1.  object <span class="apidocSignatureSpan">s3.AWS.CloudWatchLogs.</span>services
1.  string <span class="apidocSignatureSpan">s3.AWS.CloudWatchLogs.</span>serviceIdentifier

#### [module s3.AWS.CloudWatchLogs.prototype](#apidoc.module.s3.AWS.CloudWatchLogs.prototype)
1.  [function <span class="apidocSignatureSpan">s3.AWS.CloudWatchLogs.prototype.</span>constructor ()](#apidoc.element.s3.AWS.CloudWatchLogs.prototype.constructor)

#### [module s3.AWS.CodeDeploy](#apidoc.module.s3.AWS.CodeDeploy)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>CodeDeploy ()](#apidoc.element.s3.AWS.CodeDeploy.CodeDeploy)
1.  [function <span class="apidocSignatureSpan">s3.AWS.CodeDeploy.</span>__super__ (config)](#apidoc.element.s3.AWS.CodeDeploy.__super__)
1.  object <span class="apidocSignatureSpan">s3.AWS.CodeDeploy.</span>apiVersions
1.  object <span class="apidocSignatureSpan">s3.AWS.CodeDeploy.</span>services
1.  string <span class="apidocSignatureSpan">s3.AWS.CodeDeploy.</span>serviceIdentifier

#### [module s3.AWS.CodeDeploy.prototype](#apidoc.module.s3.AWS.CodeDeploy.prototype)
1.  [function <span class="apidocSignatureSpan">s3.AWS.CodeDeploy.prototype.</span>constructor ()](#apidoc.element.s3.AWS.CodeDeploy.prototype.constructor)

#### [module s3.AWS.CognitoIdentity](#apidoc.module.s3.AWS.CognitoIdentity)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>CognitoIdentity ()](#apidoc.element.s3.AWS.CognitoIdentity.CognitoIdentity)
1.  [function <span class="apidocSignatureSpan">s3.AWS.CognitoIdentity.</span>__super__ (config)](#apidoc.element.s3.AWS.CognitoIdentity.__super__)
1.  object <span class="apidocSignatureSpan">s3.AWS.CognitoIdentity.</span>apiVersions
1.  object <span class="apidocSignatureSpan">s3.AWS.CognitoIdentity.</span>services
1.  string <span class="apidocSignatureSpan">s3.AWS.CognitoIdentity.</span>serviceIdentifier

#### [module s3.AWS.CognitoIdentity.prototype](#apidoc.module.s3.AWS.CognitoIdentity.prototype)
1.  [function <span class="apidocSignatureSpan">s3.AWS.CognitoIdentity.prototype.</span>constructor ()](#apidoc.element.s3.AWS.CognitoIdentity.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">s3.AWS.CognitoIdentity.prototype.</span>getId (params, callback)](#apidoc.element.s3.AWS.CognitoIdentity.prototype.getId)
1.  [function <span class="apidocSignatureSpan">s3.AWS.CognitoIdentity.prototype.</span>getOpenIdToken (params, callback)](#apidoc.element.s3.AWS.CognitoIdentity.prototype.getOpenIdToken)

#### [module s3.AWS.CognitoIdentityCredentials](#apidoc.module.s3.AWS.CognitoIdentityCredentials)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>CognitoIdentityCredentials (params)](#apidoc.element.s3.AWS.CognitoIdentityCredentials.CognitoIdentityCredentials)
1.  [function <span class="apidocSignatureSpan">s3.AWS.CognitoIdentityCredentials.</span>__super__ ()](#apidoc.element.s3.AWS.CognitoIdentityCredentials.__super__)

#### [module s3.AWS.CognitoIdentityCredentials.prototype](#apidoc.module.s3.AWS.CognitoIdentityCredentials.prototype)
1.  [function <span class="apidocSignatureSpan">s3.AWS.CognitoIdentityCredentials.prototype.</span>cacheId (data)](#apidoc.element.s3.AWS.CognitoIdentityCredentials.prototype.cacheId)
1.  [function <span class="apidocSignatureSpan">s3.AWS.CognitoIdentityCredentials.prototype.</span>clearCachedId ()](#apidoc.element.s3.AWS.CognitoIdentityCredentials.prototype.clearCachedId)
1.  [function <span class="apidocSignatureSpan">s3.AWS.CognitoIdentityCredentials.prototype.</span>constructor (params)](#apidoc.element.s3.AWS.CognitoIdentityCredentials.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">s3.AWS.CognitoIdentityCredentials.prototype.</span>getId (callback)](#apidoc.element.s3.AWS.CognitoIdentityCredentials.prototype.getId)
1.  [function <span class="apidocSignatureSpan">s3.AWS.CognitoIdentityCredentials.prototype.</span>getStorage (key)](#apidoc.element.s3.AWS.CognitoIdentityCredentials.prototype.getStorage)
1.  [function <span class="apidocSignatureSpan">s3.AWS.CognitoIdentityCredentials.prototype.</span>loadCachedId ()](#apidoc.element.s3.AWS.CognitoIdentityCredentials.prototype.loadCachedId)
1.  [function <span class="apidocSignatureSpan">s3.AWS.CognitoIdentityCredentials.prototype.</span>refresh (callback)](#apidoc.element.s3.AWS.CognitoIdentityCredentials.prototype.refresh)
1.  [function <span class="apidocSignatureSpan">s3.AWS.CognitoIdentityCredentials.prototype.</span>setStorage (key, val)](#apidoc.element.s3.AWS.CognitoIdentityCredentials.prototype.setStorage)
1.  object <span class="apidocSignatureSpan">s3.AWS.CognitoIdentityCredentials.prototype.</span>localStorageKey
1.  object <span class="apidocSignatureSpan">s3.AWS.CognitoIdentityCredentials.prototype.</span>storage

#### [module s3.AWS.CognitoSync](#apidoc.module.s3.AWS.CognitoSync)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>CognitoSync ()](#apidoc.element.s3.AWS.CognitoSync.CognitoSync)
1.  [function <span class="apidocSignatureSpan">s3.AWS.CognitoSync.</span>__super__ (config)](#apidoc.element.s3.AWS.CognitoSync.__super__)
1.  object <span class="apidocSignatureSpan">s3.AWS.CognitoSync.</span>apiVersions
1.  object <span class="apidocSignatureSpan">s3.AWS.CognitoSync.</span>services
1.  string <span class="apidocSignatureSpan">s3.AWS.CognitoSync.</span>serviceIdentifier

#### [module s3.AWS.CognitoSync.prototype](#apidoc.module.s3.AWS.CognitoSync.prototype)
1.  [function <span class="apidocSignatureSpan">s3.AWS.CognitoSync.prototype.</span>constructor ()](#apidoc.element.s3.AWS.CognitoSync.prototype.constructor)

#### [module s3.AWS.Config](#apidoc.module.s3.AWS.Config)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>Config (options)](#apidoc.element.s3.AWS.Config.Config)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Config.</span>__super__ ()](#apidoc.element.s3.AWS.Config.__super__)

#### [module s3.AWS.Config.prototype](#apidoc.module.s3.AWS.Config.prototype)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Config.prototype.</span>clear ()](#apidoc.element.s3.AWS.Config.prototype.clear)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Config.prototype.</span>constructor (options)](#apidoc.element.s3.AWS.Config.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Config.prototype.</span>extractCredentials (options)](#apidoc.element.s3.AWS.Config.prototype.extractCredentials)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Config.prototype.</span>getCredentials (callback)](#apidoc.element.s3.AWS.Config.prototype.getCredentials)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Config.prototype.</span>loadFromPath (path)](#apidoc.element.s3.AWS.Config.prototype.loadFromPath)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Config.prototype.</span>set (property, value, defaultValue)](#apidoc.element.s3.AWS.Config.prototype.set)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Config.prototype.</span>update (options, allowUnknownKeys)](#apidoc.element.s3.AWS.Config.prototype.update)
1.  object <span class="apidocSignatureSpan">s3.AWS.Config.prototype.</span>keys

#### [module s3.AWS.Config.prototype.keys](#apidoc.module.s3.AWS.Config.prototype.keys)
1.  boolean <span class="apidocSignatureSpan">s3.AWS.Config.prototype.keys.</span>computeChecksums
1.  boolean <span class="apidocSignatureSpan">s3.AWS.Config.prototype.keys.</span>convertResponseTypes
1.  boolean <span class="apidocSignatureSpan">s3.AWS.Config.prototype.keys.</span>dynamoDbCrc32
1.  boolean <span class="apidocSignatureSpan">s3.AWS.Config.prototype.keys.</span>paramValidation
1.  boolean <span class="apidocSignatureSpan">s3.AWS.Config.prototype.keys.</span>s3BucketEndpoint
1.  boolean <span class="apidocSignatureSpan">s3.AWS.Config.prototype.keys.</span>s3ForcePathStyle
1.  boolean <span class="apidocSignatureSpan">s3.AWS.Config.prototype.keys.</span>sslEnabled
1.  [function <span class="apidocSignatureSpan">s3.AWS.Config.prototype.keys.</span>credentialProvider ()](#apidoc.element.s3.AWS.Config.prototype.keys.credentialProvider)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Config.prototype.keys.</span>credentials ()](#apidoc.element.s3.AWS.Config.prototype.keys.credentials)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Config.prototype.keys.</span>region ()](#apidoc.element.s3.AWS.Config.prototype.keys.region)
1.  number <span class="apidocSignatureSpan">s3.AWS.Config.prototype.keys.</span>maxRedirects
1.  number <span class="apidocSignatureSpan">s3.AWS.Config.prototype.keys.</span>systemClockOffset
1.  object <span class="apidocSignatureSpan">s3.AWS.Config.prototype.keys.</span>apiVersion
1.  object <span class="apidocSignatureSpan">s3.AWS.Config.prototype.keys.</span>apiVersions
1.  object <span class="apidocSignatureSpan">s3.AWS.Config.prototype.keys.</span>httpOptions
1.  object <span class="apidocSignatureSpan">s3.AWS.Config.prototype.keys.</span>logger
1.  object <span class="apidocSignatureSpan">s3.AWS.Config.prototype.keys.</span>signatureVersion

#### [module s3.AWS.ConfigService](#apidoc.module.s3.AWS.ConfigService)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>ConfigService ()](#apidoc.element.s3.AWS.ConfigService.ConfigService)
1.  [function <span class="apidocSignatureSpan">s3.AWS.ConfigService.</span>__super__ (config)](#apidoc.element.s3.AWS.ConfigService.__super__)
1.  object <span class="apidocSignatureSpan">s3.AWS.ConfigService.</span>apiVersions
1.  object <span class="apidocSignatureSpan">s3.AWS.ConfigService.</span>services
1.  string <span class="apidocSignatureSpan">s3.AWS.ConfigService.</span>serviceIdentifier

#### [module s3.AWS.ConfigService.prototype](#apidoc.module.s3.AWS.ConfigService.prototype)
1.  [function <span class="apidocSignatureSpan">s3.AWS.ConfigService.prototype.</span>constructor ()](#apidoc.element.s3.AWS.ConfigService.prototype.constructor)

#### [module s3.AWS.CredentialProviderChain](#apidoc.module.s3.AWS.CredentialProviderChain)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>CredentialProviderChain (providers)](#apidoc.element.s3.AWS.CredentialProviderChain.CredentialProviderChain)
1.  [function <span class="apidocSignatureSpan">s3.AWS.CredentialProviderChain.</span>__super__ ()](#apidoc.element.s3.AWS.CredentialProviderChain.__super__)
1.  object <span class="apidocSignatureSpan">s3.AWS.CredentialProviderChain.</span>defaultProviders

#### [module s3.AWS.CredentialProviderChain.prototype](#apidoc.module.s3.AWS.CredentialProviderChain.prototype)
1.  [function <span class="apidocSignatureSpan">s3.AWS.CredentialProviderChain.prototype.</span>constructor (providers)](#apidoc.element.s3.AWS.CredentialProviderChain.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">s3.AWS.CredentialProviderChain.prototype.</span>resolve (callback)](#apidoc.element.s3.AWS.CredentialProviderChain.prototype.resolve)

#### [module s3.AWS.Credentials](#apidoc.module.s3.AWS.Credentials)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>Credentials ()](#apidoc.element.s3.AWS.Credentials.Credentials)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Credentials.</span>__super__ ()](#apidoc.element.s3.AWS.Credentials.__super__)

#### [module s3.AWS.Credentials.prototype](#apidoc.module.s3.AWS.Credentials.prototype)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Credentials.prototype.</span>constructor ()](#apidoc.element.s3.AWS.Credentials.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Credentials.prototype.</span>get (callback)](#apidoc.element.s3.AWS.Credentials.prototype.get)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Credentials.prototype.</span>needsRefresh ()](#apidoc.element.s3.AWS.Credentials.prototype.needsRefresh)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Credentials.prototype.</span>refresh (callback)](#apidoc.element.s3.AWS.Credentials.prototype.refresh)
1.  number <span class="apidocSignatureSpan">s3.AWS.Credentials.prototype.</span>expiryWindow

#### [module s3.AWS.DataPipeline](#apidoc.module.s3.AWS.DataPipeline)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>DataPipeline ()](#apidoc.element.s3.AWS.DataPipeline.DataPipeline)
1.  [function <span class="apidocSignatureSpan">s3.AWS.DataPipeline.</span>__super__ (config)](#apidoc.element.s3.AWS.DataPipeline.__super__)
1.  object <span class="apidocSignatureSpan">s3.AWS.DataPipeline.</span>apiVersions
1.  object <span class="apidocSignatureSpan">s3.AWS.DataPipeline.</span>services
1.  string <span class="apidocSignatureSpan">s3.AWS.DataPipeline.</span>serviceIdentifier

#### [module s3.AWS.DataPipeline.prototype](#apidoc.module.s3.AWS.DataPipeline.prototype)
1.  [function <span class="apidocSignatureSpan">s3.AWS.DataPipeline.prototype.</span>constructor ()](#apidoc.element.s3.AWS.DataPipeline.prototype.constructor)

#### [module s3.AWS.DirectConnect](#apidoc.module.s3.AWS.DirectConnect)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>DirectConnect ()](#apidoc.element.s3.AWS.DirectConnect.DirectConnect)
1.  [function <span class="apidocSignatureSpan">s3.AWS.DirectConnect.</span>__super__ (config)](#apidoc.element.s3.AWS.DirectConnect.__super__)
1.  object <span class="apidocSignatureSpan">s3.AWS.DirectConnect.</span>apiVersions
1.  object <span class="apidocSignatureSpan">s3.AWS.DirectConnect.</span>services
1.  string <span class="apidocSignatureSpan">s3.AWS.DirectConnect.</span>serviceIdentifier

#### [module s3.AWS.DirectConnect.prototype](#apidoc.module.s3.AWS.DirectConnect.prototype)
1.  [function <span class="apidocSignatureSpan">s3.AWS.DirectConnect.prototype.</span>constructor ()](#apidoc.element.s3.AWS.DirectConnect.prototype.constructor)

#### [module s3.AWS.DynamoDB](#apidoc.module.s3.AWS.DynamoDB)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>DynamoDB ()](#apidoc.element.s3.AWS.DynamoDB.DynamoDB)
1.  [function <span class="apidocSignatureSpan">s3.AWS.DynamoDB.</span>__super__ (config)](#apidoc.element.s3.AWS.DynamoDB.__super__)
1.  object <span class="apidocSignatureSpan">s3.AWS.DynamoDB.</span>apiVersions
1.  object <span class="apidocSignatureSpan">s3.AWS.DynamoDB.</span>services
1.  string <span class="apidocSignatureSpan">s3.AWS.DynamoDB.</span>serviceIdentifier

#### [module s3.AWS.DynamoDB.prototype](#apidoc.module.s3.AWS.DynamoDB.prototype)
1.  [function <span class="apidocSignatureSpan">s3.AWS.DynamoDB.prototype.</span>checkCrc32 (resp)](#apidoc.element.s3.AWS.DynamoDB.prototype.checkCrc32)
1.  [function <span class="apidocSignatureSpan">s3.AWS.DynamoDB.prototype.</span>constructor ()](#apidoc.element.s3.AWS.DynamoDB.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">s3.AWS.DynamoDB.prototype.</span>crc32IsValid (resp)](#apidoc.element.s3.AWS.DynamoDB.prototype.crc32IsValid)
1.  [function <span class="apidocSignatureSpan">s3.AWS.DynamoDB.prototype.</span>retryDelays ()](#apidoc.element.s3.AWS.DynamoDB.prototype.retryDelays)
1.  [function <span class="apidocSignatureSpan">s3.AWS.DynamoDB.prototype.</span>setupRequestListeners (request)](#apidoc.element.s3.AWS.DynamoDB.prototype.setupRequestListeners)
1.  number <span class="apidocSignatureSpan">s3.AWS.DynamoDB.prototype.</span>defaultRetryCount

#### [module s3.AWS.EC2](#apidoc.module.s3.AWS.EC2)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>EC2 ()](#apidoc.element.s3.AWS.EC2.EC2)
1.  [function <span class="apidocSignatureSpan">s3.AWS.EC2.</span>__super__ (config)](#apidoc.element.s3.AWS.EC2.__super__)
1.  object <span class="apidocSignatureSpan">s3.AWS.EC2.</span>apiVersions
1.  object <span class="apidocSignatureSpan">s3.AWS.EC2.</span>services
1.  string <span class="apidocSignatureSpan">s3.AWS.EC2.</span>serviceIdentifier

#### [module s3.AWS.EC2.prototype](#apidoc.module.s3.AWS.EC2.prototype)
1.  [function <span class="apidocSignatureSpan">s3.AWS.EC2.prototype.</span>buildCopySnapshotPresignedUrl (req, done)](#apidoc.element.s3.AWS.EC2.prototype.buildCopySnapshotPresignedUrl)
1.  [function <span class="apidocSignatureSpan">s3.AWS.EC2.prototype.</span>constructor ()](#apidoc.element.s3.AWS.EC2.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">s3.AWS.EC2.prototype.</span>extractError (resp)](#apidoc.element.s3.AWS.EC2.prototype.extractError)
1.  [function <span class="apidocSignatureSpan">s3.AWS.EC2.prototype.</span>setupRequestListeners (request)](#apidoc.element.s3.AWS.EC2.prototype.setupRequestListeners)

#### [module s3.AWS.EC2MetadataCredentials](#apidoc.module.s3.AWS.EC2MetadataCredentials)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>EC2MetadataCredentials (options)](#apidoc.element.s3.AWS.EC2MetadataCredentials.EC2MetadataCredentials)
1.  [function <span class="apidocSignatureSpan">s3.AWS.EC2MetadataCredentials.</span>__super__ ()](#apidoc.element.s3.AWS.EC2MetadataCredentials.__super__)

#### [module s3.AWS.EC2MetadataCredentials.prototype](#apidoc.module.s3.AWS.EC2MetadataCredentials.prototype)
1.  [function <span class="apidocSignatureSpan">s3.AWS.EC2MetadataCredentials.prototype.</span>constructor (options)](#apidoc.element.s3.AWS.EC2MetadataCredentials.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">s3.AWS.EC2MetadataCredentials.prototype.</span>refresh (callback)](#apidoc.element.s3.AWS.EC2MetadataCredentials.prototype.refresh)
1.  number <span class="apidocSignatureSpan">s3.AWS.EC2MetadataCredentials.prototype.</span>defaultTimeout

#### [module s3.AWS.ELB](#apidoc.module.s3.AWS.ELB)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>ELB ()](#apidoc.element.s3.AWS.ELB.ELB)
1.  [function <span class="apidocSignatureSpan">s3.AWS.ELB.</span>__super__ (config)](#apidoc.element.s3.AWS.ELB.__super__)
1.  object <span class="apidocSignatureSpan">s3.AWS.ELB.</span>apiVersions
1.  object <span class="apidocSignatureSpan">s3.AWS.ELB.</span>services
1.  string <span class="apidocSignatureSpan">s3.AWS.ELB.</span>serviceIdentifier

#### [module s3.AWS.ELB.prototype](#apidoc.module.s3.AWS.ELB.prototype)
1.  [function <span class="apidocSignatureSpan">s3.AWS.ELB.prototype.</span>constructor ()](#apidoc.element.s3.AWS.ELB.prototype.constructor)

#### [module s3.AWS.EMR](#apidoc.module.s3.AWS.EMR)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>EMR ()](#apidoc.element.s3.AWS.EMR.EMR)
1.  [function <span class="apidocSignatureSpan">s3.AWS.EMR.</span>__super__ (config)](#apidoc.element.s3.AWS.EMR.__super__)
1.  object <span class="apidocSignatureSpan">s3.AWS.EMR.</span>apiVersions
1.  object <span class="apidocSignatureSpan">s3.AWS.EMR.</span>services
1.  string <span class="apidocSignatureSpan">s3.AWS.EMR.</span>serviceIdentifier

#### [module s3.AWS.EMR.prototype](#apidoc.module.s3.AWS.EMR.prototype)
1.  [function <span class="apidocSignatureSpan">s3.AWS.EMR.prototype.</span>constructor ()](#apidoc.element.s3.AWS.EMR.prototype.constructor)

#### [module s3.AWS.ElastiCache](#apidoc.module.s3.AWS.ElastiCache)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>ElastiCache ()](#apidoc.element.s3.AWS.ElastiCache.ElastiCache)
1.  [function <span class="apidocSignatureSpan">s3.AWS.ElastiCache.</span>__super__ (config)](#apidoc.element.s3.AWS.ElastiCache.__super__)
1.  object <span class="apidocSignatureSpan">s3.AWS.ElastiCache.</span>apiVersions
1.  object <span class="apidocSignatureSpan">s3.AWS.ElastiCache.</span>services
1.  string <span class="apidocSignatureSpan">s3.AWS.ElastiCache.</span>serviceIdentifier

#### [module s3.AWS.ElastiCache.prototype](#apidoc.module.s3.AWS.ElastiCache.prototype)
1.  [function <span class="apidocSignatureSpan">s3.AWS.ElastiCache.prototype.</span>constructor ()](#apidoc.element.s3.AWS.ElastiCache.prototype.constructor)

#### [module s3.AWS.ElasticBeanstalk](#apidoc.module.s3.AWS.ElasticBeanstalk)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>ElasticBeanstalk ()](#apidoc.element.s3.AWS.ElasticBeanstalk.ElasticBeanstalk)
1.  [function <span class="apidocSignatureSpan">s3.AWS.ElasticBeanstalk.</span>__super__ (config)](#apidoc.element.s3.AWS.ElasticBeanstalk.__super__)
1.  object <span class="apidocSignatureSpan">s3.AWS.ElasticBeanstalk.</span>apiVersions
1.  object <span class="apidocSignatureSpan">s3.AWS.ElasticBeanstalk.</span>services
1.  string <span class="apidocSignatureSpan">s3.AWS.ElasticBeanstalk.</span>serviceIdentifier

#### [module s3.AWS.ElasticBeanstalk.prototype](#apidoc.module.s3.AWS.ElasticBeanstalk.prototype)
1.  [function <span class="apidocSignatureSpan">s3.AWS.ElasticBeanstalk.prototype.</span>constructor ()](#apidoc.element.s3.AWS.ElasticBeanstalk.prototype.constructor)

#### [module s3.AWS.ElasticTranscoder](#apidoc.module.s3.AWS.ElasticTranscoder)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>ElasticTranscoder ()](#apidoc.element.s3.AWS.ElasticTranscoder.ElasticTranscoder)
1.  [function <span class="apidocSignatureSpan">s3.AWS.ElasticTranscoder.</span>__super__ (config)](#apidoc.element.s3.AWS.ElasticTranscoder.__super__)
1.  object <span class="apidocSignatureSpan">s3.AWS.ElasticTranscoder.</span>apiVersions
1.  object <span class="apidocSignatureSpan">s3.AWS.ElasticTranscoder.</span>services
1.  string <span class="apidocSignatureSpan">s3.AWS.ElasticTranscoder.</span>serviceIdentifier

#### [module s3.AWS.ElasticTranscoder.prototype](#apidoc.module.s3.AWS.ElasticTranscoder.prototype)
1.  [function <span class="apidocSignatureSpan">s3.AWS.ElasticTranscoder.prototype.</span>constructor ()](#apidoc.element.s3.AWS.ElasticTranscoder.prototype.constructor)

#### [module s3.AWS.Endpoint](#apidoc.module.s3.AWS.Endpoint)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>Endpoint (endpoint, config)](#apidoc.element.s3.AWS.Endpoint.Endpoint)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Endpoint.</span>__super__ ()](#apidoc.element.s3.AWS.Endpoint.__super__)

#### [module s3.AWS.Endpoint.prototype](#apidoc.module.s3.AWS.Endpoint.prototype)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Endpoint.prototype.</span>constructor (endpoint, config)](#apidoc.element.s3.AWS.Endpoint.prototype.constructor)

#### [module s3.AWS.EnvironmentCredentials](#apidoc.module.s3.AWS.EnvironmentCredentials)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>EnvironmentCredentials (envPrefix)](#apidoc.element.s3.AWS.EnvironmentCredentials.EnvironmentCredentials)
1.  [function <span class="apidocSignatureSpan">s3.AWS.EnvironmentCredentials.</span>__super__ ()](#apidoc.element.s3.AWS.EnvironmentCredentials.__super__)

#### [module s3.AWS.EnvironmentCredentials.prototype](#apidoc.module.s3.AWS.EnvironmentCredentials.prototype)
1.  [function <span class="apidocSignatureSpan">s3.AWS.EnvironmentCredentials.prototype.</span>constructor (envPrefix)](#apidoc.element.s3.AWS.EnvironmentCredentials.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">s3.AWS.EnvironmentCredentials.prototype.</span>refresh (callback)](#apidoc.element.s3.AWS.EnvironmentCredentials.prototype.refresh)

#### [module s3.AWS.FileSystemCredentials](#apidoc.module.s3.AWS.FileSystemCredentials)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>FileSystemCredentials (filename)](#apidoc.element.s3.AWS.FileSystemCredentials.FileSystemCredentials)
1.  [function <span class="apidocSignatureSpan">s3.AWS.FileSystemCredentials.</span>__super__ ()](#apidoc.element.s3.AWS.FileSystemCredentials.__super__)

#### [module s3.AWS.FileSystemCredentials.prototype](#apidoc.module.s3.AWS.FileSystemCredentials.prototype)
1.  [function <span class="apidocSignatureSpan">s3.AWS.FileSystemCredentials.prototype.</span>constructor (filename)](#apidoc.element.s3.AWS.FileSystemCredentials.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">s3.AWS.FileSystemCredentials.prototype.</span>refresh (callback)](#apidoc.element.s3.AWS.FileSystemCredentials.prototype.refresh)

#### [module s3.AWS.Glacier](#apidoc.module.s3.AWS.Glacier)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>Glacier ()](#apidoc.element.s3.AWS.Glacier.Glacier)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Glacier.</span>__super__ (config)](#apidoc.element.s3.AWS.Glacier.__super__)
1.  object <span class="apidocSignatureSpan">s3.AWS.Glacier.</span>apiVersions
1.  object <span class="apidocSignatureSpan">s3.AWS.Glacier.</span>services
1.  string <span class="apidocSignatureSpan">s3.AWS.Glacier.</span>serviceIdentifier

#### [module s3.AWS.Glacier.prototype](#apidoc.module.s3.AWS.Glacier.prototype)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Glacier.prototype.</span>addGlacierApiVersion (request)](#apidoc.element.s3.AWS.Glacier.prototype.addGlacierApiVersion)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Glacier.prototype.</span>addTreeHashHeaders (request)](#apidoc.element.s3.AWS.Glacier.prototype.addTreeHashHeaders)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Glacier.prototype.</span>buildHashTree (hashes)](#apidoc.element.s3.AWS.Glacier.prototype.buildHashTree)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Glacier.prototype.</span>computeChecksums (data)](#apidoc.element.s3.AWS.Glacier.prototype.computeChecksums)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Glacier.prototype.</span>constructor ()](#apidoc.element.s3.AWS.Glacier.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Glacier.prototype.</span>setupRequestListeners (request)](#apidoc.element.s3.AWS.Glacier.prototype.setupRequestListeners)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Glacier.prototype.</span>validateAccountId (request)](#apidoc.element.s3.AWS.Glacier.prototype.validateAccountId)

#### [module s3.AWS.HttpClient](#apidoc.module.s3.AWS.HttpClient)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>HttpClient ()](#apidoc.element.s3.AWS.HttpClient.HttpClient)
1.  [function <span class="apidocSignatureSpan">s3.AWS.HttpClient.</span>__super__ ()](#apidoc.element.s3.AWS.HttpClient.__super__)
1.  [function <span class="apidocSignatureSpan">s3.AWS.HttpClient.</span>getInstance ()](#apidoc.element.s3.AWS.HttpClient.getInstance)
1.  number <span class="apidocSignatureSpan">s3.AWS.HttpClient.</span>streamsApiVersion

#### [module s3.AWS.HttpClient.prototype](#apidoc.module.s3.AWS.HttpClient.prototype)
1.  [function <span class="apidocSignatureSpan">s3.AWS.HttpClient.prototype.</span>constructor ()](#apidoc.element.s3.AWS.HttpClient.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">s3.AWS.HttpClient.prototype.</span>handleRequest (httpRequest, httpOptions, callback, errCallback)](#apidoc.element.s3.AWS.HttpClient.prototype.handleRequest)
1.  [function <span class="apidocSignatureSpan">s3.AWS.HttpClient.prototype.</span>progressStream (stream, httpRequest)](#apidoc.element.s3.AWS.HttpClient.prototype.progressStream)
1.  [function <span class="apidocSignatureSpan">s3.AWS.HttpClient.prototype.</span>sslAgent ()](#apidoc.element.s3.AWS.HttpClient.prototype.sslAgent)
1.  [function <span class="apidocSignatureSpan">s3.AWS.HttpClient.prototype.</span>writeBody (stream, httpRequest)](#apidoc.element.s3.AWS.HttpClient.prototype.writeBody)
1.  object <span class="apidocSignatureSpan">s3.AWS.HttpClient.prototype.</span>emitter

#### [module s3.AWS.HttpRequest](#apidoc.module.s3.AWS.HttpRequest)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>HttpRequest (endpoint, region)](#apidoc.element.s3.AWS.HttpRequest.HttpRequest)
1.  [function <span class="apidocSignatureSpan">s3.AWS.HttpRequest.</span>__super__ ()](#apidoc.element.s3.AWS.HttpRequest.__super__)

#### [module s3.AWS.HttpRequest.prototype](#apidoc.module.s3.AWS.HttpRequest.prototype)
1.  [function <span class="apidocSignatureSpan">s3.AWS.HttpRequest.prototype.</span>constructor (endpoint, region)](#apidoc.element.s3.AWS.HttpRequest.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">s3.AWS.HttpRequest.prototype.</span>pathname ()](#apidoc.element.s3.AWS.HttpRequest.prototype.pathname)
1.  [function <span class="apidocSignatureSpan">s3.AWS.HttpRequest.prototype.</span>search ()](#apidoc.element.s3.AWS.HttpRequest.prototype.search)
1.  [function <span class="apidocSignatureSpan">s3.AWS.HttpRequest.prototype.</span>setUserAgent ()](#apidoc.element.s3.AWS.HttpRequest.prototype.setUserAgent)

#### [module s3.AWS.HttpResponse](#apidoc.module.s3.AWS.HttpResponse)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>HttpResponse ()](#apidoc.element.s3.AWS.HttpResponse.HttpResponse)
1.  [function <span class="apidocSignatureSpan">s3.AWS.HttpResponse.</span>__super__ ()](#apidoc.element.s3.AWS.HttpResponse.__super__)

#### [module s3.AWS.HttpResponse.prototype](#apidoc.module.s3.AWS.HttpResponse.prototype)
1.  [function <span class="apidocSignatureSpan">s3.AWS.HttpResponse.prototype.</span>constructor ()](#apidoc.element.s3.AWS.HttpResponse.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">s3.AWS.HttpResponse.prototype.</span>createUnbufferedStream ()](#apidoc.element.s3.AWS.HttpResponse.prototype.createUnbufferedStream)

#### [module s3.AWS.IAM](#apidoc.module.s3.AWS.IAM)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>IAM ()](#apidoc.element.s3.AWS.IAM.IAM)
1.  [function <span class="apidocSignatureSpan">s3.AWS.IAM.</span>__super__ (config)](#apidoc.element.s3.AWS.IAM.__super__)
1.  object <span class="apidocSignatureSpan">s3.AWS.IAM.</span>apiVersions
1.  object <span class="apidocSignatureSpan">s3.AWS.IAM.</span>services
1.  string <span class="apidocSignatureSpan">s3.AWS.IAM.</span>serviceIdentifier

#### [module s3.AWS.IAM.prototype](#apidoc.module.s3.AWS.IAM.prototype)
1.  [function <span class="apidocSignatureSpan">s3.AWS.IAM.prototype.</span>constructor ()](#apidoc.element.s3.AWS.IAM.prototype.constructor)

#### [module s3.AWS.ImportExport](#apidoc.module.s3.AWS.ImportExport)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>ImportExport ()](#apidoc.element.s3.AWS.ImportExport.ImportExport)
1.  [function <span class="apidocSignatureSpan">s3.AWS.ImportExport.</span>__super__ (config)](#apidoc.element.s3.AWS.ImportExport.__super__)
1.  object <span class="apidocSignatureSpan">s3.AWS.ImportExport.</span>apiVersions
1.  object <span class="apidocSignatureSpan">s3.AWS.ImportExport.</span>services
1.  string <span class="apidocSignatureSpan">s3.AWS.ImportExport.</span>serviceIdentifier

#### [module s3.AWS.ImportExport.prototype](#apidoc.module.s3.AWS.ImportExport.prototype)
1.  [function <span class="apidocSignatureSpan">s3.AWS.ImportExport.prototype.</span>constructor ()](#apidoc.element.s3.AWS.ImportExport.prototype.constructor)

#### [module s3.AWS.JSON](#apidoc.module.s3.AWS.JSON)
1.  [function <span class="apidocSignatureSpan">s3.AWS.JSON.</span>Builder ()](#apidoc.element.s3.AWS.JSON.Builder)
1.  [function <span class="apidocSignatureSpan">s3.AWS.JSON.</span>Parser ()](#apidoc.element.s3.AWS.JSON.Parser)

#### [module s3.AWS.JSON.Builder.prototype](#apidoc.module.s3.AWS.JSON.Builder.prototype)
1.  [function <span class="apidocSignatureSpan">s3.AWS.JSON.Builder.prototype.</span>build (value, shape)](#apidoc.element.s3.AWS.JSON.Builder.prototype.build)

#### [module s3.AWS.JSON.Parser.prototype](#apidoc.module.s3.AWS.JSON.Parser.prototype)
1.  [function <span class="apidocSignatureSpan">s3.AWS.JSON.Parser.prototype.</span>parse (value, shape)](#apidoc.element.s3.AWS.JSON.Parser.prototype.parse)

#### [module s3.AWS.KMS](#apidoc.module.s3.AWS.KMS)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>KMS ()](#apidoc.element.s3.AWS.KMS.KMS)
1.  [function <span class="apidocSignatureSpan">s3.AWS.KMS.</span>__super__ (config)](#apidoc.element.s3.AWS.KMS.__super__)
1.  object <span class="apidocSignatureSpan">s3.AWS.KMS.</span>apiVersions
1.  object <span class="apidocSignatureSpan">s3.AWS.KMS.</span>services
1.  string <span class="apidocSignatureSpan">s3.AWS.KMS.</span>serviceIdentifier

#### [module s3.AWS.KMS.prototype](#apidoc.module.s3.AWS.KMS.prototype)
1.  [function <span class="apidocSignatureSpan">s3.AWS.KMS.prototype.</span>constructor ()](#apidoc.element.s3.AWS.KMS.prototype.constructor)

#### [module s3.AWS.Kinesis](#apidoc.module.s3.AWS.Kinesis)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>Kinesis ()](#apidoc.element.s3.AWS.Kinesis.Kinesis)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Kinesis.</span>__super__ (config)](#apidoc.element.s3.AWS.Kinesis.__super__)
1.  object <span class="apidocSignatureSpan">s3.AWS.Kinesis.</span>apiVersions
1.  object <span class="apidocSignatureSpan">s3.AWS.Kinesis.</span>services
1.  string <span class="apidocSignatureSpan">s3.AWS.Kinesis.</span>serviceIdentifier

#### [module s3.AWS.Kinesis.prototype](#apidoc.module.s3.AWS.Kinesis.prototype)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Kinesis.prototype.</span>constructor ()](#apidoc.element.s3.AWS.Kinesis.prototype.constructor)

#### [module s3.AWS.Lambda](#apidoc.module.s3.AWS.Lambda)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>Lambda ()](#apidoc.element.s3.AWS.Lambda.Lambda)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Lambda.</span>__super__ (config)](#apidoc.element.s3.AWS.Lambda.__super__)
1.  object <span class="apidocSignatureSpan">s3.AWS.Lambda.</span>apiVersions
1.  object <span class="apidocSignatureSpan">s3.AWS.Lambda.</span>services
1.  string <span class="apidocSignatureSpan">s3.AWS.Lambda.</span>serviceIdentifier

#### [module s3.AWS.Lambda.prototype](#apidoc.module.s3.AWS.Lambda.prototype)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Lambda.prototype.</span>constructor ()](#apidoc.element.s3.AWS.Lambda.prototype.constructor)

#### [module s3.AWS.MetadataService](#apidoc.module.s3.AWS.MetadataService)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>MetadataService (options)](#apidoc.element.s3.AWS.MetadataService.MetadataService)
1.  [function <span class="apidocSignatureSpan">s3.AWS.MetadataService.</span>__super__ ()](#apidoc.element.s3.AWS.MetadataService.__super__)

#### [module s3.AWS.MetadataService.prototype](#apidoc.module.s3.AWS.MetadataService.prototype)
1.  [function <span class="apidocSignatureSpan">s3.AWS.MetadataService.prototype.</span>constructor (options)](#apidoc.element.s3.AWS.MetadataService.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">s3.AWS.MetadataService.prototype.</span>loadCredentials (callback)](#apidoc.element.s3.AWS.MetadataService.prototype.loadCredentials)
1.  [function <span class="apidocSignatureSpan">s3.AWS.MetadataService.prototype.</span>request (path, callback)](#apidoc.element.s3.AWS.MetadataService.prototype.request)
1.  object <span class="apidocSignatureSpan">s3.AWS.MetadataService.prototype.</span>httpOptions
1.  string <span class="apidocSignatureSpan">s3.AWS.MetadataService.prototype.</span>host

#### [module s3.AWS.Model](#apidoc.module.s3.AWS.Model)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Model.</span>Api (api, options)](#apidoc.element.s3.AWS.Model.Api)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Model.</span>Operation (name, operation, options)](#apidoc.element.s3.AWS.Model.Operation)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Model.</span>Paginator (name, paginator)](#apidoc.element.s3.AWS.Model.Paginator)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Model.</span>ResourceWaiter (name, waiter, options)](#apidoc.element.s3.AWS.Model.ResourceWaiter)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Model.</span>Shape (shape, options, memberName)](#apidoc.element.s3.AWS.Model.Shape)

#### [module s3.AWS.NodeHttpClient](#apidoc.module.s3.AWS.NodeHttpClient)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>NodeHttpClient ()](#apidoc.element.s3.AWS.NodeHttpClient.NodeHttpClient)
1.  [function <span class="apidocSignatureSpan">s3.AWS.NodeHttpClient.</span>__super__ ()](#apidoc.element.s3.AWS.NodeHttpClient.__super__)

#### [module s3.AWS.OpsWorks](#apidoc.module.s3.AWS.OpsWorks)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>OpsWorks ()](#apidoc.element.s3.AWS.OpsWorks.OpsWorks)
1.  [function <span class="apidocSignatureSpan">s3.AWS.OpsWorks.</span>__super__ (config)](#apidoc.element.s3.AWS.OpsWorks.__super__)
1.  object <span class="apidocSignatureSpan">s3.AWS.OpsWorks.</span>apiVersions
1.  object <span class="apidocSignatureSpan">s3.AWS.OpsWorks.</span>services
1.  string <span class="apidocSignatureSpan">s3.AWS.OpsWorks.</span>serviceIdentifier

#### [module s3.AWS.OpsWorks.prototype](#apidoc.module.s3.AWS.OpsWorks.prototype)
1.  [function <span class="apidocSignatureSpan">s3.AWS.OpsWorks.prototype.</span>constructor ()](#apidoc.element.s3.AWS.OpsWorks.prototype.constructor)

#### [module s3.AWS.ParamValidator](#apidoc.module.s3.AWS.ParamValidator)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>ParamValidator ()](#apidoc.element.s3.AWS.ParamValidator.ParamValidator)
1.  [function <span class="apidocSignatureSpan">s3.AWS.ParamValidator.</span>__super__ ()](#apidoc.element.s3.AWS.ParamValidator.__super__)

#### [module s3.AWS.ParamValidator.prototype](#apidoc.module.s3.AWS.ParamValidator.prototype)
1.  [function <span class="apidocSignatureSpan">s3.AWS.ParamValidator.prototype.</span>constructor ()](#apidoc.element.s3.AWS.ParamValidator.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">s3.AWS.ParamValidator.prototype.</span>fail (code, message)](#apidoc.element.s3.AWS.ParamValidator.prototype.fail)
1.  [function <span class="apidocSignatureSpan">s3.AWS.ParamValidator.prototype.</span>validate (shape, params, context)](#apidoc.element.s3.AWS.ParamValidator.prototype.validate)
1.  [function <span class="apidocSignatureSpan">s3.AWS.ParamValidator.prototype.</span>validateList (shape, params, context)](#apidoc.element.s3.AWS.ParamValidator.prototype.validateList)
1.  [function <span class="apidocSignatureSpan">s3.AWS.ParamValidator.prototype.</span>validateMap (shape, params, context)](#apidoc.element.s3.AWS.ParamValidator.prototype.validateMap)
1.  [function <span class="apidocSignatureSpan">s3.AWS.ParamValidator.prototype.</span>validateMember (shape, param, context)](#apidoc.element.s3.AWS.ParamValidator.prototype.validateMember)
1.  [function <span class="apidocSignatureSpan">s3.AWS.ParamValidator.prototype.</span>validateNumber (context, value)](#apidoc.element.s3.AWS.ParamValidator.prototype.validateNumber)
1.  [function <span class="apidocSignatureSpan">s3.AWS.ParamValidator.prototype.</span>validatePayload (context, value)](#apidoc.element.s3.AWS.ParamValidator.prototype.validatePayload)
1.  [function <span class="apidocSignatureSpan">s3.AWS.ParamValidator.prototype.</span>validateScalar (shape, value, context)](#apidoc.element.s3.AWS.ParamValidator.prototype.validateScalar)
1.  [function <span class="apidocSignatureSpan">s3.AWS.ParamValidator.prototype.</span>validateStructure (shape, params, context)](#apidoc.element.s3.AWS.ParamValidator.prototype.validateStructure)
1.  [function <span class="apidocSignatureSpan">s3.AWS.ParamValidator.prototype.</span>validateType (context, value, acceptedTypes, type)](#apidoc.element.s3.AWS.ParamValidator.prototype.validateType)

#### [module s3.AWS.RDS](#apidoc.module.s3.AWS.RDS)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>RDS ()](#apidoc.element.s3.AWS.RDS.RDS)
1.  [function <span class="apidocSignatureSpan">s3.AWS.RDS.</span>__super__ (config)](#apidoc.element.s3.AWS.RDS.__super__)
1.  object <span class="apidocSignatureSpan">s3.AWS.RDS.</span>apiVersions
1.  object <span class="apidocSignatureSpan">s3.AWS.RDS.</span>services
1.  string <span class="apidocSignatureSpan">s3.AWS.RDS.</span>serviceIdentifier

#### [module s3.AWS.RDS.prototype](#apidoc.module.s3.AWS.RDS.prototype)
1.  [function <span class="apidocSignatureSpan">s3.AWS.RDS.prototype.</span>constructor ()](#apidoc.element.s3.AWS.RDS.prototype.constructor)

#### [module s3.AWS.Redshift](#apidoc.module.s3.AWS.Redshift)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>Redshift ()](#apidoc.element.s3.AWS.Redshift.Redshift)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Redshift.</span>__super__ (config)](#apidoc.element.s3.AWS.Redshift.__super__)
1.  object <span class="apidocSignatureSpan">s3.AWS.Redshift.</span>apiVersions
1.  object <span class="apidocSignatureSpan">s3.AWS.Redshift.</span>services
1.  string <span class="apidocSignatureSpan">s3.AWS.Redshift.</span>serviceIdentifier

#### [module s3.AWS.Redshift.prototype](#apidoc.module.s3.AWS.Redshift.prototype)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Redshift.prototype.</span>constructor ()](#apidoc.element.s3.AWS.Redshift.prototype.constructor)

#### [module s3.AWS.Request](#apidoc.module.s3.AWS.Request)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>Request (service, operation, params)](#apidoc.element.s3.AWS.Request.Request)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Request.</span>__super__ ()](#apidoc.element.s3.AWS.Request.__super__)

#### [module s3.AWS.Request.prototype](#apidoc.module.s3.AWS.Request.prototype)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Request.prototype.</span>abort ()](#apidoc.element.s3.AWS.Request.prototype.abort)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Request.prototype.</span>addListener (eventName, listener)](#apidoc.element.s3.AWS.Request.prototype.addListener)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Request.prototype.</span>addListeners (listeners)](#apidoc.element.s3.AWS.Request.prototype.addListeners)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Request.prototype.</span>addNamedAsyncListener (name, eventName, callback)](#apidoc.element.s3.AWS.Request.prototype.addNamedAsyncListener)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Request.prototype.</span>addNamedListener (name, eventName, callback)](#apidoc.element.s3.AWS.Request.prototype.addNamedListener)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Request.prototype.</span>addNamedListeners (callback)](#apidoc.element.s3.AWS.Request.prototype.addNamedListeners)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Request.prototype.</span>build (callback)](#apidoc.element.s3.AWS.Request.prototype.build)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Request.prototype.</span>buildAsGet (request)](#apidoc.element.s3.AWS.Request.prototype.buildAsGet)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Request.prototype.</span>callListeners (listeners, args, doneCallback)](#apidoc.element.s3.AWS.Request.prototype.callListeners)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Request.prototype.</span>constructor (service, operation, params)](#apidoc.element.s3.AWS.Request.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Request.prototype.</span>createReadStream ()](#apidoc.element.s3.AWS.Request.prototype.createReadStream)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Request.prototype.</span>eachItem (callback)](#apidoc.element.s3.AWS.Request.prototype.eachItem)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Request.prototype.</span>eachPage (callback)](#apidoc.element.s3.AWS.Request.prototype.eachPage)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Request.prototype.</span>emit (eventName, eventArgs, doneCallback)](#apidoc.element.s3.AWS.Request.prototype.emit)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Request.prototype.</span>emitEvent (eventName, args, done)](#apidoc.element.s3.AWS.Request.prototype.emitEvent)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Request.prototype.</span>eventParameters (eventName)](#apidoc.element.s3.AWS.Request.prototype.eventParameters)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Request.prototype.</span>isPageable ()](#apidoc.element.s3.AWS.Request.prototype.isPageable)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Request.prototype.</span>listeners (eventName)](#apidoc.element.s3.AWS.Request.prototype.listeners)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Request.prototype.</span>on (eventName, listener)](#apidoc.element.s3.AWS.Request.prototype.on)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Request.prototype.</span>onAsync (eventName, listener)](#apidoc.element.s3.AWS.Request.prototype.onAsync)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Request.prototype.</span>presign (expires, callback)](#apidoc.element.s3.AWS.Request.prototype.presign)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Request.prototype.</span>removeAllListeners (eventName)](#apidoc.element.s3.AWS.Request.prototype.removeAllListeners)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Request.prototype.</span>removeListener (eventName, listener)](#apidoc.element.s3.AWS.Request.prototype.removeListener)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Request.prototype.</span>runTo (state, done)](#apidoc.element.s3.AWS.Request.prototype.runTo)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Request.prototype.</span>send (callback)](#apidoc.element.s3.AWS.Request.prototype.send)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Request.prototype.</span>toGet ()](#apidoc.element.s3.AWS.Request.prototype.toGet)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Request.prototype.</span>toUnauthenticated ()](#apidoc.element.s3.AWS.Request.prototype.toUnauthenticated)

#### [module s3.AWS.ResourceWaiter](#apidoc.module.s3.AWS.ResourceWaiter)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>ResourceWaiter (service, state)](#apidoc.element.s3.AWS.ResourceWaiter.ResourceWaiter)
1.  [function <span class="apidocSignatureSpan">s3.AWS.ResourceWaiter.</span>__super__ ()](#apidoc.element.s3.AWS.ResourceWaiter.__super__)

#### [module s3.AWS.ResourceWaiter.prototype](#apidoc.module.s3.AWS.ResourceWaiter.prototype)
1.  boolean <span class="apidocSignatureSpan">s3.AWS.ResourceWaiter.prototype.</span>waitDone
1.  [function <span class="apidocSignatureSpan">s3.AWS.ResourceWaiter.prototype.</span>checkError (resp)](#apidoc.element.s3.AWS.ResourceWaiter.prototype.checkError)
1.  [function <span class="apidocSignatureSpan">s3.AWS.ResourceWaiter.prototype.</span>checkSuccess (resp)](#apidoc.element.s3.AWS.ResourceWaiter.prototype.checkSuccess)
1.  [function <span class="apidocSignatureSpan">s3.AWS.ResourceWaiter.prototype.</span>constructor (service, state)](#apidoc.element.s3.AWS.ResourceWaiter.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">s3.AWS.ResourceWaiter.prototype.</span>loadWaiterConfig (state, noException)](#apidoc.element.s3.AWS.ResourceWaiter.prototype.loadWaiterConfig)
1.  [function <span class="apidocSignatureSpan">s3.AWS.ResourceWaiter.prototype.</span>setError (resp, retryable)](#apidoc.element.s3.AWS.ResourceWaiter.prototype.setError)
1.  [function <span class="apidocSignatureSpan">s3.AWS.ResourceWaiter.prototype.</span>wait (params, callback)](#apidoc.element.s3.AWS.ResourceWaiter.prototype.wait)
1.  object <span class="apidocSignatureSpan">s3.AWS.ResourceWaiter.prototype.</span>Listeners
1.  object <span class="apidocSignatureSpan">s3.AWS.ResourceWaiter.prototype.</span>config
1.  object <span class="apidocSignatureSpan">s3.AWS.ResourceWaiter.prototype.</span>expectedValue
1.  object <span class="apidocSignatureSpan">s3.AWS.ResourceWaiter.prototype.</span>service
1.  object <span class="apidocSignatureSpan">s3.AWS.ResourceWaiter.prototype.</span>state

#### [module s3.AWS.Response](#apidoc.module.s3.AWS.Response)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>Response (request)](#apidoc.element.s3.AWS.Response.Response)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Response.</span>__super__ ()](#apidoc.element.s3.AWS.Response.__super__)

#### [module s3.AWS.Response.prototype](#apidoc.module.s3.AWS.Response.prototype)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Response.prototype.</span>cacheNextPageTokens ()](#apidoc.element.s3.AWS.Response.prototype.cacheNextPageTokens)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Response.prototype.</span>constructor (request)](#apidoc.element.s3.AWS.Response.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Response.prototype.</span>hasNextPage ()](#apidoc.element.s3.AWS.Response.prototype.hasNextPage)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Response.prototype.</span>nextPage (callback)](#apidoc.element.s3.AWS.Response.prototype.nextPage)

#### [module s3.AWS.Route53](#apidoc.module.s3.AWS.Route53)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>Route53 ()](#apidoc.element.s3.AWS.Route53.Route53)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Route53.</span>__super__ (config)](#apidoc.element.s3.AWS.Route53.__super__)
1.  object <span class="apidocSignatureSpan">s3.AWS.Route53.</span>apiVersions
1.  object <span class="apidocSignatureSpan">s3.AWS.Route53.</span>services
1.  string <span class="apidocSignatureSpan">s3.AWS.Route53.</span>serviceIdentifier

#### [module s3.AWS.Route53.prototype](#apidoc.module.s3.AWS.Route53.prototype)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Route53.prototype.</span>constructor ()](#apidoc.element.s3.AWS.Route53.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Route53.prototype.</span>sanitizeUrl (request)](#apidoc.element.s3.AWS.Route53.prototype.sanitizeUrl)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Route53.prototype.</span>setupRequestListeners (request)](#apidoc.element.s3.AWS.Route53.prototype.setupRequestListeners)

#### [module s3.AWS.Route53Domains](#apidoc.module.s3.AWS.Route53Domains)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>Route53Domains ()](#apidoc.element.s3.AWS.Route53Domains.Route53Domains)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Route53Domains.</span>__super__ (config)](#apidoc.element.s3.AWS.Route53Domains.__super__)
1.  object <span class="apidocSignatureSpan">s3.AWS.Route53Domains.</span>apiVersions
1.  object <span class="apidocSignatureSpan">s3.AWS.Route53Domains.</span>services
1.  string <span class="apidocSignatureSpan">s3.AWS.Route53Domains.</span>serviceIdentifier

#### [module s3.AWS.Route53Domains.prototype](#apidoc.module.s3.AWS.Route53Domains.prototype)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Route53Domains.prototype.</span>constructor ()](#apidoc.element.s3.AWS.Route53Domains.prototype.constructor)

#### [module s3.AWS.S3](#apidoc.module.s3.AWS.S3)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>S3 ()](#apidoc.element.s3.AWS.S3.S3)
1.  [function <span class="apidocSignatureSpan">s3.AWS.S3.</span>__super__ (config)](#apidoc.element.s3.AWS.S3.__super__)
1.  object <span class="apidocSignatureSpan">s3.AWS.S3.</span>apiVersions
1.  object <span class="apidocSignatureSpan">s3.AWS.S3.</span>services
1.  string <span class="apidocSignatureSpan">s3.AWS.S3.</span>serviceIdentifier

#### [module s3.AWS.S3.prototype](#apidoc.module.s3.AWS.S3.prototype)
1.  [function <span class="apidocSignatureSpan">s3.AWS.S3.prototype.</span>addContentType (req)](#apidoc.element.s3.AWS.S3.prototype.addContentType)
1.  [function <span class="apidocSignatureSpan">s3.AWS.S3.prototype.</span>computeContentMd5 (req)](#apidoc.element.s3.AWS.S3.prototype.computeContentMd5)
1.  [function <span class="apidocSignatureSpan">s3.AWS.S3.prototype.</span>computeSha256 (req, done)](#apidoc.element.s3.AWS.S3.prototype.computeSha256)
1.  [function <span class="apidocSignatureSpan">s3.AWS.S3.prototype.</span>computeSseCustomerKeyMd5 (req)](#apidoc.element.s3.AWS.S3.prototype.computeSseCustomerKeyMd5)
1.  [function <span class="apidocSignatureSpan">s3.AWS.S3.prototype.</span>constructor ()](#apidoc.element.s3.AWS.S3.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">s3.AWS.S3.prototype.</span>createBucket (params, callback)](#apidoc.element.s3.AWS.S3.prototype.createBucket)
1.  [function <span class="apidocSignatureSpan">s3.AWS.S3.prototype.</span>dnsCompatibleBucketName (bucketName)](#apidoc.element.s3.AWS.S3.prototype.dnsCompatibleBucketName)
1.  [function <span class="apidocSignatureSpan">s3.AWS.S3.prototype.</span>extractData (resp)](#apidoc.element.s3.AWS.S3.prototype.extractData)
1.  [function <span class="apidocSignatureSpan">s3.AWS.S3.prototype.</span>extractError (resp)](#apidoc.element.s3.AWS.S3.prototype.extractError)
1.  [function <span class="apidocSignatureSpan">s3.AWS.S3.prototype.</span>getSignedUrl (operation, params, callback)](#apidoc.element.s3.AWS.S3.prototype.getSignedUrl)
1.  [function <span class="apidocSignatureSpan">s3.AWS.S3.prototype.</span>pathStyleBucketName (bucketName)](#apidoc.element.s3.AWS.S3.prototype.pathStyleBucketName)
1.  [function <span class="apidocSignatureSpan">s3.AWS.S3.prototype.</span>populateURI (req)](#apidoc.element.s3.AWS.S3.prototype.populateURI)
1.  [function <span class="apidocSignatureSpan">s3.AWS.S3.prototype.</span>prepareSignedUrl (request)](#apidoc.element.s3.AWS.S3.prototype.prepareSignedUrl)
1.  [function <span class="apidocSignatureSpan">s3.AWS.S3.prototype.</span>retryableError (error, request)](#apidoc.element.s3.AWS.S3.prototype.retryableError)
1.  [function <span class="apidocSignatureSpan">s3.AWS.S3.prototype.</span>setupRequestListeners (request)](#apidoc.element.s3.AWS.S3.prototype.setupRequestListeners)
1.  [function <span class="apidocSignatureSpan">s3.AWS.S3.prototype.</span>successfulResponse (resp)](#apidoc.element.s3.AWS.S3.prototype.successfulResponse)
1.  [function <span class="apidocSignatureSpan">s3.AWS.S3.prototype.</span>validateBucketEndpoint (req)](#apidoc.element.s3.AWS.S3.prototype.validateBucketEndpoint)
1.  [function <span class="apidocSignatureSpan">s3.AWS.S3.prototype.</span>validateScheme (req)](#apidoc.element.s3.AWS.S3.prototype.validateScheme)
1.  [function <span class="apidocSignatureSpan">s3.AWS.S3.prototype.</span>validateService ()](#apidoc.element.s3.AWS.S3.prototype.validateService)
1.  [function <span class="apidocSignatureSpan">s3.AWS.S3.prototype.</span>willComputeChecksums (req)](#apidoc.element.s3.AWS.S3.prototype.willComputeChecksums)
1.  object <span class="apidocSignatureSpan">s3.AWS.S3.prototype.</span>computableChecksumOperations

#### [module s3.AWS.SAMLCredentials](#apidoc.module.s3.AWS.SAMLCredentials)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>SAMLCredentials (params)](#apidoc.element.s3.AWS.SAMLCredentials.SAMLCredentials)
1.  [function <span class="apidocSignatureSpan">s3.AWS.SAMLCredentials.</span>__super__ ()](#apidoc.element.s3.AWS.SAMLCredentials.__super__)

#### [module s3.AWS.SAMLCredentials.prototype](#apidoc.module.s3.AWS.SAMLCredentials.prototype)
1.  [function <span class="apidocSignatureSpan">s3.AWS.SAMLCredentials.prototype.</span>constructor (params)](#apidoc.element.s3.AWS.SAMLCredentials.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">s3.AWS.SAMLCredentials.prototype.</span>refresh (callback)](#apidoc.element.s3.AWS.SAMLCredentials.prototype.refresh)

#### [module s3.AWS.SES](#apidoc.module.s3.AWS.SES)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>SES ()](#apidoc.element.s3.AWS.SES.SES)
1.  [function <span class="apidocSignatureSpan">s3.AWS.SES.</span>__super__ (config)](#apidoc.element.s3.AWS.SES.__super__)
1.  object <span class="apidocSignatureSpan">s3.AWS.SES.</span>apiVersions
1.  object <span class="apidocSignatureSpan">s3.AWS.SES.</span>services
1.  string <span class="apidocSignatureSpan">s3.AWS.SES.</span>serviceIdentifier

#### [module s3.AWS.SES.prototype](#apidoc.module.s3.AWS.SES.prototype)
1.  [function <span class="apidocSignatureSpan">s3.AWS.SES.prototype.</span>constructor ()](#apidoc.element.s3.AWS.SES.prototype.constructor)

#### [module s3.AWS.SNS](#apidoc.module.s3.AWS.SNS)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>SNS ()](#apidoc.element.s3.AWS.SNS.SNS)
1.  [function <span class="apidocSignatureSpan">s3.AWS.SNS.</span>__super__ (config)](#apidoc.element.s3.AWS.SNS.__super__)
1.  object <span class="apidocSignatureSpan">s3.AWS.SNS.</span>apiVersions
1.  object <span class="apidocSignatureSpan">s3.AWS.SNS.</span>services
1.  string <span class="apidocSignatureSpan">s3.AWS.SNS.</span>serviceIdentifier

#### [module s3.AWS.SNS.prototype](#apidoc.module.s3.AWS.SNS.prototype)
1.  [function <span class="apidocSignatureSpan">s3.AWS.SNS.prototype.</span>constructor ()](#apidoc.element.s3.AWS.SNS.prototype.constructor)

#### [module s3.AWS.SQS](#apidoc.module.s3.AWS.SQS)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>SQS ()](#apidoc.element.s3.AWS.SQS.SQS)
1.  [function <span class="apidocSignatureSpan">s3.AWS.SQS.</span>__super__ (config)](#apidoc.element.s3.AWS.SQS.__super__)
1.  object <span class="apidocSignatureSpan">s3.AWS.SQS.</span>apiVersions
1.  object <span class="apidocSignatureSpan">s3.AWS.SQS.</span>services
1.  string <span class="apidocSignatureSpan">s3.AWS.SQS.</span>serviceIdentifier

#### [module s3.AWS.SQS.prototype](#apidoc.module.s3.AWS.SQS.prototype)
1.  [function <span class="apidocSignatureSpan">s3.AWS.SQS.prototype.</span>buildEndpoint (request)](#apidoc.element.s3.AWS.SQS.prototype.buildEndpoint)
1.  [function <span class="apidocSignatureSpan">s3.AWS.SQS.prototype.</span>calculateChecksum (data)](#apidoc.element.s3.AWS.SQS.prototype.calculateChecksum)
1.  [function <span class="apidocSignatureSpan">s3.AWS.SQS.prototype.</span>constructor ()](#apidoc.element.s3.AWS.SQS.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">s3.AWS.SQS.prototype.</span>isChecksumValid (checksum, data)](#apidoc.element.s3.AWS.SQS.prototype.isChecksumValid)
1.  [function <span class="apidocSignatureSpan">s3.AWS.SQS.prototype.</span>setupRequestListeners (request)](#apidoc.element.s3.AWS.SQS.prototype.setupRequestListeners)
1.  [function <span class="apidocSignatureSpan">s3.AWS.SQS.prototype.</span>throwInvalidChecksumError (response, ids, message)](#apidoc.element.s3.AWS.SQS.prototype.throwInvalidChecksumError)
1.  [function <span class="apidocSignatureSpan">s3.AWS.SQS.prototype.</span>verifyReceiveMessageChecksum (response)](#apidoc.element.s3.AWS.SQS.prototype.verifyReceiveMessageChecksum)
1.  [function <span class="apidocSignatureSpan">s3.AWS.SQS.prototype.</span>verifySendMessageBatchChecksum (response)](#apidoc.element.s3.AWS.SQS.prototype.verifySendMessageBatchChecksum)
1.  [function <span class="apidocSignatureSpan">s3.AWS.SQS.prototype.</span>verifySendMessageChecksum (response)](#apidoc.element.s3.AWS.SQS.prototype.verifySendMessageChecksum)

#### [module s3.AWS.STS](#apidoc.module.s3.AWS.STS)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>STS ()](#apidoc.element.s3.AWS.STS.STS)
1.  [function <span class="apidocSignatureSpan">s3.AWS.STS.</span>__super__ (config)](#apidoc.element.s3.AWS.STS.__super__)
1.  object <span class="apidocSignatureSpan">s3.AWS.STS.</span>apiVersions
1.  object <span class="apidocSignatureSpan">s3.AWS.STS.</span>services
1.  string <span class="apidocSignatureSpan">s3.AWS.STS.</span>serviceIdentifier

#### [module s3.AWS.STS.prototype](#apidoc.module.s3.AWS.STS.prototype)
1.  [function <span class="apidocSignatureSpan">s3.AWS.STS.prototype.</span>assumeRoleWithSAML (params, callback)](#apidoc.element.s3.AWS.STS.prototype.assumeRoleWithSAML)
1.  [function <span class="apidocSignatureSpan">s3.AWS.STS.prototype.</span>assumeRoleWithWebIdentity (params, callback)](#apidoc.element.s3.AWS.STS.prototype.assumeRoleWithWebIdentity)
1.  [function <span class="apidocSignatureSpan">s3.AWS.STS.prototype.</span>constructor ()](#apidoc.element.s3.AWS.STS.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">s3.AWS.STS.prototype.</span>credentialsFrom (data, credentials)](#apidoc.element.s3.AWS.STS.prototype.credentialsFrom)

#### [module s3.AWS.SWF](#apidoc.module.s3.AWS.SWF)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>SWF ()](#apidoc.element.s3.AWS.SWF.SWF)
1.  [function <span class="apidocSignatureSpan">s3.AWS.SWF.</span>__super__ (config)](#apidoc.element.s3.AWS.SWF.__super__)
1.  object <span class="apidocSignatureSpan">s3.AWS.SWF.</span>apiVersions
1.  object <span class="apidocSignatureSpan">s3.AWS.SWF.</span>services
1.  string <span class="apidocSignatureSpan">s3.AWS.SWF.</span>serviceIdentifier

#### [module s3.AWS.SWF.prototype](#apidoc.module.s3.AWS.SWF.prototype)
1.  [function <span class="apidocSignatureSpan">s3.AWS.SWF.prototype.</span>constructor ()](#apidoc.element.s3.AWS.SWF.prototype.constructor)

#### [module s3.AWS.SequentialExecutor](#apidoc.module.s3.AWS.SequentialExecutor)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>SequentialExecutor ()](#apidoc.element.s3.AWS.SequentialExecutor.SequentialExecutor)
1.  [function <span class="apidocSignatureSpan">s3.AWS.SequentialExecutor.</span>__super__ ()](#apidoc.element.s3.AWS.SequentialExecutor.__super__)

#### [module s3.AWS.SequentialExecutor.prototype](#apidoc.module.s3.AWS.SequentialExecutor.prototype)
1.  [function <span class="apidocSignatureSpan">s3.AWS.SequentialExecutor.prototype.</span>addListener (eventName, listener)](#apidoc.element.s3.AWS.SequentialExecutor.prototype.addListener)
1.  [function <span class="apidocSignatureSpan">s3.AWS.SequentialExecutor.prototype.</span>addListeners (listeners)](#apidoc.element.s3.AWS.SequentialExecutor.prototype.addListeners)
1.  [function <span class="apidocSignatureSpan">s3.AWS.SequentialExecutor.prototype.</span>addNamedAsyncListener (name, eventName, callback)](#apidoc.element.s3.AWS.SequentialExecutor.prototype.addNamedAsyncListener)
1.  [function <span class="apidocSignatureSpan">s3.AWS.SequentialExecutor.prototype.</span>addNamedListener (name, eventName, callback)](#apidoc.element.s3.AWS.SequentialExecutor.prototype.addNamedListener)
1.  [function <span class="apidocSignatureSpan">s3.AWS.SequentialExecutor.prototype.</span>addNamedListeners (callback)](#apidoc.element.s3.AWS.SequentialExecutor.prototype.addNamedListeners)
1.  [function <span class="apidocSignatureSpan">s3.AWS.SequentialExecutor.prototype.</span>callListeners (listeners, args, doneCallback)](#apidoc.element.s3.AWS.SequentialExecutor.prototype.callListeners)
1.  [function <span class="apidocSignatureSpan">s3.AWS.SequentialExecutor.prototype.</span>constructor ()](#apidoc.element.s3.AWS.SequentialExecutor.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">s3.AWS.SequentialExecutor.prototype.</span>emit (eventName, eventArgs, doneCallback)](#apidoc.element.s3.AWS.SequentialExecutor.prototype.emit)
1.  [function <span class="apidocSignatureSpan">s3.AWS.SequentialExecutor.prototype.</span>listeners (eventName)](#apidoc.element.s3.AWS.SequentialExecutor.prototype.listeners)
1.  [function <span class="apidocSignatureSpan">s3.AWS.SequentialExecutor.prototype.</span>on (eventName, listener)](#apidoc.element.s3.AWS.SequentialExecutor.prototype.on)
1.  [function <span class="apidocSignatureSpan">s3.AWS.SequentialExecutor.prototype.</span>onAsync (eventName, listener)](#apidoc.element.s3.AWS.SequentialExecutor.prototype.onAsync)
1.  [function <span class="apidocSignatureSpan">s3.AWS.SequentialExecutor.prototype.</span>removeAllListeners (eventName)](#apidoc.element.s3.AWS.SequentialExecutor.prototype.removeAllListeners)
1.  [function <span class="apidocSignatureSpan">s3.AWS.SequentialExecutor.prototype.</span>removeListener (eventName, listener)](#apidoc.element.s3.AWS.SequentialExecutor.prototype.removeListener)

#### [module s3.AWS.Service](#apidoc.module.s3.AWS.Service)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>Service (config)](#apidoc.element.s3.AWS.Service.Service)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Service.</span>__super__ ()](#apidoc.element.s3.AWS.Service.__super__)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Service.</span>addVersions (svc, versions)](#apidoc.element.s3.AWS.Service.addVersions)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Service.</span>defineMethods (svc)](#apidoc.element.s3.AWS.Service.defineMethods)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Service.</span>defineService (serviceIdentifier, versions, features)](#apidoc.element.s3.AWS.Service.defineService)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Service.</span>defineServiceApi (superclass, version, apiConfig)](#apidoc.element.s3.AWS.Service.defineServiceApi)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Service.</span>hasService (identifier)](#apidoc.element.s3.AWS.Service.hasService)
1.  object <span class="apidocSignatureSpan">s3.AWS.Service.</span>_serviceMap

#### [module s3.AWS.Service.prototype](#apidoc.module.s3.AWS.Service.prototype)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Service.prototype.</span>addAllRequestListeners (request)](#apidoc.element.s3.AWS.Service.prototype.addAllRequestListeners)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Service.prototype.</span>constructor (config)](#apidoc.element.s3.AWS.Service.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Service.prototype.</span>endpointFromTemplate (endpoint)](#apidoc.element.s3.AWS.Service.prototype.endpointFromTemplate)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Service.prototype.</span>expiredCredentialsError (error)](#apidoc.element.s3.AWS.Service.prototype.expiredCredentialsError)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Service.prototype.</span>getLatestServiceClass (version)](#apidoc.element.s3.AWS.Service.prototype.getLatestServiceClass)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Service.prototype.</span>getLatestServiceVersion (version)](#apidoc.element.s3.AWS.Service.prototype.getLatestServiceVersion)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Service.prototype.</span>getSignerClass ()](#apidoc.element.s3.AWS.Service.prototype.getSignerClass)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Service.prototype.</span>initialize (config)](#apidoc.element.s3.AWS.Service.prototype.initialize)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Service.prototype.</span>loadServiceClass (serviceConfig)](#apidoc.element.s3.AWS.Service.prototype.loadServiceClass)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Service.prototype.</span>makeRequest (operation, params, callback)](#apidoc.element.s3.AWS.Service.prototype.makeRequest)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Service.prototype.</span>makeUnauthenticatedRequest (operation, params, callback)](#apidoc.element.s3.AWS.Service.prototype.makeUnauthenticatedRequest)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Service.prototype.</span>networkingError (error)](#apidoc.element.s3.AWS.Service.prototype.networkingError)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Service.prototype.</span>numRetries ()](#apidoc.element.s3.AWS.Service.prototype.numRetries)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Service.prototype.</span>paginationConfig (operation, throwException)](#apidoc.element.s3.AWS.Service.prototype.paginationConfig)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Service.prototype.</span>retryDelays ()](#apidoc.element.s3.AWS.Service.prototype.retryDelays)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Service.prototype.</span>retryableError (error)](#apidoc.element.s3.AWS.Service.prototype.retryableError)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Service.prototype.</span>serviceInterface ()](#apidoc.element.s3.AWS.Service.prototype.serviceInterface)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Service.prototype.</span>setEndpoint (endpoint)](#apidoc.element.s3.AWS.Service.prototype.setEndpoint)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Service.prototype.</span>setupRequestListeners ()](#apidoc.element.s3.AWS.Service.prototype.setupRequestListeners)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Service.prototype.</span>successfulResponse (resp)](#apidoc.element.s3.AWS.Service.prototype.successfulResponse)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Service.prototype.</span>throttledError (error)](#apidoc.element.s3.AWS.Service.prototype.throttledError)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Service.prototype.</span>validateService ()](#apidoc.element.s3.AWS.Service.prototype.validateService)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Service.prototype.</span>waitFor (state, params, callback)](#apidoc.element.s3.AWS.Service.prototype.waitFor)
1.  number <span class="apidocSignatureSpan">s3.AWS.Service.prototype.</span>defaultRetryCount
1.  object <span class="apidocSignatureSpan">s3.AWS.Service.prototype.</span>api

#### [module s3.AWS.SharedIniFileCredentials](#apidoc.module.s3.AWS.SharedIniFileCredentials)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>SharedIniFileCredentials (options)](#apidoc.element.s3.AWS.SharedIniFileCredentials.SharedIniFileCredentials)
1.  [function <span class="apidocSignatureSpan">s3.AWS.SharedIniFileCredentials.</span>__super__ ()](#apidoc.element.s3.AWS.SharedIniFileCredentials.__super__)

#### [module s3.AWS.SharedIniFileCredentials.prototype](#apidoc.module.s3.AWS.SharedIniFileCredentials.prototype)
1.  [function <span class="apidocSignatureSpan">s3.AWS.SharedIniFileCredentials.prototype.</span>constructor (options)](#apidoc.element.s3.AWS.SharedIniFileCredentials.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">s3.AWS.SharedIniFileCredentials.prototype.</span>loadDefaultFilename ()](#apidoc.element.s3.AWS.SharedIniFileCredentials.prototype.loadDefaultFilename)
1.  [function <span class="apidocSignatureSpan">s3.AWS.SharedIniFileCredentials.prototype.</span>refresh (callback)](#apidoc.element.s3.AWS.SharedIniFileCredentials.prototype.refresh)

#### [module s3.AWS.Signers](#apidoc.module.s3.AWS.Signers)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Signers.</span>Presign ()](#apidoc.element.s3.AWS.Signers.Presign)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Signers.</span>RequestSigner (request)](#apidoc.element.s3.AWS.Signers.RequestSigner)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Signers.</span>S3 ()](#apidoc.element.s3.AWS.Signers.S3)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Signers.</span>V2 ()](#apidoc.element.s3.AWS.Signers.V2)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Signers.</span>V3 ()](#apidoc.element.s3.AWS.Signers.V3)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Signers.</span>V3Https ()](#apidoc.element.s3.AWS.Signers.V3Https)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Signers.</span>V4 (request, serviceName)](#apidoc.element.s3.AWS.Signers.V4)

#### [module s3.AWS.Signers.Presign.prototype](#apidoc.module.s3.AWS.Signers.Presign.prototype)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Signers.Presign.prototype.</span>constructor ()](#apidoc.element.s3.AWS.Signers.Presign.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Signers.Presign.prototype.</span>sign (request, expireTime, callback)](#apidoc.element.s3.AWS.Signers.Presign.prototype.sign)

#### [module s3.AWS.Signers.RequestSigner.prototype](#apidoc.module.s3.AWS.Signers.RequestSigner.prototype)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Signers.RequestSigner.prototype.</span>constructor (request)](#apidoc.element.s3.AWS.Signers.RequestSigner.prototype.constructor)

#### [module s3.AWS.Signers.S3.prototype](#apidoc.module.s3.AWS.Signers.S3.prototype)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Signers.S3.prototype.</span>addAuthorization (credentials, date)](#apidoc.element.s3.AWS.Signers.S3.prototype.addAuthorization)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Signers.S3.prototype.</span>canonicalizedAmzHeaders ()](#apidoc.element.s3.AWS.Signers.S3.prototype.canonicalizedAmzHeaders)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Signers.S3.prototype.</span>canonicalizedResource ()](#apidoc.element.s3.AWS.Signers.S3.prototype.canonicalizedResource)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Signers.S3.prototype.</span>constructor ()](#apidoc.element.s3.AWS.Signers.S3.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Signers.S3.prototype.</span>sign (secret, string)](#apidoc.element.s3.AWS.Signers.S3.prototype.sign)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Signers.S3.prototype.</span>stringToSign ()](#apidoc.element.s3.AWS.Signers.S3.prototype.stringToSign)
1.  object <span class="apidocSignatureSpan">s3.AWS.Signers.S3.prototype.</span>responseHeaders
1.  object <span class="apidocSignatureSpan">s3.AWS.Signers.S3.prototype.</span>subResources

#### [module s3.AWS.Signers.V2.prototype](#apidoc.module.s3.AWS.Signers.V2.prototype)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Signers.V2.prototype.</span>addAuthorization (credentials, date)](#apidoc.element.s3.AWS.Signers.V2.prototype.addAuthorization)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Signers.V2.prototype.</span>constructor ()](#apidoc.element.s3.AWS.Signers.V2.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Signers.V2.prototype.</span>signature (credentials)](#apidoc.element.s3.AWS.Signers.V2.prototype.signature)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Signers.V2.prototype.</span>stringToSign ()](#apidoc.element.s3.AWS.Signers.V2.prototype.stringToSign)

#### [module s3.AWS.Signers.V3.prototype](#apidoc.module.s3.AWS.Signers.V3.prototype)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Signers.V3.prototype.</span>addAuthorization (credentials, date)](#apidoc.element.s3.AWS.Signers.V3.prototype.addAuthorization)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Signers.V3.prototype.</span>authorization (credentials)](#apidoc.element.s3.AWS.Signers.V3.prototype.authorization)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Signers.V3.prototype.</span>canonicalHeaders ()](#apidoc.element.s3.AWS.Signers.V3.prototype.canonicalHeaders)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Signers.V3.prototype.</span>constructor ()](#apidoc.element.s3.AWS.Signers.V3.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Signers.V3.prototype.</span>headersToSign ()](#apidoc.element.s3.AWS.Signers.V3.prototype.headersToSign)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Signers.V3.prototype.</span>signature (credentials)](#apidoc.element.s3.AWS.Signers.V3.prototype.signature)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Signers.V3.prototype.</span>signedHeaders ()](#apidoc.element.s3.AWS.Signers.V3.prototype.signedHeaders)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Signers.V3.prototype.</span>stringToSign ()](#apidoc.element.s3.AWS.Signers.V3.prototype.stringToSign)

#### [module s3.AWS.Signers.V3Https.prototype](#apidoc.module.s3.AWS.Signers.V3Https.prototype)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Signers.V3Https.prototype.</span>authorization (credentials)](#apidoc.element.s3.AWS.Signers.V3Https.prototype.authorization)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Signers.V3Https.prototype.</span>constructor ()](#apidoc.element.s3.AWS.Signers.V3Https.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Signers.V3Https.prototype.</span>stringToSign ()](#apidoc.element.s3.AWS.Signers.V3Https.prototype.stringToSign)

#### [module s3.AWS.Signers.V4.prototype](#apidoc.module.s3.AWS.Signers.V4.prototype)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Signers.V4.prototype.</span>addAuthorization (credentials, date)](#apidoc.element.s3.AWS.Signers.V4.prototype.addAuthorization)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Signers.V4.prototype.</span>addHeaders (credentials, datetime)](#apidoc.element.s3.AWS.Signers.V4.prototype.addHeaders)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Signers.V4.prototype.</span>authorization (credentials, datetime)](#apidoc.element.s3.AWS.Signers.V4.prototype.authorization)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Signers.V4.prototype.</span>canonicalHeaderValues (values)](#apidoc.element.s3.AWS.Signers.V4.prototype.canonicalHeaderValues)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Signers.V4.prototype.</span>canonicalHeaders ()](#apidoc.element.s3.AWS.Signers.V4.prototype.canonicalHeaders)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Signers.V4.prototype.</span>canonicalString ()](#apidoc.element.s3.AWS.Signers.V4.prototype.canonicalString)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Signers.V4.prototype.</span>constructor (request, serviceName)](#apidoc.element.s3.AWS.Signers.V4.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Signers.V4.prototype.</span>credentialString (datetime)](#apidoc.element.s3.AWS.Signers.V4.prototype.credentialString)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Signers.V4.prototype.</span>hexEncodedBodyHash ()](#apidoc.element.s3.AWS.Signers.V4.prototype.hexEncodedBodyHash)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Signers.V4.prototype.</span>hexEncodedHash (string)](#apidoc.element.s3.AWS.Signers.V4.prototype.hexEncodedHash)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Signers.V4.prototype.</span>isPresigned ()](#apidoc.element.s3.AWS.Signers.V4.prototype.isPresigned)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Signers.V4.prototype.</span>isSignableHeader (key)](#apidoc.element.s3.AWS.Signers.V4.prototype.isSignableHeader)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Signers.V4.prototype.</span>signature (credentials, datetime)](#apidoc.element.s3.AWS.Signers.V4.prototype.signature)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Signers.V4.prototype.</span>signedHeaders ()](#apidoc.element.s3.AWS.Signers.V4.prototype.signedHeaders)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Signers.V4.prototype.</span>stringToSign (datetime)](#apidoc.element.s3.AWS.Signers.V4.prototype.stringToSign)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Signers.V4.prototype.</span>updateBody (credentials)](#apidoc.element.s3.AWS.Signers.V4.prototype.updateBody)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Signers.V4.prototype.</span>updateForPresigned (credentials, datetime)](#apidoc.element.s3.AWS.Signers.V4.prototype.updateForPresigned)
1.  object <span class="apidocSignatureSpan">s3.AWS.Signers.V4.prototype.</span>unsignableHeaders
1.  string <span class="apidocSignatureSpan">s3.AWS.Signers.V4.prototype.</span>algorithm

#### [module s3.AWS.SimpleDB](#apidoc.module.s3.AWS.SimpleDB)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>SimpleDB ()](#apidoc.element.s3.AWS.SimpleDB.SimpleDB)
1.  [function <span class="apidocSignatureSpan">s3.AWS.SimpleDB.</span>__super__ (config)](#apidoc.element.s3.AWS.SimpleDB.__super__)
1.  object <span class="apidocSignatureSpan">s3.AWS.SimpleDB.</span>apiVersions
1.  object <span class="apidocSignatureSpan">s3.AWS.SimpleDB.</span>services
1.  string <span class="apidocSignatureSpan">s3.AWS.SimpleDB.</span>serviceIdentifier

#### [module s3.AWS.SimpleDB.prototype](#apidoc.module.s3.AWS.SimpleDB.prototype)
1.  [function <span class="apidocSignatureSpan">s3.AWS.SimpleDB.prototype.</span>constructor ()](#apidoc.element.s3.AWS.SimpleDB.prototype.constructor)

#### [module s3.AWS.StorageGateway](#apidoc.module.s3.AWS.StorageGateway)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>StorageGateway ()](#apidoc.element.s3.AWS.StorageGateway.StorageGateway)
1.  [function <span class="apidocSignatureSpan">s3.AWS.StorageGateway.</span>__super__ (config)](#apidoc.element.s3.AWS.StorageGateway.__super__)
1.  object <span class="apidocSignatureSpan">s3.AWS.StorageGateway.</span>apiVersions
1.  object <span class="apidocSignatureSpan">s3.AWS.StorageGateway.</span>services
1.  string <span class="apidocSignatureSpan">s3.AWS.StorageGateway.</span>serviceIdentifier

#### [module s3.AWS.StorageGateway.prototype](#apidoc.module.s3.AWS.StorageGateway.prototype)
1.  [function <span class="apidocSignatureSpan">s3.AWS.StorageGateway.prototype.</span>constructor ()](#apidoc.element.s3.AWS.StorageGateway.prototype.constructor)

#### [module s3.AWS.Support](#apidoc.module.s3.AWS.Support)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>Support ()](#apidoc.element.s3.AWS.Support.Support)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Support.</span>__super__ (config)](#apidoc.element.s3.AWS.Support.__super__)
1.  object <span class="apidocSignatureSpan">s3.AWS.Support.</span>apiVersions
1.  object <span class="apidocSignatureSpan">s3.AWS.Support.</span>services
1.  string <span class="apidocSignatureSpan">s3.AWS.Support.</span>serviceIdentifier

#### [module s3.AWS.Support.prototype](#apidoc.module.s3.AWS.Support.prototype)
1.  [function <span class="apidocSignatureSpan">s3.AWS.Support.prototype.</span>constructor ()](#apidoc.element.s3.AWS.Support.prototype.constructor)

#### [module s3.AWS.TemporaryCredentials](#apidoc.module.s3.AWS.TemporaryCredentials)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>TemporaryCredentials (params)](#apidoc.element.s3.AWS.TemporaryCredentials.TemporaryCredentials)
1.  [function <span class="apidocSignatureSpan">s3.AWS.TemporaryCredentials.</span>__super__ ()](#apidoc.element.s3.AWS.TemporaryCredentials.__super__)

#### [module s3.AWS.TemporaryCredentials.prototype](#apidoc.module.s3.AWS.TemporaryCredentials.prototype)
1.  [function <span class="apidocSignatureSpan">s3.AWS.TemporaryCredentials.prototype.</span>constructor (params)](#apidoc.element.s3.AWS.TemporaryCredentials.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">s3.AWS.TemporaryCredentials.prototype.</span>loadMasterCredentials ()](#apidoc.element.s3.AWS.TemporaryCredentials.prototype.loadMasterCredentials)
1.  [function <span class="apidocSignatureSpan">s3.AWS.TemporaryCredentials.prototype.</span>refresh (callback)](#apidoc.element.s3.AWS.TemporaryCredentials.prototype.refresh)

#### [module s3.AWS.WebIdentityCredentials](#apidoc.module.s3.AWS.WebIdentityCredentials)
1.  [function <span class="apidocSignatureSpan">s3.AWS.</span>WebIdentityCredentials (params)](#apidoc.element.s3.AWS.WebIdentityCredentials.WebIdentityCredentials)
1.  [function <span class="apidocSignatureSpan">s3.AWS.WebIdentityCredentials.</span>__super__ ()](#apidoc.element.s3.AWS.WebIdentityCredentials.__super__)

#### [module s3.AWS.WebIdentityCredentials.prototype](#apidoc.module.s3.AWS.WebIdentityCredentials.prototype)
1.  [function <span class="apidocSignatureSpan">s3.AWS.WebIdentityCredentials.prototype.</span>constructor (params)](#apidoc.element.s3.AWS.WebIdentityCredentials.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">s3.AWS.WebIdentityCredentials.prototype.</span>refresh (callback)](#apidoc.element.s3.AWS.WebIdentityCredentials.prototype.refresh)

#### [module s3.AWS.XML](#apidoc.module.s3.AWS.XML)
1.  [function <span class="apidocSignatureSpan">s3.AWS.XML.</span>Builder ()](#apidoc.element.s3.AWS.XML.Builder)
1.  [function <span class="apidocSignatureSpan">s3.AWS.XML.</span>Parser ()](#apidoc.element.s3.AWS.XML.Parser)

#### [module s3.AWS.XML.Builder.prototype](#apidoc.module.s3.AWS.XML.Builder.prototype)
1.  [function <span class="apidocSignatureSpan">s3.AWS.XML.Builder.prototype.</span>toXML (params, shape, rootElement)](#apidoc.element.s3.AWS.XML.Builder.prototype.toXML)

#### [module s3.AWS.XML.Parser.prototype](#apidoc.module.s3.AWS.XML.Parser.prototype)
1.  [function <span class="apidocSignatureSpan">s3.AWS.XML.Parser.prototype.</span>parse (xml, shape)](#apidoc.element.s3.AWS.XML.Parser.prototype.parse)

#### [module s3.AWS.util](#apidoc.module.s3.AWS.util)
1.  [function <span class="apidocSignatureSpan">s3.AWS.util.</span>Buffer (arg, encodingOrOffset, length)](#apidoc.element.s3.AWS.util.Buffer)
1.  [function <span class="apidocSignatureSpan">s3.AWS.util.</span>arrayEach (array, iterFunction)](#apidoc.element.s3.AWS.util.arrayEach)
1.  [function <span class="apidocSignatureSpan">s3.AWS.util.</span>copy (object)](#apidoc.element.s3.AWS.util.copy)
1.  [function <span class="apidocSignatureSpan">s3.AWS.util.</span>each (object, iterFunction)](#apidoc.element.s3.AWS.util.each)
1.  [function <span class="apidocSignatureSpan">s3.AWS.util.</span>engine ()](#apidoc.element.s3.AWS.util.engine)
1.  [function <span class="apidocSignatureSpan">s3.AWS.util.</span>error (err, options)](#apidoc.element.s3.AWS.util.error)
1.  [function <span class="apidocSignatureSpan">s3.AWS.util.</span>hideProperties (obj, props)](#apidoc.element.s3.AWS.util.hideProperties)
1.  [function <span class="apidocSignatureSpan">s3.AWS.util.</span>inherit (klass, features)](#apidoc.element.s3.AWS.util.inherit)
1.  [function <span class="apidocSignatureSpan">s3.AWS.util.</span>isBrowser ()](#apidoc.element.s3.AWS.util.isBrowser)
1.  [function <span class="apidocSignatureSpan">s3.AWS.util.</span>isEmpty (obj)](#apidoc.element.s3.AWS.util.isEmpty)
1.  [function <span class="apidocSignatureSpan">s3.AWS.util.</span>isNode ()](#apidoc.element.s3.AWS.util.isNode)
1.  [function <span class="apidocSignatureSpan">s3.AWS.util.</span>isType (obj, type)](#apidoc.element.s3.AWS.util.isType)
1.  [function <span class="apidocSignatureSpan">s3.AWS.util.</span>memoizedProperty (obj, name, get, enumerable)](#apidoc.element.s3.AWS.util.memoizedProperty)
1.  [function <span class="apidocSignatureSpan">s3.AWS.util.</span>merge (obj1, obj2)](#apidoc.element.s3.AWS.util.merge)
1.  [function <span class="apidocSignatureSpan">s3.AWS.util.</span>mixin ()](#apidoc.element.s3.AWS.util.mixin)
1.  [function <span class="apidocSignatureSpan">s3.AWS.util.</span>multiRequire (module1, module2)](#apidoc.element.s3.AWS.util.multiRequire)
1.  [function <span class="apidocSignatureSpan">s3.AWS.util.</span>nodeRequire (module)](#apidoc.element.s3.AWS.util.nodeRequire)
1.  [function <span class="apidocSignatureSpan">s3.AWS.util.</span>property (obj, name, value, enumerable, isValue)](#apidoc.element.s3.AWS.util.property)
1.  [function <span class="apidocSignatureSpan">s3.AWS.util.</span>queryParamsToString (params)](#apidoc.element.s3.AWS.util.queryParamsToString)
1.  [function <span class="apidocSignatureSpan">s3.AWS.util.</span>queryStringParse (qs)](#apidoc.element.s3.AWS.util.queryStringParse)
1.  [function <span class="apidocSignatureSpan">s3.AWS.util.</span>readFileSync (path)](#apidoc.element.s3.AWS.util.readFileSync)
1.  [function <span class="apidocSignatureSpan">s3.AWS.util.</span>typeName (type)](#apidoc.element.s3.AWS.util.typeName)
1.  [function <span class="apidocSignatureSpan">s3.AWS.util.</span>update (obj1, obj2)](#apidoc.element.s3.AWS.util.update)
1.  [function <span class="apidocSignatureSpan">s3.AWS.util.</span>uriEscape (string)](#apidoc.element.s3.AWS.util.uriEscape)
1.  [function <span class="apidocSignatureSpan">s3.AWS.util.</span>uriEscapePath (string)](#apidoc.element.s3.AWS.util.uriEscapePath)
1.  [function <span class="apidocSignatureSpan">s3.AWS.util.</span>urlFormat (url)](#apidoc.element.s3.AWS.util.urlFormat)
1.  [function <span class="apidocSignatureSpan">s3.AWS.util.</span>urlParse (url)](#apidoc.element.s3.AWS.util.urlParse)
1.  [function <span class="apidocSignatureSpan">s3.AWS.util.</span>userAgent ()](#apidoc.element.s3.AWS.util.userAgent)
1.  object <span class="apidocSignatureSpan">s3.AWS.util.</span>abort
1.  object <span class="apidocSignatureSpan">s3.AWS.util.</span>base64
1.  object <span class="apidocSignatureSpan">s3.AWS.util.</span>buffer
1.  object <span class="apidocSignatureSpan">s3.AWS.util.</span>crypto
1.  object <span class="apidocSignatureSpan">s3.AWS.util.</span>date
1.  object <span class="apidocSignatureSpan">s3.AWS.util.</span>fn
1.  object <span class="apidocSignatureSpan">s3.AWS.util.</span>ini
1.  object <span class="apidocSignatureSpan">s3.AWS.util.</span>jamespath
1.  object <span class="apidocSignatureSpan">s3.AWS.util.</span>string

#### [module s3.AWS.util.Buffer.prototype](#apidoc.module.s3.AWS.util.Buffer.prototype)
1.  [function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>asciiSlice ()](#apidoc.element.s3.AWS.util.Buffer.prototype.asciiSlice)
1.  [function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>asciiWrite ()](#apidoc.element.s3.AWS.util.Buffer.prototype.asciiWrite)
1.  [function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>base64Slice ()](#apidoc.element.s3.AWS.util.Buffer.prototype.base64Slice)
1.  [function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>base64Write ()](#apidoc.element.s3.AWS.util.Buffer.prototype.base64Write)
1.  [function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>compare (target, start, end, thisStart, thisEnd)](#apidoc.element.s3.AWS.util.Buffer.prototype.compare)
1.  [function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>copy ()](#apidoc.element.s3.AWS.util.Buffer.prototype.copy)
1.  [function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>equals (b)](#apidoc.element.s3.AWS.util.Buffer.prototype.equals)
1.  [function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>fill (val, start, end, encoding)](#apidoc.element.s3.AWS.util.Buffer.prototype.fill)
1.  [function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>hexSlice ()](#apidoc.element.s3.AWS.util.Buffer.prototype.hexSlice)
1.  [function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>hexWrite ()](#apidoc.element.s3.AWS.util.Buffer.prototype.hexWrite)
1.  [function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>includes (val, byteOffset, encoding)](#apidoc.element.s3.AWS.util.Buffer.prototype.includes)
1.  [function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>indexOf (val, byteOffset, encoding)](#apidoc.element.s3.AWS.util.Buffer.prototype.indexOf)
1.  [function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>inspect ()](#apidoc.element.s3.AWS.util.Buffer.prototype.inspect)
1.  [function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>lastIndexOf (val, byteOffset, encoding)](#apidoc.element.s3.AWS.util.Buffer.prototype.lastIndexOf)
1.  [function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>latin1Slice ()](#apidoc.element.s3.AWS.util.Buffer.prototype.latin1Slice)
1.  [function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>latin1Write ()](#apidoc.element.s3.AWS.util.Buffer.prototype.latin1Write)
1.  [function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>readDoubleBE (offset, noAssert)](#apidoc.element.s3.AWS.util.Buffer.prototype.readDoubleBE)
1.  [function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>readDoubleLE (offset, noAssert)](#apidoc.element.s3.AWS.util.Buffer.prototype.readDoubleLE)
1.  [function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>readFloatBE (offset, noAssert)](#apidoc.element.s3.AWS.util.Buffer.prototype.readFloatBE)
1.  [function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>readFloatLE (offset, noAssert)](#apidoc.element.s3.AWS.util.Buffer.prototype.readFloatLE)
1.  [function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>readInt16BE (offset, noAssert)](#apidoc.element.s3.AWS.util.Buffer.prototype.readInt16BE)
1.  [function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>readInt16LE (offset, noAssert)](#apidoc.element.s3.AWS.util.Buffer.prototype.readInt16LE)
1.  [function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>readInt32BE (offset, noAssert)](#apidoc.element.s3.AWS.util.Buffer.prototype.readInt32BE)
1.  [function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>readInt32LE (offset, noAssert)](#apidoc.element.s3.AWS.util.Buffer.prototype.readInt32LE)
1.  [function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>readInt8 (offset, noAssert)](#apidoc.element.s3.AWS.util.Buffer.prototype.readInt8)
1.  [function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>readIntBE (offset, byteLength, noAssert)](#apidoc.element.s3.AWS.util.Buffer.prototype.readIntBE)
1.  [function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>readIntLE (offset, byteLength, noAssert)](#apidoc.element.s3.AWS.util.Buffer.prototype.readIntLE)
1.  [function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>readUInt16BE (offset, noAssert)](#apidoc.element.s3.AWS.util.Buffer.prototype.readUInt16BE)
1.  [function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>readUInt16LE (offset, noAssert)](#apidoc.element.s3.AWS.util.Buffer.prototype.readUInt16LE)
1.  [function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>readUInt32BE (offset, noAssert)](#apidoc.element.s3.AWS.util.Buffer.prototype.readUInt32BE)
1.  [function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>readUInt32LE (offset, noAssert)](#apidoc.element.s3.AWS.util.Buffer.prototype.readUInt32LE)
1.  [function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>readUInt8 (offset, noAssert)](#apidoc.element.s3.AWS.util.Buffer.prototype.readUInt8)
1.  [function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>readUIntBE (offset, byteLength, noAssert)](#apidoc.element.s3.AWS.util.Buffer.prototype.readUIntBE)
1.  [function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>readUIntLE (offset, byteLength, noAssert)](#apidoc.element.s3.AWS.util.Buffer.prototype.readUIntLE)
1.  [function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>slice (start, end)](#apidoc.element.s3.AWS.util.Buffer.prototype.slice)
1.  [function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>swap16 ()](#apidoc.element.s3.AWS.util.Buffer.prototype.swap16)
1.  [function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>swap32 ()](#apidoc.element.s3.AWS.util.Buffer.prototype.swap32)
1.  [function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>swap64 ()](#apidoc.element.s3.AWS.util.Buffer.prototype.swap64)
1.  [function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>toJSON ()](#apidoc.element.s3.AWS.util.Buffer.prototype.toJSON)
1.  [function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>toString ()](#apidoc.element.s3.AWS.util.Buffer.prototype.toString)
1.  [function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>ucs2Slice ()](#apidoc.element.s3.AWS.util.Buffer.prototype.ucs2Slice)
1.  [function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>ucs2Write ()](#apidoc.element.s3.AWS.util.Buffer.prototype.ucs2Write)
1.  [function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>utf8Slice ()](#apidoc.element.s3.AWS.util.Buffer.prototype.utf8Slice)
1.  [function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>utf8Write ()](#apidoc.element.s3.AWS.util.Buffer.prototype.utf8Write)
1.  [function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>write (string, offset, length, encoding)](#apidoc.element.s3.AWS.util.Buffer.prototype.write)
1.  [function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>writeDoubleBE (val, offset, noAssert)](#apidoc.element.s3.AWS.util.Buffer.prototype.writeDoubleBE)
1.  [function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>writeDoubleLE (val, offset, noAssert)](#apidoc.element.s3.AWS.util.Buffer.prototype.writeDoubleLE)
1.  [function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>writeFloatBE (val, offset, noAssert)](#apidoc.element.s3.AWS.util.Buffer.prototype.writeFloatBE)
1.  [function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>writeFloatLE (val, offset, noAssert)](#apidoc.element.s3.AWS.util.Buffer.prototype.writeFloatLE)
1.  [function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>writeInt16BE (value, offset, noAssert)](#apidoc.element.s3.AWS.util.Buffer.prototype.writeInt16BE)
1.  [function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>writeInt16LE (value, offset, noAssert)](#apidoc.element.s3.AWS.util.Buffer.prototype.writeInt16LE)
1.  [function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>writeInt32BE (value, offset, noAssert)](#apidoc.element.s3.AWS.util.Buffer.prototype.writeInt32BE)
1.  [function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>writeInt32LE (value, offset, noAssert)](#apidoc.element.s3.AWS.util.Buffer.prototype.writeInt32LE)
1.  [function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>writeInt8 (value, offset, noAssert)](#apidoc.element.s3.AWS.util.Buffer.prototype.writeInt8)
1.  [function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>writeIntBE (value, offset, byteLength, noAssert)](#apidoc.element.s3.AWS.util.Buffer.prototype.writeIntBE)
1.  [function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>writeIntLE (value, offset, byteLength, noAssert)](#apidoc.element.s3.AWS.util.Buffer.prototype.writeIntLE)
1.  [function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>writeUInt16BE (value, offset, noAssert)](#apidoc.element.s3.AWS.util.Buffer.prototype.writeUInt16BE)
1.  [function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>writeUInt16LE (value, offset, noAssert)](#apidoc.element.s3.AWS.util.Buffer.prototype.writeUInt16LE)
1.  [function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>writeUInt32BE (value, offset, noAssert)](#apidoc.element.s3.AWS.util.Buffer.prototype.writeUInt32BE)
1.  [function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>writeUInt32LE (value, offset, noAssert)](#apidoc.element.s3.AWS.util.Buffer.prototype.writeUInt32LE)
1.  [function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>writeUInt8 (value, offset, noAssert)](#apidoc.element.s3.AWS.util.Buffer.prototype.writeUInt8)
1.  [function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>writeUIntBE (value, offset, byteLength, noAssert)](#apidoc.element.s3.AWS.util.Buffer.prototype.writeUIntBE)
1.  [function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>writeUIntLE (value, offset, byteLength, noAssert)](#apidoc.element.s3.AWS.util.Buffer.prototype.writeUIntLE)

#### [module s3.Client](#apidoc.module.s3.Client)
1.  [function <span class="apidocSignatureSpan">s3.</span>Client (options)](#apidoc.element.s3.Client.Client)

#### [module s3.Client.prototype](#apidoc.module.s3.Client.prototype)
1.  [function <span class="apidocSignatureSpan">s3.Client.prototype.</span>copyObject (_s3Params)](#apidoc.element.s3.Client.prototype.copyObject)
1.  [function <span class="apidocSignatureSpan">s3.Client.prototype.</span>deleteDir (s3Params)](#apidoc.element.s3.Client.prototype.deleteDir)
1.  [function <span class="apidocSignatureSpan">s3.Client.prototype.</span>deleteObjects (s3Params)](#apidoc.element.s3.Client.prototype.deleteObjects)
1.  [function <span class="apidocSignatureSpan">s3.Client.prototype.</span>downloadBuffer (s3Params)](#apidoc.element.s3.Client.prototype.downloadBuffer)
1.  [function <span class="apidocSignatureSpan">s3.Client.prototype.</span>downloadDir (params)](#apidoc.element.s3.Client.prototype.downloadDir)
1.  [function <span class="apidocSignatureSpan">s3.Client.prototype.</span>downloadFile (params)](#apidoc.element.s3.Client.prototype.downloadFile)
1.  [function <span class="apidocSignatureSpan">s3.Client.prototype.</span>downloadStream (s3Params)](#apidoc.element.s3.Client.prototype.downloadStream)
1.  [function <span class="apidocSignatureSpan">s3.Client.prototype.</span>listObjects (params)](#apidoc.element.s3.Client.prototype.listObjects)
1.  [function <span class="apidocSignatureSpan">s3.Client.prototype.</span>moveObject (s3Params)](#apidoc.element.s3.Client.prototype.moveObject)
1.  [function <span class="apidocSignatureSpan">s3.Client.prototype.</span>uploadDir (params)](#apidoc.element.s3.Client.prototype.uploadDir)
1.  [function <span class="apidocSignatureSpan">s3.Client.prototype.</span>uploadFile (params)](#apidoc.element.s3.Client.prototype.uploadFile)

#### [module s3.MultipartETag](#apidoc.module.s3.MultipartETag)
1.  [function <span class="apidocSignatureSpan">s3.</span>MultipartETag (options)](#apidoc.element.s3.MultipartETag.MultipartETag)
1.  [function <span class="apidocSignatureSpan">s3.MultipartETag.</span>super_ (options)](#apidoc.element.s3.MultipartETag.super_)

#### [module s3.MultipartETag.prototype](#apidoc.module.s3.MultipartETag.prototype)
1.  [function <span class="apidocSignatureSpan">s3.MultipartETag.prototype.</span>_flush (callback)](#apidoc.element.s3.MultipartETag.prototype._flush)
1.  [function <span class="apidocSignatureSpan">s3.MultipartETag.prototype.</span>_transform (chunk, encoding, callback)](#apidoc.element.s3.MultipartETag.prototype._transform)
1.  [function <span class="apidocSignatureSpan">s3.MultipartETag.prototype.</span>anyMatch (eTag)](#apidoc.element.s3.MultipartETag.prototype.anyMatch)



# <a name="apidoc.module.s3"></a>[module s3](#apidoc.module.s3)

#### <a name="apidoc.element.s3.AWS.AutoScaling"></a>[function <span class="apidocSignatureSpan">s3.</span>AWS.AutoScaling ()](#apidoc.element.s3.AWS.AutoScaling)
- description and source-code
```javascript
AWS.AutoScaling = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.CloudFormation"></a>[function <span class="apidocSignatureSpan">s3.</span>AWS.CloudFormation ()](#apidoc.element.s3.AWS.CloudFormation)
- description and source-code
```javascript
AWS.CloudFormation = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.CloudFront"></a>[function <span class="apidocSignatureSpan">s3.</span>AWS.CloudFront ()](#apidoc.element.s3.AWS.CloudFront)
- description and source-code
```javascript
AWS.CloudFront = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.CloudSearch"></a>[function <span class="apidocSignatureSpan">s3.</span>AWS.CloudSearch ()](#apidoc.element.s3.AWS.CloudSearch)
- description and source-code
```javascript
AWS.CloudSearch = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.CloudSearchDomain"></a>[function <span class="apidocSignatureSpan">s3.</span>AWS.CloudSearchDomain ()](#apidoc.element.s3.AWS.CloudSearchDomain)
- description and source-code
```javascript
AWS.CloudSearchDomain = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.CloudTrail"></a>[function <span class="apidocSignatureSpan">s3.</span>AWS.CloudTrail ()](#apidoc.element.s3.AWS.CloudTrail)
- description and source-code
```javascript
AWS.CloudTrail = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.CloudWatch"></a>[function <span class="apidocSignatureSpan">s3.</span>AWS.CloudWatch ()](#apidoc.element.s3.AWS.CloudWatch)
- description and source-code
```javascript
AWS.CloudWatch = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.CloudWatchLogs"></a>[function <span class="apidocSignatureSpan">s3.</span>AWS.CloudWatchLogs ()](#apidoc.element.s3.AWS.CloudWatchLogs)
- description and source-code
```javascript
AWS.CloudWatchLogs = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.CodeDeploy"></a>[function <span class="apidocSignatureSpan">s3.</span>AWS.CodeDeploy ()](#apidoc.element.s3.AWS.CodeDeploy)
- description and source-code
```javascript
AWS.CodeDeploy = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.CognitoIdentity"></a>[function <span class="apidocSignatureSpan">s3.</span>AWS.CognitoIdentity ()](#apidoc.element.s3.AWS.CognitoIdentity)
- description and source-code
```javascript
AWS.CognitoIdentity = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.CognitoIdentityCredentials"></a>[function <span class="apidocSignatureSpan">s3.</span>AWS.CognitoIdentityCredentials (params)](#apidoc.element.s3.AWS.CognitoIdentityCredentials)
- description and source-code
```javascript
function CognitoIdentityCredentials(params) {
  AWS.Credentials.call(this);
  this.expired = true;
  this.webIdentityCredentials = new AWS.WebIdentityCredentials(params);
  this.cognito = new AWS.CognitoIdentity({params: params});
  this.sts = new AWS.STS();
  this.params = params;
  this.data = null;
  this.identityId = null;
  this.loadCachedId();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.CognitoSync"></a>[function <span class="apidocSignatureSpan">s3.</span>AWS.CognitoSync ()](#apidoc.element.s3.AWS.CognitoSync)
- description and source-code
```javascript
AWS.CognitoSync = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Config"></a>[function <span class="apidocSignatureSpan">s3.</span>AWS.Config (options)](#apidoc.element.s3.AWS.Config)
- description and source-code
```javascript
function Config(options) {
  if (options === undefined) options = {};
  options = this.extractCredentials(options);

  AWS.util.each.call(this, this.keys, function (key, value) {
    this.set(key, options[key], value);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.ConfigService"></a>[function <span class="apidocSignatureSpan">s3.</span>AWS.ConfigService ()](#apidoc.element.s3.AWS.ConfigService)
- description and source-code
```javascript
AWS.ConfigService = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.CredentialProviderChain"></a>[function <span class="apidocSignatureSpan">s3.</span>AWS.CredentialProviderChain (providers)](#apidoc.element.s3.AWS.CredentialProviderChain)
- description and source-code
```javascript
function CredentialProviderChain(providers) {
  if (providers) {
    this.providers = providers;
  } else {
    this.providers = AWS.CredentialProviderChain.defaultProviders.slice(0);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Credentials"></a>[function <span class="apidocSignatureSpan">s3.</span>AWS.Credentials ()](#apidoc.element.s3.AWS.Credentials)
- description and source-code
```javascript
function Credentials() {
  // hide secretAccessKey from being displayed with util.inspect
  AWS.util.hideProperties(this, ['secretAccessKey']);

  this.expired = false;
  this.expireTime = null;
  if (arguments.length === 1 && typeof arguments[0] === 'object') {
    var creds = arguments[0].credentials || arguments[0];
    this.accessKeyId = creds.accessKeyId;
    this.secretAccessKey = creds.secretAccessKey;
    this.sessionToken = creds.sessionToken;
  } else {
    this.accessKeyId = arguments[0];
    this.secretAccessKey = arguments[1];
    this.sessionToken = arguments[2];
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.DataPipeline"></a>[function <span class="apidocSignatureSpan">s3.</span>AWS.DataPipeline ()](#apidoc.element.s3.AWS.DataPipeline)
- description and source-code
```javascript
AWS.DataPipeline = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.DirectConnect"></a>[function <span class="apidocSignatureSpan">s3.</span>AWS.DirectConnect ()](#apidoc.element.s3.AWS.DirectConnect)
- description and source-code
```javascript
AWS.DirectConnect = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.DynamoDB"></a>[function <span class="apidocSignatureSpan">s3.</span>AWS.DynamoDB ()](#apidoc.element.s3.AWS.DynamoDB)
- description and source-code
```javascript
AWS.DynamoDB = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.EC2"></a>[function <span class="apidocSignatureSpan">s3.</span>AWS.EC2 ()](#apidoc.element.s3.AWS.EC2)
- description and source-code
```javascript
AWS.EC2 = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.EC2MetadataCredentials"></a>[function <span class="apidocSignatureSpan">s3.</span>AWS.EC2MetadataCredentials (options)](#apidoc.element.s3.AWS.EC2MetadataCredentials)
- description and source-code
```javascript
function EC2MetadataCredentials(options) {
  AWS.Credentials.call(this);

  options = options ? AWS.util.copy(options) : {};
  if (!options.httpOptions) options.httpOptions = {};
  options.httpOptions = AWS.util.merge(
    {timeout: this.defaultTimeout}, options.httpOptions);

  this.metadataService = new AWS.MetadataService(options);
  this.metadata = {};
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.ELB"></a>[function <span class="apidocSignatureSpan">s3.</span>AWS.ELB ()](#apidoc.element.s3.AWS.ELB)
- description and source-code
```javascript
AWS.ELB = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.EMR"></a>[function <span class="apidocSignatureSpan">s3.</span>AWS.EMR ()](#apidoc.element.s3.AWS.EMR)
- description and source-code
```javascript
AWS.EMR = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.ElastiCache"></a>[function <span class="apidocSignatureSpan">s3.</span>AWS.ElastiCache ()](#apidoc.element.s3.AWS.ElastiCache)
- description and source-code
```javascript
AWS.ElastiCache = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.ElasticBeanstalk"></a>[function <span class="apidocSignatureSpan">s3.</span>AWS.ElasticBeanstalk ()](#apidoc.element.s3.AWS.ElasticBeanstalk)
- description and source-code
```javascript
AWS.ElasticBeanstalk = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.ElasticTranscoder"></a>[function <span class="apidocSignatureSpan">s3.</span>AWS.ElasticTranscoder ()](#apidoc.element.s3.AWS.ElasticTranscoder)
- description and source-code
```javascript
AWS.ElasticTranscoder = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Endpoint"></a>[function <span class="apidocSignatureSpan">s3.</span>AWS.Endpoint (endpoint, config)](#apidoc.element.s3.AWS.Endpoint)
- description and source-code
```javascript
function Endpoint(endpoint, config) {
  AWS.util.hideProperties(this, ['slashes', 'auth', 'hash', 'search', 'query']);

  if (typeof endpoint === 'undefined' || endpoint === null) {
    throw new Error('Invalid endpoint: ' + endpoint);
  } else if (typeof endpoint !== 'string') {
    return AWS.util.copy(endpoint);
  }

  if (!endpoint.match(/^http/)) {
    var useSSL = config && config.sslEnabled !== undefined ?
      config.sslEnabled : AWS.config.sslEnabled;
    endpoint = (useSSL ? 'https' : 'http') + '://' + endpoint;
  }

  AWS.util.update(this, AWS.util.urlParse(endpoint));

  // Ensure the port property is set as an integer
  if (this.port) {
    this.port = parseInt(this.port, 10);
  } else {
    this.port = this.protocol === 'https:' ? 443 : 80;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.EnvironmentCredentials"></a>[function <span class="apidocSignatureSpan">s3.</span>AWS.EnvironmentCredentials (envPrefix)](#apidoc.element.s3.AWS.EnvironmentCredentials)
- description and source-code
```javascript
function EnvironmentCredentials(envPrefix) {
  AWS.Credentials.call(this);
  this.envPrefix = envPrefix;
  this.get(function() {});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.FileSystemCredentials"></a>[function <span class="apidocSignatureSpan">s3.</span>AWS.FileSystemCredentials (filename)](#apidoc.element.s3.AWS.FileSystemCredentials)
- description and source-code
```javascript
function FileSystemCredentials(filename) {
  AWS.Credentials.call(this);
  this.filename = filename;
  this.get(function() {});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Glacier"></a>[function <span class="apidocSignatureSpan">s3.</span>AWS.Glacier ()](#apidoc.element.s3.AWS.Glacier)
- description and source-code
```javascript
AWS.Glacier = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.HttpClient"></a>[function <span class="apidocSignatureSpan">s3.</span>AWS.HttpClient ()](#apidoc.element.s3.AWS.HttpClient)
- description and source-code
```javascript
AWS.HttpClient = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.HttpRequest"></a>[function <span class="apidocSignatureSpan">s3.</span>AWS.HttpRequest (endpoint, region)](#apidoc.element.s3.AWS.HttpRequest)
- description and source-code
```javascript
function HttpRequest(endpoint, region) {
  endpoint = new AWS.Endpoint(endpoint);
  this.method = 'POST';
  this.path = endpoint.path || '/';
  this.headers = {};
  this.body = '';
  this.endpoint = endpoint;
  this.region = region;
  this.setUserAgent();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.HttpResponse"></a>[function <span class="apidocSignatureSpan">s3.</span>AWS.HttpResponse ()](#apidoc.element.s3.AWS.HttpResponse)
- description and source-code
```javascript
function HttpResponse() {
  this.statusCode = undefined;
  this.headers = {};
  this.body = undefined;
  this.streaming = false;
  this.stream = null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.IAM"></a>[function <span class="apidocSignatureSpan">s3.</span>AWS.IAM ()](#apidoc.element.s3.AWS.IAM)
- description and source-code
```javascript
AWS.IAM = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.ImportExport"></a>[function <span class="apidocSignatureSpan">s3.</span>AWS.ImportExport ()](#apidoc.element.s3.AWS.ImportExport)
- description and source-code
```javascript
AWS.ImportExport = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.KMS"></a>[function <span class="apidocSignatureSpan">s3.</span>AWS.KMS ()](#apidoc.element.s3.AWS.KMS)
- description and source-code
```javascript
AWS.KMS = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Kinesis"></a>[function <span class="apidocSignatureSpan">s3.</span>AWS.Kinesis ()](#apidoc.element.s3.AWS.Kinesis)
- description and source-code
```javascript
AWS.Kinesis = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Lambda"></a>[function <span class="apidocSignatureSpan">s3.</span>AWS.Lambda ()](#apidoc.element.s3.AWS.Lambda)
- description and source-code
```javascript
AWS.Lambda = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.MetadataService"></a>[function <span class="apidocSignatureSpan">s3.</span>AWS.MetadataService (options)](#apidoc.element.s3.AWS.MetadataService)
- description and source-code
```javascript
function MetadataService(options) {
  AWS.util.update(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.NodeHttpClient"></a>[function <span class="apidocSignatureSpan">s3.</span>AWS.NodeHttpClient ()](#apidoc.element.s3.AWS.NodeHttpClient)
- description and source-code
```javascript
AWS.NodeHttpClient = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.OpsWorks"></a>[function <span class="apidocSignatureSpan">s3.</span>AWS.OpsWorks ()](#apidoc.element.s3.AWS.OpsWorks)
- description and source-code
```javascript
AWS.OpsWorks = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.ParamValidator"></a>[function <span class="apidocSignatureSpan">s3.</span>AWS.ParamValidator ()](#apidoc.element.s3.AWS.ParamValidator)
- description and source-code
```javascript
AWS.ParamValidator = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.RDS"></a>[function <span class="apidocSignatureSpan">s3.</span>AWS.RDS ()](#apidoc.element.s3.AWS.RDS)
- description and source-code
```javascript
AWS.RDS = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Redshift"></a>[function <span class="apidocSignatureSpan">s3.</span>AWS.Redshift ()](#apidoc.element.s3.AWS.Redshift)
- description and source-code
```javascript
AWS.Redshift = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Request"></a>[function <span class="apidocSignatureSpan">s3.</span>AWS.Request (service, operation, params)](#apidoc.element.s3.AWS.Request)
- description and source-code
```javascript
function Request(service, operation, params) {
  var endpoint = service.endpoint;
  var region = service.config.region;

  // global endpoints sign as us-east-1
  if (service.isGlobalEndpoint) region = 'us-east-1';

  this.domain = domain && domain.active;
  this.service = service;
  this.operation = operation;
  this.params = params || {};
  this.httpRequest = new AWS.HttpRequest(endpoint, region);
  this.startTime = AWS.util.date.getDate();

  this.response = new AWS.Response(this);
  this._asm = new AcceptorStateMachine(fsm.states, 'validate');

  AWS.SequentialExecutor.call(this);
  this.emit = this.emitEvent;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.ResourceWaiter"></a>[function <span class="apidocSignatureSpan">s3.</span>AWS.ResourceWaiter (service, state)](#apidoc.element.s3.AWS.ResourceWaiter)
- description and source-code
```javascript
function constructor(service, state) {
  this.service = service;
  this.state = state;

  if (typeof this.state === 'object') {
    AWS.util.each.call(this, this.state, function (key, value) {
      this.state = key;
      this.expectedValue = value;
    });
  }

  this.loadWaiterConfig(this.state);
  if (!this.expectedValue) {
    this.expectedValue = this.config.successValue;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Response"></a>[function <span class="apidocSignatureSpan">s3.</span>AWS.Response (request)](#apidoc.element.s3.AWS.Response)
- description and source-code
```javascript
function Response(request) {
  this.request = request;
  this.data = null;
  this.error = null;
  this.retryCount = 0;
  this.redirectCount = 0;
  this.httpResponse = new AWS.HttpResponse();
  if (request) {
    this.maxRetries = request.service.numRetries();
    this.maxRedirects = request.service.config.maxRedirects;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Route53"></a>[function <span class="apidocSignatureSpan">s3.</span>AWS.Route53 ()](#apidoc.element.s3.AWS.Route53)
- description and source-code
```javascript
AWS.Route53 = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Route53Domains"></a>[function <span class="apidocSignatureSpan">s3.</span>AWS.Route53Domains ()](#apidoc.element.s3.AWS.Route53Domains)
- description and source-code
```javascript
AWS.Route53Domains = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.S3"></a>[function <span class="apidocSignatureSpan">s3.</span>AWS.S3 ()](#apidoc.element.s3.AWS.S3)
- description and source-code
```javascript
AWS.S3 = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.SAMLCredentials"></a>[function <span class="apidocSignatureSpan">s3.</span>AWS.SAMLCredentials (params)](#apidoc.element.s3.AWS.SAMLCredentials)
- description and source-code
```javascript
function SAMLCredentials(params) {
  AWS.Credentials.call(this);
  this.expired = true;
  this.params = params;
  this.service = new AWS.STS({params: this.params});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.SES"></a>[function <span class="apidocSignatureSpan">s3.</span>AWS.SES ()](#apidoc.element.s3.AWS.SES)
- description and source-code
```javascript
AWS.SES = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.SNS"></a>[function <span class="apidocSignatureSpan">s3.</span>AWS.SNS ()](#apidoc.element.s3.AWS.SNS)
- description and source-code
```javascript
AWS.SNS = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.SQS"></a>[function <span class="apidocSignatureSpan">s3.</span>AWS.SQS ()](#apidoc.element.s3.AWS.SQS)
- description and source-code
```javascript
AWS.SQS = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.STS"></a>[function <span class="apidocSignatureSpan">s3.</span>AWS.STS ()](#apidoc.element.s3.AWS.STS)
- description and source-code
```javascript
AWS.STS = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.SWF"></a>[function <span class="apidocSignatureSpan">s3.</span>AWS.SWF ()](#apidoc.element.s3.AWS.SWF)
- description and source-code
```javascript
AWS.SWF = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.SequentialExecutor"></a>[function <span class="apidocSignatureSpan">s3.</span>AWS.SequentialExecutor ()](#apidoc.element.s3.AWS.SequentialExecutor)
- description and source-code
```javascript
function SequentialExecutor() {
  this._events = {};
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Service"></a>[function <span class="apidocSignatureSpan">s3.</span>AWS.Service (config)](#apidoc.element.s3.AWS.Service)
- description and source-code
```javascript
function Service(config) {
  if (!this.loadServiceClass) {
    throw AWS.util.error(new Error(),
      'Service must be constructed with 'new\' operator');
  }
  var ServiceClass = this.loadServiceClass(config || {});
  if (ServiceClass) return new ServiceClass(config);
  this.initialize(config);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.SharedIniFileCredentials"></a>[function <span class="apidocSignatureSpan">s3.</span>AWS.SharedIniFileCredentials (options)](#apidoc.element.s3.AWS.SharedIniFileCredentials)
- description and source-code
```javascript
function SharedIniFileCredentials(options) {
  AWS.Credentials.call(this);

  options = options || {};

  this.filename = options.filename;
  this.profile = options.profile || process.env.AWS_PROFILE || 'default';
  this.get(function() {});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.SimpleDB"></a>[function <span class="apidocSignatureSpan">s3.</span>AWS.SimpleDB ()](#apidoc.element.s3.AWS.SimpleDB)
- description and source-code
```javascript
AWS.SimpleDB = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.StorageGateway"></a>[function <span class="apidocSignatureSpan">s3.</span>AWS.StorageGateway ()](#apidoc.element.s3.AWS.StorageGateway)
- description and source-code
```javascript
AWS.StorageGateway = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Support"></a>[function <span class="apidocSignatureSpan">s3.</span>AWS.Support ()](#apidoc.element.s3.AWS.Support)
- description and source-code
```javascript
AWS.Support = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.TemporaryCredentials"></a>[function <span class="apidocSignatureSpan">s3.</span>AWS.TemporaryCredentials (params)](#apidoc.element.s3.AWS.TemporaryCredentials)
- description and source-code
```javascript
function TemporaryCredentials(params) {
  AWS.Credentials.call(this);
  this.loadMasterCredentials();
  this.expired = true;

  this.params = params || {};
  if (this.params.RoleArn) {
    this.params.RoleSessionName =
      this.params.RoleSessionName || 'temporary-credentials';
  }
  this.service = new AWS.STS({params: this.params});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.WebIdentityCredentials"></a>[function <span class="apidocSignatureSpan">s3.</span>AWS.WebIdentityCredentials (params)](#apidoc.element.s3.AWS.WebIdentityCredentials)
- description and source-code
```javascript
function WebIdentityCredentials(params) {
  AWS.Credentials.call(this);
  this.expired = true;
  this.params = params;
  this.params.RoleSessionName = this.params.RoleSessionName || 'web-identity';
  this.service = new AWS.STS({params: this.params});
  this.data = null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.Client"></a>[function <span class="apidocSignatureSpan">s3.</span>Client (options)](#apidoc.element.s3.Client)
- description and source-code
```javascript
function Client(options) {
  options = options || {};
  this.s3 = options.s3Client || new AWS.S3(options.s3Options);
  this.s3Pend = new Pend();
  this.s3Pend.max = options.maxAsyncS3 || 20;
  this.s3RetryCount = options.s3RetryCount || 3;
  this.s3RetryDelay = options.s3RetryDelay || 1000;
  this.multipartUploadThreshold = options.multipartUploadThreshold || (20 * 1024 * 1024);
  this.multipartUploadSize = options.multipartUploadSize || (15 * 1024 * 1024);
  this.multipartDownloadThreshold = options.multipartDownloadThreshold || (20 * 1024 * 1024);
  this.multipartDownloadSize = options.multipartDownloadSize || (15 * 1024 * 1024);

  if (this.multipartUploadThreshold < MIN_MULTIPART_SIZE) {
    throw new Error("Minimum multipartUploadThreshold is 5MB.");
  }
  if (this.multipartUploadThreshold > MAX_PUTOBJECT_SIZE) {
    throw new Error("Maximum multipartUploadThreshold is 5GB.");
  }
  if (this.multipartUploadSize < MIN_MULTIPART_SIZE) {
    throw new Error("Minimum multipartUploadSize is 5MB.");
  }
  if (this.multipartUploadSize > MAX_PUTOBJECT_SIZE) {
    throw new Error("Maximum multipartUploadSize is 5GB.");
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.MultipartETag"></a>[function <span class="apidocSignatureSpan">s3.</span>MultipartETag (options)](#apidoc.element.s3.MultipartETag)
- description and source-code
```javascript
function MultipartETag(options) {
  options = options || {};
  Transform.call(this, options);
  var sizes = [
    maximumUploadSize,
    minimumUploadSize,
    commonUploadSize1,
    commonUploadSize2,
  ];
  if (options.size != null && options.count != null) {
    if (options.count === 1) {
      sizes = [maximumUploadSize];
    } else {
      sizes.push(guessPartSizeFromSizeAndCount(options.size, options.count));
    }
  }
  this.sums = [];
  this.bytes = 0;
  this.digest = null; // if it is less than maximumUploadSize
  this.done = false;
  for (var i = 0; i < sizes.length; i += 1) {
    this.sums.push({
      size: sizes[i],
      hash: crypto.createHash('md5'),
      amtWritten: 0,
      digests: [],
      eTag: null,
    });
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.createClient"></a>[function <span class="apidocSignatureSpan">s3.</span>createClient (options)](#apidoc.element.s3.createClient)
- description and source-code
```javascript
createClient = function (options) {
  return new Client(options);
}
```
- example usage
```shell
...
## Synopsis

### Create a client

'''js
var s3 = require('s3');

var client = s3.createClient({
maxAsyncS3: 20,     // this is the default
s3RetryCount: 3,    // this is the default
s3RetryDelay: 1000, // this is the default
multipartUploadThreshold: 20971520, // this is the default (20 MB)
multipartUploadSize: 15728640, // this is the default (15 MB)
s3Options: {
  accessKeyId: "your s3 key",
...
```

#### <a name="apidoc.element.s3.getPublicUrl"></a>[function <span class="apidocSignatureSpan">s3.</span>getPublicUrl (bucket, key, bucketLocation)](#apidoc.element.s3.getPublicUrl)
- description and source-code
```javascript
function getPublicUrl(bucket, key, bucketLocation) {
  var nonStandardBucketLocation = (bucketLocation && bucketLocation !== 'us-east-1');
  var hostnamePrefix = nonStandardBucketLocation ? ("s3-" + bucketLocation) : "s3";
  var parts = {
    protocol: "https:",
    hostname: hostnamePrefix + ".amazonaws.com",
    pathname: "/" + bucket + "/" + encodeSpecialCharacters(key),
  };
  return url.format(parts);
}
```
- example usage
```shell
...
  Maximum is 5GB.
* 'multipartUploadSize' - when uploading via multipart, this is the part size.
  The minimum size is 5MB. The maximum size is 5GB. Default is 15MB. Note that
  S3 has a maximum of 10000 parts for a multipart upload, so if this value is
  too small, it will be ignored in favor of the minimum necessary value
  required to upload the file.

### s3.getPublicUrl(bucket, key, [bucketLocation])

* 'bucket' S3 bucket
* 'key' S3 key
* 'bucketLocation' string, one of these:
  - "" (default) - US Standard
  - "eu-west-1"
  - "us-west-1"
...
```

#### <a name="apidoc.element.s3.getPublicUrlHttp"></a>[function <span class="apidocSignatureSpan">s3.</span>getPublicUrlHttp (bucket, key)](#apidoc.element.s3.getPublicUrlHttp)
- description and source-code
```javascript
function getPublicUrlHttp(bucket, key) {
  var parts = {
    protocol: "http:",
    hostname: bucket + ".s3.amazonaws.com",
    pathname: "/" + encodeSpecialCharacters(key),
  };
  return url.format(parts);
}
```
- example usage
```shell
...

'https://s3.amazonaws.com/bucket/key'

or maybe this if you are not in US Standard:

'https://s3-eu-west-1.amazonaws.com/bucket/key'

### s3.getPublicUrlHttp(bucket, key)

 * 'bucket' S3 Bucket
 * 'key' S3 Key

Works for any region, and returns a string which looks like this:

'http://bucket.s3.amazonaws.com/key'
...
```



# <a name="apidoc.module.s3.AWS"></a>[module s3.AWS](#apidoc.module.s3.AWS)

#### <a name="apidoc.element.s3.AWS.AutoScaling"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>AutoScaling ()](#apidoc.element.s3.AWS.AutoScaling)
- description and source-code
```javascript
AutoScaling = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.CloudFormation"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>CloudFormation ()](#apidoc.element.s3.AWS.CloudFormation)
- description and source-code
```javascript
CloudFormation = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.CloudFront"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>CloudFront ()](#apidoc.element.s3.AWS.CloudFront)
- description and source-code
```javascript
CloudFront = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.CloudSearch"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>CloudSearch ()](#apidoc.element.s3.AWS.CloudSearch)
- description and source-code
```javascript
CloudSearch = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.CloudSearchDomain"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>CloudSearchDomain ()](#apidoc.element.s3.AWS.CloudSearchDomain)
- description and source-code
```javascript
CloudSearchDomain = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.CloudTrail"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>CloudTrail ()](#apidoc.element.s3.AWS.CloudTrail)
- description and source-code
```javascript
CloudTrail = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.CloudWatch"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>CloudWatch ()](#apidoc.element.s3.AWS.CloudWatch)
- description and source-code
```javascript
CloudWatch = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.CloudWatchLogs"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>CloudWatchLogs ()](#apidoc.element.s3.AWS.CloudWatchLogs)
- description and source-code
```javascript
CloudWatchLogs = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.CodeDeploy"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>CodeDeploy ()](#apidoc.element.s3.AWS.CodeDeploy)
- description and source-code
```javascript
CodeDeploy = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.CognitoIdentity"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>CognitoIdentity ()](#apidoc.element.s3.AWS.CognitoIdentity)
- description and source-code
```javascript
CognitoIdentity = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.CognitoIdentityCredentials"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>CognitoIdentityCredentials (params)](#apidoc.element.s3.AWS.CognitoIdentityCredentials)
- description and source-code
```javascript
function CognitoIdentityCredentials(params) {
  AWS.Credentials.call(this);
  this.expired = true;
  this.webIdentityCredentials = new AWS.WebIdentityCredentials(params);
  this.cognito = new AWS.CognitoIdentity({params: params});
  this.sts = new AWS.STS();
  this.params = params;
  this.data = null;
  this.identityId = null;
  this.loadCachedId();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.CognitoSync"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>CognitoSync ()](#apidoc.element.s3.AWS.CognitoSync)
- description and source-code
```javascript
CognitoSync = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Config"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>Config (options)](#apidoc.element.s3.AWS.Config)
- description and source-code
```javascript
function Config(options) {
  if (options === undefined) options = {};
  options = this.extractCredentials(options);

  AWS.util.each.call(this, this.keys, function (key, value) {
    this.set(key, options[key], value);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.ConfigService"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>ConfigService ()](#apidoc.element.s3.AWS.ConfigService)
- description and source-code
```javascript
ConfigService = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.CredentialProviderChain"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>CredentialProviderChain (providers)](#apidoc.element.s3.AWS.CredentialProviderChain)
- description and source-code
```javascript
function CredentialProviderChain(providers) {
  if (providers) {
    this.providers = providers;
  } else {
    this.providers = AWS.CredentialProviderChain.defaultProviders.slice(0);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Credentials"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>Credentials ()](#apidoc.element.s3.AWS.Credentials)
- description and source-code
```javascript
function Credentials() {
  // hide secretAccessKey from being displayed with util.inspect
  AWS.util.hideProperties(this, ['secretAccessKey']);

  this.expired = false;
  this.expireTime = null;
  if (arguments.length === 1 && typeof arguments[0] === 'object') {
    var creds = arguments[0].credentials || arguments[0];
    this.accessKeyId = creds.accessKeyId;
    this.secretAccessKey = creds.secretAccessKey;
    this.sessionToken = creds.sessionToken;
  } else {
    this.accessKeyId = arguments[0];
    this.secretAccessKey = arguments[1];
    this.sessionToken = arguments[2];
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.DataPipeline"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>DataPipeline ()](#apidoc.element.s3.AWS.DataPipeline)
- description and source-code
```javascript
DataPipeline = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.DirectConnect"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>DirectConnect ()](#apidoc.element.s3.AWS.DirectConnect)
- description and source-code
```javascript
DirectConnect = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.DynamoDB"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>DynamoDB ()](#apidoc.element.s3.AWS.DynamoDB)
- description and source-code
```javascript
DynamoDB = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.EC2"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>EC2 ()](#apidoc.element.s3.AWS.EC2)
- description and source-code
```javascript
EC2 = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.EC2MetadataCredentials"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>EC2MetadataCredentials (options)](#apidoc.element.s3.AWS.EC2MetadataCredentials)
- description and source-code
```javascript
function EC2MetadataCredentials(options) {
  AWS.Credentials.call(this);

  options = options ? AWS.util.copy(options) : {};
  if (!options.httpOptions) options.httpOptions = {};
  options.httpOptions = AWS.util.merge(
    {timeout: this.defaultTimeout}, options.httpOptions);

  this.metadataService = new AWS.MetadataService(options);
  this.metadata = {};
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.ELB"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>ELB ()](#apidoc.element.s3.AWS.ELB)
- description and source-code
```javascript
ELB = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.EMR"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>EMR ()](#apidoc.element.s3.AWS.EMR)
- description and source-code
```javascript
EMR = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.ElastiCache"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>ElastiCache ()](#apidoc.element.s3.AWS.ElastiCache)
- description and source-code
```javascript
ElastiCache = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.ElasticBeanstalk"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>ElasticBeanstalk ()](#apidoc.element.s3.AWS.ElasticBeanstalk)
- description and source-code
```javascript
ElasticBeanstalk = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.ElasticTranscoder"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>ElasticTranscoder ()](#apidoc.element.s3.AWS.ElasticTranscoder)
- description and source-code
```javascript
ElasticTranscoder = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Endpoint"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>Endpoint (endpoint, config)](#apidoc.element.s3.AWS.Endpoint)
- description and source-code
```javascript
function Endpoint(endpoint, config) {
  AWS.util.hideProperties(this, ['slashes', 'auth', 'hash', 'search', 'query']);

  if (typeof endpoint === 'undefined' || endpoint === null) {
    throw new Error('Invalid endpoint: ' + endpoint);
  } else if (typeof endpoint !== 'string') {
    return AWS.util.copy(endpoint);
  }

  if (!endpoint.match(/^http/)) {
    var useSSL = config && config.sslEnabled !== undefined ?
      config.sslEnabled : AWS.config.sslEnabled;
    endpoint = (useSSL ? 'https' : 'http') + '://' + endpoint;
  }

  AWS.util.update(this, AWS.util.urlParse(endpoint));

  // Ensure the port property is set as an integer
  if (this.port) {
    this.port = parseInt(this.port, 10);
  } else {
    this.port = this.protocol === 'https:' ? 443 : 80;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.EnvironmentCredentials"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>EnvironmentCredentials (envPrefix)](#apidoc.element.s3.AWS.EnvironmentCredentials)
- description and source-code
```javascript
function EnvironmentCredentials(envPrefix) {
  AWS.Credentials.call(this);
  this.envPrefix = envPrefix;
  this.get(function() {});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.FileSystemCredentials"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>FileSystemCredentials (filename)](#apidoc.element.s3.AWS.FileSystemCredentials)
- description and source-code
```javascript
function FileSystemCredentials(filename) {
  AWS.Credentials.call(this);
  this.filename = filename;
  this.get(function() {});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Glacier"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>Glacier ()](#apidoc.element.s3.AWS.Glacier)
- description and source-code
```javascript
Glacier = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.HttpClient"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>HttpClient ()](#apidoc.element.s3.AWS.HttpClient)
- description and source-code
```javascript
HttpClient = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.HttpRequest"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>HttpRequest (endpoint, region)](#apidoc.element.s3.AWS.HttpRequest)
- description and source-code
```javascript
function HttpRequest(endpoint, region) {
  endpoint = new AWS.Endpoint(endpoint);
  this.method = 'POST';
  this.path = endpoint.path || '/';
  this.headers = {};
  this.body = '';
  this.endpoint = endpoint;
  this.region = region;
  this.setUserAgent();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.HttpResponse"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>HttpResponse ()](#apidoc.element.s3.AWS.HttpResponse)
- description and source-code
```javascript
function HttpResponse() {
  this.statusCode = undefined;
  this.headers = {};
  this.body = undefined;
  this.streaming = false;
  this.stream = null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.IAM"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>IAM ()](#apidoc.element.s3.AWS.IAM)
- description and source-code
```javascript
IAM = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.ImportExport"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>ImportExport ()](#apidoc.element.s3.AWS.ImportExport)
- description and source-code
```javascript
ImportExport = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.KMS"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>KMS ()](#apidoc.element.s3.AWS.KMS)
- description and source-code
```javascript
KMS = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Kinesis"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>Kinesis ()](#apidoc.element.s3.AWS.Kinesis)
- description and source-code
```javascript
Kinesis = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Lambda"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>Lambda ()](#apidoc.element.s3.AWS.Lambda)
- description and source-code
```javascript
Lambda = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.MetadataService"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>MetadataService (options)](#apidoc.element.s3.AWS.MetadataService)
- description and source-code
```javascript
function MetadataService(options) {
  AWS.util.update(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.NodeHttpClient"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>NodeHttpClient ()](#apidoc.element.s3.AWS.NodeHttpClient)
- description and source-code
```javascript
NodeHttpClient = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.OpsWorks"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>OpsWorks ()](#apidoc.element.s3.AWS.OpsWorks)
- description and source-code
```javascript
OpsWorks = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.ParamValidator"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>ParamValidator ()](#apidoc.element.s3.AWS.ParamValidator)
- description and source-code
```javascript
ParamValidator = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.RDS"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>RDS ()](#apidoc.element.s3.AWS.RDS)
- description and source-code
```javascript
RDS = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Redshift"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>Redshift ()](#apidoc.element.s3.AWS.Redshift)
- description and source-code
```javascript
Redshift = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Request"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>Request (service, operation, params)](#apidoc.element.s3.AWS.Request)
- description and source-code
```javascript
function Request(service, operation, params) {
  var endpoint = service.endpoint;
  var region = service.config.region;

  // global endpoints sign as us-east-1
  if (service.isGlobalEndpoint) region = 'us-east-1';

  this.domain = domain && domain.active;
  this.service = service;
  this.operation = operation;
  this.params = params || {};
  this.httpRequest = new AWS.HttpRequest(endpoint, region);
  this.startTime = AWS.util.date.getDate();

  this.response = new AWS.Response(this);
  this._asm = new AcceptorStateMachine(fsm.states, 'validate');

  AWS.SequentialExecutor.call(this);
  this.emit = this.emitEvent;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.ResourceWaiter"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>ResourceWaiter (service, state)](#apidoc.element.s3.AWS.ResourceWaiter)
- description and source-code
```javascript
function constructor(service, state) {
  this.service = service;
  this.state = state;

  if (typeof this.state === 'object') {
    AWS.util.each.call(this, this.state, function (key, value) {
      this.state = key;
      this.expectedValue = value;
    });
  }

  this.loadWaiterConfig(this.state);
  if (!this.expectedValue) {
    this.expectedValue = this.config.successValue;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Response"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>Response (request)](#apidoc.element.s3.AWS.Response)
- description and source-code
```javascript
function Response(request) {
  this.request = request;
  this.data = null;
  this.error = null;
  this.retryCount = 0;
  this.redirectCount = 0;
  this.httpResponse = new AWS.HttpResponse();
  if (request) {
    this.maxRetries = request.service.numRetries();
    this.maxRedirects = request.service.config.maxRedirects;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Route53"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>Route53 ()](#apidoc.element.s3.AWS.Route53)
- description and source-code
```javascript
Route53 = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Route53Domains"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>Route53Domains ()](#apidoc.element.s3.AWS.Route53Domains)
- description and source-code
```javascript
Route53Domains = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.S3"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>S3 ()](#apidoc.element.s3.AWS.S3)
- description and source-code
```javascript
S3 = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
...
  s3RetryCount: 3,    // this is the default
  s3RetryDelay: 1000, // this is the default
  multipartUploadThreshold: 20971520, // this is the default (20 MB)
  multipartUploadSize: 15728640, // this is the default (15 MB)
  s3Options: {
    accessKeyId: "your s3 key",
    secretAccessKey: "your s3 secret",
    // any other options are passed to new AWS.S3()
    // See: http://docs.aws.amazon.com/AWSJavaScriptSDK/latest/AWS/Config.html#constructor-property
  },
});
'''

### Create a client from existing AWS.S3 object
...
```

#### <a name="apidoc.element.s3.AWS.SAMLCredentials"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>SAMLCredentials (params)](#apidoc.element.s3.AWS.SAMLCredentials)
- description and source-code
```javascript
function SAMLCredentials(params) {
  AWS.Credentials.call(this);
  this.expired = true;
  this.params = params;
  this.service = new AWS.STS({params: this.params});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.SES"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>SES ()](#apidoc.element.s3.AWS.SES)
- description and source-code
```javascript
SES = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.SNS"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>SNS ()](#apidoc.element.s3.AWS.SNS)
- description and source-code
```javascript
SNS = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.SQS"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>SQS ()](#apidoc.element.s3.AWS.SQS)
- description and source-code
```javascript
SQS = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.STS"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>STS ()](#apidoc.element.s3.AWS.STS)
- description and source-code
```javascript
STS = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.SWF"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>SWF ()](#apidoc.element.s3.AWS.SWF)
- description and source-code
```javascript
SWF = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.SequentialExecutor"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>SequentialExecutor ()](#apidoc.element.s3.AWS.SequentialExecutor)
- description and source-code
```javascript
function SequentialExecutor() {
  this._events = {};
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Service"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>Service (config)](#apidoc.element.s3.AWS.Service)
- description and source-code
```javascript
function Service(config) {
  if (!this.loadServiceClass) {
    throw AWS.util.error(new Error(),
      'Service must be constructed with 'new\' operator');
  }
  var ServiceClass = this.loadServiceClass(config || {});
  if (ServiceClass) return new ServiceClass(config);
  this.initialize(config);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.SharedIniFileCredentials"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>SharedIniFileCredentials (options)](#apidoc.element.s3.AWS.SharedIniFileCredentials)
- description and source-code
```javascript
function SharedIniFileCredentials(options) {
  AWS.Credentials.call(this);

  options = options || {};

  this.filename = options.filename;
  this.profile = options.profile || process.env.AWS_PROFILE || 'default';
  this.get(function() {});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.SimpleDB"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>SimpleDB ()](#apidoc.element.s3.AWS.SimpleDB)
- description and source-code
```javascript
SimpleDB = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.StorageGateway"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>StorageGateway ()](#apidoc.element.s3.AWS.StorageGateway)
- description and source-code
```javascript
StorageGateway = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Support"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>Support ()](#apidoc.element.s3.AWS.Support)
- description and source-code
```javascript
Support = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.TemporaryCredentials"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>TemporaryCredentials (params)](#apidoc.element.s3.AWS.TemporaryCredentials)
- description and source-code
```javascript
function TemporaryCredentials(params) {
  AWS.Credentials.call(this);
  this.loadMasterCredentials();
  this.expired = true;

  this.params = params || {};
  if (this.params.RoleArn) {
    this.params.RoleSessionName =
      this.params.RoleSessionName || 'temporary-credentials';
  }
  this.service = new AWS.STS({params: this.params});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.WebIdentityCredentials"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>WebIdentityCredentials (params)](#apidoc.element.s3.AWS.WebIdentityCredentials)
- description and source-code
```javascript
function WebIdentityCredentials(params) {
  AWS.Credentials.call(this);
  this.expired = true;
  this.params = params;
  this.params.RoleSessionName = this.params.RoleSessionName || 'web-identity';
  this.service = new AWS.STS({params: this.params});
  this.data = null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.apiLoader"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>apiLoader (svc, version)](#apidoc.element.s3.AWS.apiLoader)
- description and source-code
```javascript
function load(svc, version) {
  buildServiceMap();
  svc = serviceIdentifier(svc);
  if (version === 'latest') version = null;
  version = version || serviceMap[svc].versions[serviceMap[svc].versions.length - 1];
  if (!serviceMap[svc]) return null;

  var api = require(serviceFile(svc, version));

  // Try to load paginators
  if (fs.existsSync(paginatorsFile(svc, version))) {
    var paginators = require(paginatorsFile(svc, version));
    api.paginators = paginators.pagination;
  }

  // Try to load waiters
  if (fs.existsSync(waitersFile(svc, version))) {
    var waiters = require(waitersFile(svc, version));
    api.waiters = waiters.waiters;
  }

  return api;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.AutoScaling"></a>[module s3.AWS.AutoScaling](#apidoc.module.s3.AWS.AutoScaling)

#### <a name="apidoc.element.s3.AWS.AutoScaling.AutoScaling"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>AutoScaling ()](#apidoc.element.s3.AWS.AutoScaling.AutoScaling)
- description and source-code
```javascript
AutoScaling = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.AutoScaling.__super__"></a>[function <span class="apidocSignatureSpan">s3.AWS.AutoScaling.</span>__super__ (config)](#apidoc.element.s3.AWS.AutoScaling.__super__)
- description and source-code
```javascript
function Service(config) {
  if (!this.loadServiceClass) {
    throw AWS.util.error(new Error(),
      'Service must be constructed with 'new\' operator');
  }
  var ServiceClass = this.loadServiceClass(config || {});
  if (ServiceClass) return new ServiceClass(config);
  this.initialize(config);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.AutoScaling.prototype"></a>[module s3.AWS.AutoScaling.prototype](#apidoc.module.s3.AWS.AutoScaling.prototype)

#### <a name="apidoc.element.s3.AWS.AutoScaling.prototype.constructor"></a>[function <span class="apidocSignatureSpan">s3.AWS.AutoScaling.prototype.</span>constructor ()](#apidoc.element.s3.AWS.AutoScaling.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.CloudFormation"></a>[module s3.AWS.CloudFormation](#apidoc.module.s3.AWS.CloudFormation)

#### <a name="apidoc.element.s3.AWS.CloudFormation.CloudFormation"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>CloudFormation ()](#apidoc.element.s3.AWS.CloudFormation.CloudFormation)
- description and source-code
```javascript
CloudFormation = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.CloudFormation.__super__"></a>[function <span class="apidocSignatureSpan">s3.AWS.CloudFormation.</span>__super__ (config)](#apidoc.element.s3.AWS.CloudFormation.__super__)
- description and source-code
```javascript
function Service(config) {
  if (!this.loadServiceClass) {
    throw AWS.util.error(new Error(),
      'Service must be constructed with 'new\' operator');
  }
  var ServiceClass = this.loadServiceClass(config || {});
  if (ServiceClass) return new ServiceClass(config);
  this.initialize(config);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.CloudFormation.prototype"></a>[module s3.AWS.CloudFormation.prototype](#apidoc.module.s3.AWS.CloudFormation.prototype)

#### <a name="apidoc.element.s3.AWS.CloudFormation.prototype.constructor"></a>[function <span class="apidocSignatureSpan">s3.AWS.CloudFormation.prototype.</span>constructor ()](#apidoc.element.s3.AWS.CloudFormation.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.CloudFront"></a>[module s3.AWS.CloudFront](#apidoc.module.s3.AWS.CloudFront)

#### <a name="apidoc.element.s3.AWS.CloudFront.CloudFront"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>CloudFront ()](#apidoc.element.s3.AWS.CloudFront.CloudFront)
- description and source-code
```javascript
CloudFront = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.CloudFront.__super__"></a>[function <span class="apidocSignatureSpan">s3.AWS.CloudFront.</span>__super__ (config)](#apidoc.element.s3.AWS.CloudFront.__super__)
- description and source-code
```javascript
function Service(config) {
  if (!this.loadServiceClass) {
    throw AWS.util.error(new Error(),
      'Service must be constructed with 'new\' operator');
  }
  var ServiceClass = this.loadServiceClass(config || {});
  if (ServiceClass) return new ServiceClass(config);
  this.initialize(config);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.CloudFront.prototype"></a>[module s3.AWS.CloudFront.prototype](#apidoc.module.s3.AWS.CloudFront.prototype)

#### <a name="apidoc.element.s3.AWS.CloudFront.prototype.constructor"></a>[function <span class="apidocSignatureSpan">s3.AWS.CloudFront.prototype.</span>constructor ()](#apidoc.element.s3.AWS.CloudFront.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.CloudSearch"></a>[module s3.AWS.CloudSearch](#apidoc.module.s3.AWS.CloudSearch)

#### <a name="apidoc.element.s3.AWS.CloudSearch.CloudSearch"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>CloudSearch ()](#apidoc.element.s3.AWS.CloudSearch.CloudSearch)
- description and source-code
```javascript
CloudSearch = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.CloudSearch.__super__"></a>[function <span class="apidocSignatureSpan">s3.AWS.CloudSearch.</span>__super__ (config)](#apidoc.element.s3.AWS.CloudSearch.__super__)
- description and source-code
```javascript
function Service(config) {
  if (!this.loadServiceClass) {
    throw AWS.util.error(new Error(),
      'Service must be constructed with 'new\' operator');
  }
  var ServiceClass = this.loadServiceClass(config || {});
  if (ServiceClass) return new ServiceClass(config);
  this.initialize(config);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.CloudSearch.prototype"></a>[module s3.AWS.CloudSearch.prototype](#apidoc.module.s3.AWS.CloudSearch.prototype)

#### <a name="apidoc.element.s3.AWS.CloudSearch.prototype.constructor"></a>[function <span class="apidocSignatureSpan">s3.AWS.CloudSearch.prototype.</span>constructor ()](#apidoc.element.s3.AWS.CloudSearch.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.CloudSearchDomain"></a>[module s3.AWS.CloudSearchDomain](#apidoc.module.s3.AWS.CloudSearchDomain)

#### <a name="apidoc.element.s3.AWS.CloudSearchDomain.CloudSearchDomain"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>CloudSearchDomain ()](#apidoc.element.s3.AWS.CloudSearchDomain.CloudSearchDomain)
- description and source-code
```javascript
CloudSearchDomain = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.CloudSearchDomain.__super__"></a>[function <span class="apidocSignatureSpan">s3.AWS.CloudSearchDomain.</span>__super__ (config)](#apidoc.element.s3.AWS.CloudSearchDomain.__super__)
- description and source-code
```javascript
function Service(config) {
  if (!this.loadServiceClass) {
    throw AWS.util.error(new Error(),
      'Service must be constructed with 'new\' operator');
  }
  var ServiceClass = this.loadServiceClass(config || {});
  if (ServiceClass) return new ServiceClass(config);
  this.initialize(config);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.CloudSearchDomain.prototype"></a>[module s3.AWS.CloudSearchDomain.prototype](#apidoc.module.s3.AWS.CloudSearchDomain.prototype)

#### <a name="apidoc.element.s3.AWS.CloudSearchDomain.prototype.constructor"></a>[function <span class="apidocSignatureSpan">s3.AWS.CloudSearchDomain.prototype.</span>constructor ()](#apidoc.element.s3.AWS.CloudSearchDomain.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.CloudSearchDomain.prototype.setupRequestListeners"></a>[function <span class="apidocSignatureSpan">s3.AWS.CloudSearchDomain.prototype.</span>setupRequestListeners (request)](#apidoc.element.s3.AWS.CloudSearchDomain.prototype.setupRequestListeners)
- description and source-code
```javascript
function setupRequestListeners(request) {
  if (!request.service.config.credentials) {
    request.removeListener('validate',
                           AWS.EventListeners.Core.VALIDATE_CREDENTIALS
                          );
    request.removeListener('sign', AWS.EventListeners.Core.SIGN);
  } else {
    request.addListener('validate', this.updateRegion);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.CloudSearchDomain.prototype.updateRegion"></a>[function <span class="apidocSignatureSpan">s3.AWS.CloudSearchDomain.prototype.</span>updateRegion (request)](#apidoc.element.s3.AWS.CloudSearchDomain.prototype.updateRegion)
- description and source-code
```javascript
function updateRegion(request) {
  var endpoint = request.httpRequest.endpoint.hostname;
  var zones = endpoint.split('.');
  request.httpRequest.region = zones[1] || request.httpRequest.region;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.CloudSearchDomain.prototype.validateService"></a>[function <span class="apidocSignatureSpan">s3.AWS.CloudSearchDomain.prototype.</span>validateService ()](#apidoc.element.s3.AWS.CloudSearchDomain.prototype.validateService)
- description and source-code
```javascript
function validateService() {
  if (!this.config.endpoint || this.config.endpoint.indexOf('{') >= 0) {
    var msg = 'AWS.CloudSearchDomain requires an explicit ' +
              ''endpoint\' configuration option.';
    throw AWS.util.error(new Error(),
      {name: 'InvalidEndpoint', message: msg});
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.CloudTrail"></a>[module s3.AWS.CloudTrail](#apidoc.module.s3.AWS.CloudTrail)

#### <a name="apidoc.element.s3.AWS.CloudTrail.CloudTrail"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>CloudTrail ()](#apidoc.element.s3.AWS.CloudTrail.CloudTrail)
- description and source-code
```javascript
CloudTrail = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.CloudTrail.__super__"></a>[function <span class="apidocSignatureSpan">s3.AWS.CloudTrail.</span>__super__ (config)](#apidoc.element.s3.AWS.CloudTrail.__super__)
- description and source-code
```javascript
function Service(config) {
  if (!this.loadServiceClass) {
    throw AWS.util.error(new Error(),
      'Service must be constructed with 'new\' operator');
  }
  var ServiceClass = this.loadServiceClass(config || {});
  if (ServiceClass) return new ServiceClass(config);
  this.initialize(config);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.CloudTrail.prototype"></a>[module s3.AWS.CloudTrail.prototype](#apidoc.module.s3.AWS.CloudTrail.prototype)

#### <a name="apidoc.element.s3.AWS.CloudTrail.prototype.constructor"></a>[function <span class="apidocSignatureSpan">s3.AWS.CloudTrail.prototype.</span>constructor ()](#apidoc.element.s3.AWS.CloudTrail.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.CloudWatch"></a>[module s3.AWS.CloudWatch](#apidoc.module.s3.AWS.CloudWatch)

#### <a name="apidoc.element.s3.AWS.CloudWatch.CloudWatch"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>CloudWatch ()](#apidoc.element.s3.AWS.CloudWatch.CloudWatch)
- description and source-code
```javascript
CloudWatch = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.CloudWatch.__super__"></a>[function <span class="apidocSignatureSpan">s3.AWS.CloudWatch.</span>__super__ (config)](#apidoc.element.s3.AWS.CloudWatch.__super__)
- description and source-code
```javascript
function Service(config) {
  if (!this.loadServiceClass) {
    throw AWS.util.error(new Error(),
      'Service must be constructed with 'new\' operator');
  }
  var ServiceClass = this.loadServiceClass(config || {});
  if (ServiceClass) return new ServiceClass(config);
  this.initialize(config);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.CloudWatch.prototype"></a>[module s3.AWS.CloudWatch.prototype](#apidoc.module.s3.AWS.CloudWatch.prototype)

#### <a name="apidoc.element.s3.AWS.CloudWatch.prototype.constructor"></a>[function <span class="apidocSignatureSpan">s3.AWS.CloudWatch.prototype.</span>constructor ()](#apidoc.element.s3.AWS.CloudWatch.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.CloudWatchLogs"></a>[module s3.AWS.CloudWatchLogs](#apidoc.module.s3.AWS.CloudWatchLogs)

#### <a name="apidoc.element.s3.AWS.CloudWatchLogs.CloudWatchLogs"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>CloudWatchLogs ()](#apidoc.element.s3.AWS.CloudWatchLogs.CloudWatchLogs)
- description and source-code
```javascript
CloudWatchLogs = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.CloudWatchLogs.__super__"></a>[function <span class="apidocSignatureSpan">s3.AWS.CloudWatchLogs.</span>__super__ (config)](#apidoc.element.s3.AWS.CloudWatchLogs.__super__)
- description and source-code
```javascript
function Service(config) {
  if (!this.loadServiceClass) {
    throw AWS.util.error(new Error(),
      'Service must be constructed with 'new\' operator');
  }
  var ServiceClass = this.loadServiceClass(config || {});
  if (ServiceClass) return new ServiceClass(config);
  this.initialize(config);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.CloudWatchLogs.prototype"></a>[module s3.AWS.CloudWatchLogs.prototype](#apidoc.module.s3.AWS.CloudWatchLogs.prototype)

#### <a name="apidoc.element.s3.AWS.CloudWatchLogs.prototype.constructor"></a>[function <span class="apidocSignatureSpan">s3.AWS.CloudWatchLogs.prototype.</span>constructor ()](#apidoc.element.s3.AWS.CloudWatchLogs.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.CodeDeploy"></a>[module s3.AWS.CodeDeploy](#apidoc.module.s3.AWS.CodeDeploy)

#### <a name="apidoc.element.s3.AWS.CodeDeploy.CodeDeploy"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>CodeDeploy ()](#apidoc.element.s3.AWS.CodeDeploy.CodeDeploy)
- description and source-code
```javascript
CodeDeploy = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.CodeDeploy.__super__"></a>[function <span class="apidocSignatureSpan">s3.AWS.CodeDeploy.</span>__super__ (config)](#apidoc.element.s3.AWS.CodeDeploy.__super__)
- description and source-code
```javascript
function Service(config) {
  if (!this.loadServiceClass) {
    throw AWS.util.error(new Error(),
      'Service must be constructed with 'new\' operator');
  }
  var ServiceClass = this.loadServiceClass(config || {});
  if (ServiceClass) return new ServiceClass(config);
  this.initialize(config);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.CodeDeploy.prototype"></a>[module s3.AWS.CodeDeploy.prototype](#apidoc.module.s3.AWS.CodeDeploy.prototype)

#### <a name="apidoc.element.s3.AWS.CodeDeploy.prototype.constructor"></a>[function <span class="apidocSignatureSpan">s3.AWS.CodeDeploy.prototype.</span>constructor ()](#apidoc.element.s3.AWS.CodeDeploy.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.CognitoIdentity"></a>[module s3.AWS.CognitoIdentity](#apidoc.module.s3.AWS.CognitoIdentity)

#### <a name="apidoc.element.s3.AWS.CognitoIdentity.CognitoIdentity"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>CognitoIdentity ()](#apidoc.element.s3.AWS.CognitoIdentity.CognitoIdentity)
- description and source-code
```javascript
CognitoIdentity = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.CognitoIdentity.__super__"></a>[function <span class="apidocSignatureSpan">s3.AWS.CognitoIdentity.</span>__super__ (config)](#apidoc.element.s3.AWS.CognitoIdentity.__super__)
- description and source-code
```javascript
function Service(config) {
  if (!this.loadServiceClass) {
    throw AWS.util.error(new Error(),
      'Service must be constructed with 'new\' operator');
  }
  var ServiceClass = this.loadServiceClass(config || {});
  if (ServiceClass) return new ServiceClass(config);
  this.initialize(config);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.CognitoIdentity.prototype"></a>[module s3.AWS.CognitoIdentity.prototype](#apidoc.module.s3.AWS.CognitoIdentity.prototype)

#### <a name="apidoc.element.s3.AWS.CognitoIdentity.prototype.constructor"></a>[function <span class="apidocSignatureSpan">s3.AWS.CognitoIdentity.prototype.</span>constructor ()](#apidoc.element.s3.AWS.CognitoIdentity.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.CognitoIdentity.prototype.getId"></a>[function <span class="apidocSignatureSpan">s3.AWS.CognitoIdentity.prototype.</span>getId (params, callback)](#apidoc.element.s3.AWS.CognitoIdentity.prototype.getId)
- description and source-code
```javascript
function getId(params, callback) {
  return this.makeUnauthenticatedRequest('getId', params, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.CognitoIdentity.prototype.getOpenIdToken"></a>[function <span class="apidocSignatureSpan">s3.AWS.CognitoIdentity.prototype.</span>getOpenIdToken (params, callback)](#apidoc.element.s3.AWS.CognitoIdentity.prototype.getOpenIdToken)
- description and source-code
```javascript
function getOpenIdToken(params, callback) {
  return this.makeUnauthenticatedRequest('getOpenIdToken', params, callback);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.CognitoIdentityCredentials"></a>[module s3.AWS.CognitoIdentityCredentials](#apidoc.module.s3.AWS.CognitoIdentityCredentials)

#### <a name="apidoc.element.s3.AWS.CognitoIdentityCredentials.CognitoIdentityCredentials"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>CognitoIdentityCredentials (params)](#apidoc.element.s3.AWS.CognitoIdentityCredentials.CognitoIdentityCredentials)
- description and source-code
```javascript
function CognitoIdentityCredentials(params) {
  AWS.Credentials.call(this);
  this.expired = true;
  this.webIdentityCredentials = new AWS.WebIdentityCredentials(params);
  this.cognito = new AWS.CognitoIdentity({params: params});
  this.sts = new AWS.STS();
  this.params = params;
  this.data = null;
  this.identityId = null;
  this.loadCachedId();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.CognitoIdentityCredentials.__super__"></a>[function <span class="apidocSignatureSpan">s3.AWS.CognitoIdentityCredentials.</span>__super__ ()](#apidoc.element.s3.AWS.CognitoIdentityCredentials.__super__)
- description and source-code
```javascript
function Credentials() {
  // hide secretAccessKey from being displayed with util.inspect
  AWS.util.hideProperties(this, ['secretAccessKey']);

  this.expired = false;
  this.expireTime = null;
  if (arguments.length === 1 && typeof arguments[0] === 'object') {
    var creds = arguments[0].credentials || arguments[0];
    this.accessKeyId = creds.accessKeyId;
    this.secretAccessKey = creds.secretAccessKey;
    this.sessionToken = creds.sessionToken;
  } else {
    this.accessKeyId = arguments[0];
    this.secretAccessKey = arguments[1];
    this.sessionToken = arguments[2];
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.CognitoIdentityCredentials.prototype"></a>[module s3.AWS.CognitoIdentityCredentials.prototype](#apidoc.module.s3.AWS.CognitoIdentityCredentials.prototype)

#### <a name="apidoc.element.s3.AWS.CognitoIdentityCredentials.prototype.cacheId"></a>[function <span class="apidocSignatureSpan">s3.AWS.CognitoIdentityCredentials.prototype.</span>cacheId (data)](#apidoc.element.s3.AWS.CognitoIdentityCredentials.prototype.cacheId)
- description and source-code
```javascript
function cacheId(data) {
  this.identityId = data.IdentityId;
  this.params.IdentityId = this.identityId;

  // cache this IdentityId in browser localStorage if possible
  if (AWS.util.isBrowser()) {
    this.setStorage('id', data.IdentityId);

    if (this.params.Logins) {
      this.setStorage('providers', Object.keys(this.params.Logins).join(','));
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.CognitoIdentityCredentials.prototype.clearCachedId"></a>[function <span class="apidocSignatureSpan">s3.AWS.CognitoIdentityCredentials.prototype.</span>clearCachedId ()](#apidoc.element.s3.AWS.CognitoIdentityCredentials.prototype.clearCachedId)
- description and source-code
```javascript
function clearCache() {
  var poolId = this.params.IdentityPoolId;
  delete this.storage[this.localStorageKey.id + poolId];
  delete this.storage[this.localStorageKey.providers + poolId];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.CognitoIdentityCredentials.prototype.constructor"></a>[function <span class="apidocSignatureSpan">s3.AWS.CognitoIdentityCredentials.prototype.</span>constructor (params)](#apidoc.element.s3.AWS.CognitoIdentityCredentials.prototype.constructor)
- description and source-code
```javascript
function CognitoIdentityCredentials(params) {
  AWS.Credentials.call(this);
  this.expired = true;
  this.webIdentityCredentials = new AWS.WebIdentityCredentials(params);
  this.cognito = new AWS.CognitoIdentity({params: params});
  this.sts = new AWS.STS();
  this.params = params;
  this.data = null;
  this.identityId = null;
  this.loadCachedId();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.CognitoIdentityCredentials.prototype.getId"></a>[function <span class="apidocSignatureSpan">s3.AWS.CognitoIdentityCredentials.prototype.</span>getId (callback)](#apidoc.element.s3.AWS.CognitoIdentityCredentials.prototype.getId)
- description and source-code
```javascript
function getId(callback) {
  var self = this;
  if (typeof self.params.IdentityId === 'string') {
    return callback(null, self.params.IdentityId);
  }

  self.cognito.getId(function(err, data) {
    if (!err && data.IdentityId) {
      self.params.IdentityId = data.IdentityId;
      callback(null, data.IdentityId);
    } else {
      callback(err);
    }
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.CognitoIdentityCredentials.prototype.getStorage"></a>[function <span class="apidocSignatureSpan">s3.AWS.CognitoIdentityCredentials.prototype.</span>getStorage (key)](#apidoc.element.s3.AWS.CognitoIdentityCredentials.prototype.getStorage)
- description and source-code
```javascript
function getStorage(key) {
  return this.storage[this.localStorageKey[key] + this.params.IdentityPoolId];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.CognitoIdentityCredentials.prototype.loadCachedId"></a>[function <span class="apidocSignatureSpan">s3.AWS.CognitoIdentityCredentials.prototype.</span>loadCachedId ()](#apidoc.element.s3.AWS.CognitoIdentityCredentials.prototype.loadCachedId)
- description and source-code
```javascript
function loadCachedId() {
  var self = this;

  // in the browser we source default IdentityId from localStorage
  if (AWS.util.isBrowser() && !self.params.IdentityId) {
    var id = self.getStorage('id');
    if (id && self.params.Logins) {
      var actualProviders = Object.keys(self.params.Logins);
      var cachedProviders =
        (self.getStorage('providers') || '').split(',');

      // only load ID if at least one provider used this ID before
      var intersect = cachedProviders.filter(function(n) {
        return actualProviders.indexOf(n) !== -1;
      });
      if (intersect.length !== 0) {
        self.params.IdentityId = id;
      }
    } else if (id) {
      self.params.IdentityId = id;
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.CognitoIdentityCredentials.prototype.refresh"></a>[function <span class="apidocSignatureSpan">s3.AWS.CognitoIdentityCredentials.prototype.</span>refresh (callback)](#apidoc.element.s3.AWS.CognitoIdentityCredentials.prototype.refresh)
- description and source-code
```javascript
function refresh(callback) {
  var self = this;
  self.data = null;
  self.identityId = null;
  self.getId(function(err) {
    if (!err) {
      self.cognito.getOpenIdToken(function(cogErr, data) {
        if (!cogErr) {
          self.cacheId(data);
          self.params.WebIdentityToken = data.Token;
          self.webIdentityCredentials.refresh(function(webErr) {
            if (!webErr) {
              self.data = self.webIdentityCredentials.data;
              self.sts.credentialsFrom(self.data, self);
            } else {
              self.clearCachedId();
            }
            callback(webErr);
          });
        } else {
          self.clearCachedId();
          callback(cogErr);
        }
      });
    } else {
      self.clearCachedId();
      callback(err);
    }
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.CognitoIdentityCredentials.prototype.setStorage"></a>[function <span class="apidocSignatureSpan">s3.AWS.CognitoIdentityCredentials.prototype.</span>setStorage (key, val)](#apidoc.element.s3.AWS.CognitoIdentityCredentials.prototype.setStorage)
- description and source-code
```javascript
function setStorage(key, val) {
  this.storage[this.localStorageKey[key] + this.params.IdentityPoolId] = val;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.CognitoSync"></a>[module s3.AWS.CognitoSync](#apidoc.module.s3.AWS.CognitoSync)

#### <a name="apidoc.element.s3.AWS.CognitoSync.CognitoSync"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>CognitoSync ()](#apidoc.element.s3.AWS.CognitoSync.CognitoSync)
- description and source-code
```javascript
CognitoSync = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.CognitoSync.__super__"></a>[function <span class="apidocSignatureSpan">s3.AWS.CognitoSync.</span>__super__ (config)](#apidoc.element.s3.AWS.CognitoSync.__super__)
- description and source-code
```javascript
function Service(config) {
  if (!this.loadServiceClass) {
    throw AWS.util.error(new Error(),
      'Service must be constructed with 'new\' operator');
  }
  var ServiceClass = this.loadServiceClass(config || {});
  if (ServiceClass) return new ServiceClass(config);
  this.initialize(config);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.CognitoSync.prototype"></a>[module s3.AWS.CognitoSync.prototype](#apidoc.module.s3.AWS.CognitoSync.prototype)

#### <a name="apidoc.element.s3.AWS.CognitoSync.prototype.constructor"></a>[function <span class="apidocSignatureSpan">s3.AWS.CognitoSync.prototype.</span>constructor ()](#apidoc.element.s3.AWS.CognitoSync.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.Config"></a>[module s3.AWS.Config](#apidoc.module.s3.AWS.Config)

#### <a name="apidoc.element.s3.AWS.Config.Config"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>Config (options)](#apidoc.element.s3.AWS.Config.Config)
- description and source-code
```javascript
function Config(options) {
  if (options === undefined) options = {};
  options = this.extractCredentials(options);

  AWS.util.each.call(this, this.keys, function (key, value) {
    this.set(key, options[key], value);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Config.__super__"></a>[function <span class="apidocSignatureSpan">s3.AWS.Config.</span>__super__ ()](#apidoc.element.s3.AWS.Config.__super__)
- description and source-code
```javascript
function Object() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.Config.prototype"></a>[module s3.AWS.Config.prototype](#apidoc.module.s3.AWS.Config.prototype)

#### <a name="apidoc.element.s3.AWS.Config.prototype.clear"></a>[function <span class="apidocSignatureSpan">s3.AWS.Config.prototype.</span>clear ()](#apidoc.element.s3.AWS.Config.prototype.clear)
- description and source-code
```javascript
function clear() {
<span class="apidocCodeCommentSpan">  /*jshint forin:false */
</span>  AWS.util.each.call(this, this.keys, function (key) {
    delete this[key];
  });

  // reset credential provider
  this.set('credentials', undefined);
  this.set('credentialProvider', undefined);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Config.prototype.constructor"></a>[function <span class="apidocSignatureSpan">s3.AWS.Config.prototype.</span>constructor (options)](#apidoc.element.s3.AWS.Config.prototype.constructor)
- description and source-code
```javascript
function Config(options) {
  if (options === undefined) options = {};
  options = this.extractCredentials(options);

  AWS.util.each.call(this, this.keys, function (key, value) {
    this.set(key, options[key], value);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Config.prototype.extractCredentials"></a>[function <span class="apidocSignatureSpan">s3.AWS.Config.prototype.</span>extractCredentials (options)](#apidoc.element.s3.AWS.Config.prototype.extractCredentials)
- description and source-code
```javascript
function extractCredentials(options) {
  if (options.accessKeyId && options.secretAccessKey) {
    options = AWS.util.copy(options);
    options.credentials = new AWS.Credentials(options);
  }
  return options;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Config.prototype.getCredentials"></a>[function <span class="apidocSignatureSpan">s3.AWS.Config.prototype.</span>getCredentials (callback)](#apidoc.element.s3.AWS.Config.prototype.getCredentials)
- description and source-code
```javascript
function getCredentials(callback) {
  var self = this;

  function finish(err) {
    callback(err, err ? null : self.credentials);
  }

  function credError(msg, err) {
    return new AWS.util.error(err || new Error(), {
      code: 'CredentialsError', message: msg
    });
  }

  function getAsyncCredentials() {
    self.credentials.get(function(err) {
      if (err) {
        var msg = 'Could not load credentials from ' +
          self.credentials.constructor.name;
        err = credError(msg, err);
      }
      finish(err);
    });
  }

  function getStaticCredentials() {
    var err = null;
    if (!self.credentials.accessKeyId || !self.credentials.secretAccessKey) {
      err = credError('Missing credentials');
    }
    finish(err);
  }

  if (self.credentials) {
    if (typeof self.credentials.get === 'function') {
      getAsyncCredentials();
    } else { // static credentials
      getStaticCredentials();
    }
  } else if (self.credentialProvider) {
    self.credentialProvider.resolve(function(err, creds) {
      if (err) {
        err = credError('Could not load credentials from any providers', err);
      }
      self.credentials = creds;
      finish(err);
    });
  } else {
    finish(credError('No credentials to load'));
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Config.prototype.loadFromPath"></a>[function <span class="apidocSignatureSpan">s3.AWS.Config.prototype.</span>loadFromPath (path)](#apidoc.element.s3.AWS.Config.prototype.loadFromPath)
- description and source-code
```javascript
function loadFromPath(path) {
  this.clear();

  var options = JSON.parse(AWS.util.readFileSync(path));
  var fileSystemCreds = new AWS.FileSystemCredentials(path);
  var chain = new AWS.CredentialProviderChain();
  chain.providers.unshift(fileSystemCreds);
  chain.resolve(function (err, creds) {
    if (err) throw err;
    else options.credentials = creds;
  });

  this.constructor(options);

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Config.prototype.set"></a>[function <span class="apidocSignatureSpan">s3.AWS.Config.prototype.</span>set (property, value, defaultValue)](#apidoc.element.s3.AWS.Config.prototype.set)
- description and source-code
```javascript
function set(property, value, defaultValue) {
  if (value === undefined) {
    if (defaultValue === undefined) {
      defaultValue = this.keys[property];
    }
    if (typeof defaultValue === 'function') {
      this[property] = defaultValue.call(this);
    } else {
      this[property] = defaultValue;
    }
  } else if (property === 'httpOptions' && this[property]) {
    // deep merge httpOptions
    this[property] = AWS.util.merge(this[property], value);
  } else {
    this[property] = value;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Config.prototype.update"></a>[function <span class="apidocSignatureSpan">s3.AWS.Config.prototype.</span>update (options, allowUnknownKeys)](#apidoc.element.s3.AWS.Config.prototype.update)
- description and source-code
```javascript
function update(options, allowUnknownKeys) {
  allowUnknownKeys = allowUnknownKeys || false;
  options = this.extractCredentials(options);
  AWS.util.each.call(this, options, function (key, value) {
    if (allowUnknownKeys || this.keys.hasOwnProperty(key) ||
        AWS.Service.hasService(key)) {
      this.set(key, value);
    }
  });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.Config.prototype.keys"></a>[module s3.AWS.Config.prototype.keys](#apidoc.module.s3.AWS.Config.prototype.keys)

#### <a name="apidoc.element.s3.AWS.Config.prototype.keys.credentialProvider"></a>[function <span class="apidocSignatureSpan">s3.AWS.Config.prototype.keys.</span>credentialProvider ()](#apidoc.element.s3.AWS.Config.prototype.keys.credentialProvider)
- description and source-code
```javascript
credentialProvider = function () {
  return new AWS.CredentialProviderChain();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Config.prototype.keys.credentials"></a>[function <span class="apidocSignatureSpan">s3.AWS.Config.prototype.keys.</span>credentials ()](#apidoc.element.s3.AWS.Config.prototype.keys.credentials)
- description and source-code
```javascript
credentials = function () {
  var credentials = null;
  new AWS.CredentialProviderChain([
    function () { return new AWS.EnvironmentCredentials('AWS'); },
    function () { return new AWS.EnvironmentCredentials('AMAZON'); },
    function () { return new AWS.SharedIniFileCredentials(); }
  ]).resolve(function(err, creds) {
    if (!err) credentials = creds;
  });
  return credentials;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Config.prototype.keys.region"></a>[function <span class="apidocSignatureSpan">s3.AWS.Config.prototype.keys.</span>region ()](#apidoc.element.s3.AWS.Config.prototype.keys.region)
- description and source-code
```javascript
region = function () {
  return process.env.AWS_REGION || process.env.AMAZON_REGION;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.ConfigService"></a>[module s3.AWS.ConfigService](#apidoc.module.s3.AWS.ConfigService)

#### <a name="apidoc.element.s3.AWS.ConfigService.ConfigService"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>ConfigService ()](#apidoc.element.s3.AWS.ConfigService.ConfigService)
- description and source-code
```javascript
ConfigService = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.ConfigService.__super__"></a>[function <span class="apidocSignatureSpan">s3.AWS.ConfigService.</span>__super__ (config)](#apidoc.element.s3.AWS.ConfigService.__super__)
- description and source-code
```javascript
function Service(config) {
  if (!this.loadServiceClass) {
    throw AWS.util.error(new Error(),
      'Service must be constructed with 'new\' operator');
  }
  var ServiceClass = this.loadServiceClass(config || {});
  if (ServiceClass) return new ServiceClass(config);
  this.initialize(config);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.ConfigService.prototype"></a>[module s3.AWS.ConfigService.prototype](#apidoc.module.s3.AWS.ConfigService.prototype)

#### <a name="apidoc.element.s3.AWS.ConfigService.prototype.constructor"></a>[function <span class="apidocSignatureSpan">s3.AWS.ConfigService.prototype.</span>constructor ()](#apidoc.element.s3.AWS.ConfigService.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.CredentialProviderChain"></a>[module s3.AWS.CredentialProviderChain](#apidoc.module.s3.AWS.CredentialProviderChain)

#### <a name="apidoc.element.s3.AWS.CredentialProviderChain.CredentialProviderChain"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>CredentialProviderChain (providers)](#apidoc.element.s3.AWS.CredentialProviderChain.CredentialProviderChain)
- description and source-code
```javascript
function CredentialProviderChain(providers) {
  if (providers) {
    this.providers = providers;
  } else {
    this.providers = AWS.CredentialProviderChain.defaultProviders.slice(0);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.CredentialProviderChain.__super__"></a>[function <span class="apidocSignatureSpan">s3.AWS.CredentialProviderChain.</span>__super__ ()](#apidoc.element.s3.AWS.CredentialProviderChain.__super__)
- description and source-code
```javascript
function Credentials() {
  // hide secretAccessKey from being displayed with util.inspect
  AWS.util.hideProperties(this, ['secretAccessKey']);

  this.expired = false;
  this.expireTime = null;
  if (arguments.length === 1 && typeof arguments[0] === 'object') {
    var creds = arguments[0].credentials || arguments[0];
    this.accessKeyId = creds.accessKeyId;
    this.secretAccessKey = creds.secretAccessKey;
    this.sessionToken = creds.sessionToken;
  } else {
    this.accessKeyId = arguments[0];
    this.secretAccessKey = arguments[1];
    this.sessionToken = arguments[2];
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.CredentialProviderChain.prototype"></a>[module s3.AWS.CredentialProviderChain.prototype](#apidoc.module.s3.AWS.CredentialProviderChain.prototype)

#### <a name="apidoc.element.s3.AWS.CredentialProviderChain.prototype.constructor"></a>[function <span class="apidocSignatureSpan">s3.AWS.CredentialProviderChain.prototype.</span>constructor (providers)](#apidoc.element.s3.AWS.CredentialProviderChain.prototype.constructor)
- description and source-code
```javascript
function CredentialProviderChain(providers) {
  if (providers) {
    this.providers = providers;
  } else {
    this.providers = AWS.CredentialProviderChain.defaultProviders.slice(0);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.CredentialProviderChain.prototype.resolve"></a>[function <span class="apidocSignatureSpan">s3.AWS.CredentialProviderChain.prototype.</span>resolve (callback)](#apidoc.element.s3.AWS.CredentialProviderChain.prototype.resolve)
- description and source-code
```javascript
function resolve(callback) {
  if (this.providers.length === 0) {
    callback(new Error('No providers'));
    return this;
  }

  var index = 0;
  var providers = this.providers.slice(0);

  function resolveNext(err, creds) {
    if ((!err && creds) || index === providers.length) {
      callback(err, creds);
      return;
    }

    var provider = providers[index++];
    if (typeof provider === 'function') {
      creds = provider.call();
    } else {
      creds = provider;
    }

    if (creds.get) {
      creds.get(function(err) {
        resolveNext(err, err ? null : creds);
      });
    } else {
      resolveNext(null, creds);
    }
  }

  resolveNext();
  return this;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.Credentials"></a>[module s3.AWS.Credentials](#apidoc.module.s3.AWS.Credentials)

#### <a name="apidoc.element.s3.AWS.Credentials.Credentials"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>Credentials ()](#apidoc.element.s3.AWS.Credentials.Credentials)
- description and source-code
```javascript
function Credentials() {
  // hide secretAccessKey from being displayed with util.inspect
  AWS.util.hideProperties(this, ['secretAccessKey']);

  this.expired = false;
  this.expireTime = null;
  if (arguments.length === 1 && typeof arguments[0] === 'object') {
    var creds = arguments[0].credentials || arguments[0];
    this.accessKeyId = creds.accessKeyId;
    this.secretAccessKey = creds.secretAccessKey;
    this.sessionToken = creds.sessionToken;
  } else {
    this.accessKeyId = arguments[0];
    this.secretAccessKey = arguments[1];
    this.sessionToken = arguments[2];
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Credentials.__super__"></a>[function <span class="apidocSignatureSpan">s3.AWS.Credentials.</span>__super__ ()](#apidoc.element.s3.AWS.Credentials.__super__)
- description and source-code
```javascript
function Object() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.Credentials.prototype"></a>[module s3.AWS.Credentials.prototype](#apidoc.module.s3.AWS.Credentials.prototype)

#### <a name="apidoc.element.s3.AWS.Credentials.prototype.constructor"></a>[function <span class="apidocSignatureSpan">s3.AWS.Credentials.prototype.</span>constructor ()](#apidoc.element.s3.AWS.Credentials.prototype.constructor)
- description and source-code
```javascript
function Credentials() {
  // hide secretAccessKey from being displayed with util.inspect
  AWS.util.hideProperties(this, ['secretAccessKey']);

  this.expired = false;
  this.expireTime = null;
  if (arguments.length === 1 && typeof arguments[0] === 'object') {
    var creds = arguments[0].credentials || arguments[0];
    this.accessKeyId = creds.accessKeyId;
    this.secretAccessKey = creds.secretAccessKey;
    this.sessionToken = creds.sessionToken;
  } else {
    this.accessKeyId = arguments[0];
    this.secretAccessKey = arguments[1];
    this.sessionToken = arguments[2];
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Credentials.prototype.get"></a>[function <span class="apidocSignatureSpan">s3.AWS.Credentials.prototype.</span>get (callback)](#apidoc.element.s3.AWS.Credentials.prototype.get)
- description and source-code
```javascript
function get(callback) {
  var self = this;
  if (this.needsRefresh()) {
    this.refresh(function(err) {
      if (!err) self.expired = false; // reset expired flag
      if (callback) callback(err);
    });
  } else if (callback) {
    callback();
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Credentials.prototype.needsRefresh"></a>[function <span class="apidocSignatureSpan">s3.AWS.Credentials.prototype.</span>needsRefresh ()](#apidoc.element.s3.AWS.Credentials.prototype.needsRefresh)
- description and source-code
```javascript
function needsRefresh() {
  var currentTime = AWS.util.date.getDate().getTime();
  var adjustedTime = new Date(currentTime + this.expiryWindow * 1000);

  if (this.expireTime && adjustedTime > this.expireTime) {
    return true;
  } else {
    return this.expired || !this.accessKeyId || !this.secretAccessKey;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Credentials.prototype.refresh"></a>[function <span class="apidocSignatureSpan">s3.AWS.Credentials.prototype.</span>refresh (callback)](#apidoc.element.s3.AWS.Credentials.prototype.refresh)
- description and source-code
```javascript
function refresh(callback) {
  this.expired = false;
  callback();
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.DataPipeline"></a>[module s3.AWS.DataPipeline](#apidoc.module.s3.AWS.DataPipeline)

#### <a name="apidoc.element.s3.AWS.DataPipeline.DataPipeline"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>DataPipeline ()](#apidoc.element.s3.AWS.DataPipeline.DataPipeline)
- description and source-code
```javascript
DataPipeline = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.DataPipeline.__super__"></a>[function <span class="apidocSignatureSpan">s3.AWS.DataPipeline.</span>__super__ (config)](#apidoc.element.s3.AWS.DataPipeline.__super__)
- description and source-code
```javascript
function Service(config) {
  if (!this.loadServiceClass) {
    throw AWS.util.error(new Error(),
      'Service must be constructed with 'new\' operator');
  }
  var ServiceClass = this.loadServiceClass(config || {});
  if (ServiceClass) return new ServiceClass(config);
  this.initialize(config);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.DataPipeline.prototype"></a>[module s3.AWS.DataPipeline.prototype](#apidoc.module.s3.AWS.DataPipeline.prototype)

#### <a name="apidoc.element.s3.AWS.DataPipeline.prototype.constructor"></a>[function <span class="apidocSignatureSpan">s3.AWS.DataPipeline.prototype.</span>constructor ()](#apidoc.element.s3.AWS.DataPipeline.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.DirectConnect"></a>[module s3.AWS.DirectConnect](#apidoc.module.s3.AWS.DirectConnect)

#### <a name="apidoc.element.s3.AWS.DirectConnect.DirectConnect"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>DirectConnect ()](#apidoc.element.s3.AWS.DirectConnect.DirectConnect)
- description and source-code
```javascript
DirectConnect = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.DirectConnect.__super__"></a>[function <span class="apidocSignatureSpan">s3.AWS.DirectConnect.</span>__super__ (config)](#apidoc.element.s3.AWS.DirectConnect.__super__)
- description and source-code
```javascript
function Service(config) {
  if (!this.loadServiceClass) {
    throw AWS.util.error(new Error(),
      'Service must be constructed with 'new\' operator');
  }
  var ServiceClass = this.loadServiceClass(config || {});
  if (ServiceClass) return new ServiceClass(config);
  this.initialize(config);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.DirectConnect.prototype"></a>[module s3.AWS.DirectConnect.prototype](#apidoc.module.s3.AWS.DirectConnect.prototype)

#### <a name="apidoc.element.s3.AWS.DirectConnect.prototype.constructor"></a>[function <span class="apidocSignatureSpan">s3.AWS.DirectConnect.prototype.</span>constructor ()](#apidoc.element.s3.AWS.DirectConnect.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.DynamoDB"></a>[module s3.AWS.DynamoDB](#apidoc.module.s3.AWS.DynamoDB)

#### <a name="apidoc.element.s3.AWS.DynamoDB.DynamoDB"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>DynamoDB ()](#apidoc.element.s3.AWS.DynamoDB.DynamoDB)
- description and source-code
```javascript
DynamoDB = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.DynamoDB.__super__"></a>[function <span class="apidocSignatureSpan">s3.AWS.DynamoDB.</span>__super__ (config)](#apidoc.element.s3.AWS.DynamoDB.__super__)
- description and source-code
```javascript
function Service(config) {
  if (!this.loadServiceClass) {
    throw AWS.util.error(new Error(),
      'Service must be constructed with 'new\' operator');
  }
  var ServiceClass = this.loadServiceClass(config || {});
  if (ServiceClass) return new ServiceClass(config);
  this.initialize(config);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.DynamoDB.prototype"></a>[module s3.AWS.DynamoDB.prototype](#apidoc.module.s3.AWS.DynamoDB.prototype)

#### <a name="apidoc.element.s3.AWS.DynamoDB.prototype.checkCrc32"></a>[function <span class="apidocSignatureSpan">s3.AWS.DynamoDB.prototype.</span>checkCrc32 (resp)](#apidoc.element.s3.AWS.DynamoDB.prototype.checkCrc32)
- description and source-code
```javascript
function checkCrc32(resp) {
  if (!resp.httpResponse.streaming && !resp.request.service.crc32IsValid(resp)) {
    resp.error = AWS.util.error(new Error(), {
      code: 'CRC32CheckFailed',
      message: 'CRC32 integrity check failed',
      retryable: true
    });
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.DynamoDB.prototype.constructor"></a>[function <span class="apidocSignatureSpan">s3.AWS.DynamoDB.prototype.</span>constructor ()](#apidoc.element.s3.AWS.DynamoDB.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.DynamoDB.prototype.crc32IsValid"></a>[function <span class="apidocSignatureSpan">s3.AWS.DynamoDB.prototype.</span>crc32IsValid (resp)](#apidoc.element.s3.AWS.DynamoDB.prototype.crc32IsValid)
- description and source-code
```javascript
function crc32IsValid(resp) {
  var crc = resp.httpResponse.headers['x-amz-crc32'];
  if (!crc) return true; // no (valid) CRC32 header
  return parseInt(crc, 10) === AWS.util.crypto.crc32(resp.httpResponse.body);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.DynamoDB.prototype.retryDelays"></a>[function <span class="apidocSignatureSpan">s3.AWS.DynamoDB.prototype.</span>retryDelays ()](#apidoc.element.s3.AWS.DynamoDB.prototype.retryDelays)
- description and source-code
```javascript
function retryDelays() {
  var retryCount = this.numRetries();
  var delays = [];
  for (var i = 0; i < retryCount; ++i) {
    if (i === 0) {
      delays.push(0);
    } else {
      delays.push(50 * Math.pow(2, i - 1));
    }
  }
  return delays;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.DynamoDB.prototype.setupRequestListeners"></a>[function <span class="apidocSignatureSpan">s3.AWS.DynamoDB.prototype.</span>setupRequestListeners (request)](#apidoc.element.s3.AWS.DynamoDB.prototype.setupRequestListeners)
- description and source-code
```javascript
function setupRequestListeners(request) {
  if (request.service.config.dynamoDbCrc32) {
    request.addListener('extractData', this.checkCrc32);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.EC2"></a>[module s3.AWS.EC2](#apidoc.module.s3.AWS.EC2)

#### <a name="apidoc.element.s3.AWS.EC2.EC2"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>EC2 ()](#apidoc.element.s3.AWS.EC2.EC2)
- description and source-code
```javascript
EC2 = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.EC2.__super__"></a>[function <span class="apidocSignatureSpan">s3.AWS.EC2.</span>__super__ (config)](#apidoc.element.s3.AWS.EC2.__super__)
- description and source-code
```javascript
function Service(config) {
  if (!this.loadServiceClass) {
    throw AWS.util.error(new Error(),
      'Service must be constructed with 'new\' operator');
  }
  var ServiceClass = this.loadServiceClass(config || {});
  if (ServiceClass) return new ServiceClass(config);
  this.initialize(config);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.EC2.prototype"></a>[module s3.AWS.EC2.prototype](#apidoc.module.s3.AWS.EC2.prototype)

#### <a name="apidoc.element.s3.AWS.EC2.prototype.buildCopySnapshotPresignedUrl"></a>[function <span class="apidocSignatureSpan">s3.AWS.EC2.prototype.</span>buildCopySnapshotPresignedUrl (req, done)](#apidoc.element.s3.AWS.EC2.prototype.buildCopySnapshotPresignedUrl)
- description and source-code
```javascript
function buildCopySnapshotPresignedUrl(req, done) {
  if (req.params.PresignedUrl || req._subRequest) {
    return done();
  }

  req.params = AWS.util.copy(req.params);
  req.params.DestinationRegion = req.service.config.region;

  var config = AWS.util.copy(req.service.config);
  delete config.endpoint;
  config.region = req.params.SourceRegion;
  var svc = new req.service.constructor(config);
  var newReq = svc[req.operation](req.params);
  newReq._subRequest = true;
  newReq.presign(function(err, url) {
    if (err) done(err);
    else {
      req.params.PresignedUrl = url;
      done();
    }
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.EC2.prototype.constructor"></a>[function <span class="apidocSignatureSpan">s3.AWS.EC2.prototype.</span>constructor ()](#apidoc.element.s3.AWS.EC2.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.EC2.prototype.extractError"></a>[function <span class="apidocSignatureSpan">s3.AWS.EC2.prototype.</span>extractError (resp)](#apidoc.element.s3.AWS.EC2.prototype.extractError)
- description and source-code
```javascript
function extractError(resp) {
  // EC2 nests the error code and message deeper than other AWS Query services.
  var httpResponse = resp.httpResponse;
  var data = new AWS.XML.Parser().parse(httpResponse.body.toString() || '');
  if (data.Errors)
    resp.error = AWS.util.error(new Error(), {
      code: data.Errors.Error.Code,
      message: data.Errors.Error.Message
    });
  else
    resp.error = AWS.util.error(new Error(), {
      code: httpResponse.statusCode,
      message: null
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.EC2.prototype.setupRequestListeners"></a>[function <span class="apidocSignatureSpan">s3.AWS.EC2.prototype.</span>setupRequestListeners (request)](#apidoc.element.s3.AWS.EC2.prototype.setupRequestListeners)
- description and source-code
```javascript
function setupRequestListeners(request) {
  request.removeListener('extractError', AWS.EventListeners.Query.EXTRACT_ERROR);
  request.addListener('extractError', this.extractError);

  if (request.operation === 'copySnapshot') {
    request.onAsync('validate', this.buildCopySnapshotPresignedUrl);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.EC2MetadataCredentials"></a>[module s3.AWS.EC2MetadataCredentials](#apidoc.module.s3.AWS.EC2MetadataCredentials)

#### <a name="apidoc.element.s3.AWS.EC2MetadataCredentials.EC2MetadataCredentials"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>EC2MetadataCredentials (options)](#apidoc.element.s3.AWS.EC2MetadataCredentials.EC2MetadataCredentials)
- description and source-code
```javascript
function EC2MetadataCredentials(options) {
  AWS.Credentials.call(this);

  options = options ? AWS.util.copy(options) : {};
  if (!options.httpOptions) options.httpOptions = {};
  options.httpOptions = AWS.util.merge(
    {timeout: this.defaultTimeout}, options.httpOptions);

  this.metadataService = new AWS.MetadataService(options);
  this.metadata = {};
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.EC2MetadataCredentials.__super__"></a>[function <span class="apidocSignatureSpan">s3.AWS.EC2MetadataCredentials.</span>__super__ ()](#apidoc.element.s3.AWS.EC2MetadataCredentials.__super__)
- description and source-code
```javascript
function Credentials() {
  // hide secretAccessKey from being displayed with util.inspect
  AWS.util.hideProperties(this, ['secretAccessKey']);

  this.expired = false;
  this.expireTime = null;
  if (arguments.length === 1 && typeof arguments[0] === 'object') {
    var creds = arguments[0].credentials || arguments[0];
    this.accessKeyId = creds.accessKeyId;
    this.secretAccessKey = creds.secretAccessKey;
    this.sessionToken = creds.sessionToken;
  } else {
    this.accessKeyId = arguments[0];
    this.secretAccessKey = arguments[1];
    this.sessionToken = arguments[2];
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.EC2MetadataCredentials.prototype"></a>[module s3.AWS.EC2MetadataCredentials.prototype](#apidoc.module.s3.AWS.EC2MetadataCredentials.prototype)

#### <a name="apidoc.element.s3.AWS.EC2MetadataCredentials.prototype.constructor"></a>[function <span class="apidocSignatureSpan">s3.AWS.EC2MetadataCredentials.prototype.</span>constructor (options)](#apidoc.element.s3.AWS.EC2MetadataCredentials.prototype.constructor)
- description and source-code
```javascript
function EC2MetadataCredentials(options) {
  AWS.Credentials.call(this);

  options = options ? AWS.util.copy(options) : {};
  if (!options.httpOptions) options.httpOptions = {};
  options.httpOptions = AWS.util.merge(
    {timeout: this.defaultTimeout}, options.httpOptions);

  this.metadataService = new AWS.MetadataService(options);
  this.metadata = {};
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.EC2MetadataCredentials.prototype.refresh"></a>[function <span class="apidocSignatureSpan">s3.AWS.EC2MetadataCredentials.prototype.</span>refresh (callback)](#apidoc.element.s3.AWS.EC2MetadataCredentials.prototype.refresh)
- description and source-code
```javascript
function refresh(callback) {
  var self = this;
  if (!callback) callback = function(err) { if (err) throw err; };

  self.metadataService.loadCredentials(function (err, creds) {
    if (!err) {
      self.expired = false;
      self.metadata = creds;
      self.accessKeyId = creds.AccessKeyId;
      self.secretAccessKey = creds.SecretAccessKey;
      self.sessionToken = creds.Token;
      self.expireTime = new Date(creds.Expiration);
    }
    callback(err);
  });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.ELB"></a>[module s3.AWS.ELB](#apidoc.module.s3.AWS.ELB)

#### <a name="apidoc.element.s3.AWS.ELB.ELB"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>ELB ()](#apidoc.element.s3.AWS.ELB.ELB)
- description and source-code
```javascript
ELB = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.ELB.__super__"></a>[function <span class="apidocSignatureSpan">s3.AWS.ELB.</span>__super__ (config)](#apidoc.element.s3.AWS.ELB.__super__)
- description and source-code
```javascript
function Service(config) {
  if (!this.loadServiceClass) {
    throw AWS.util.error(new Error(),
      'Service must be constructed with 'new\' operator');
  }
  var ServiceClass = this.loadServiceClass(config || {});
  if (ServiceClass) return new ServiceClass(config);
  this.initialize(config);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.ELB.prototype"></a>[module s3.AWS.ELB.prototype](#apidoc.module.s3.AWS.ELB.prototype)

#### <a name="apidoc.element.s3.AWS.ELB.prototype.constructor"></a>[function <span class="apidocSignatureSpan">s3.AWS.ELB.prototype.</span>constructor ()](#apidoc.element.s3.AWS.ELB.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.EMR"></a>[module s3.AWS.EMR](#apidoc.module.s3.AWS.EMR)

#### <a name="apidoc.element.s3.AWS.EMR.EMR"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>EMR ()](#apidoc.element.s3.AWS.EMR.EMR)
- description and source-code
```javascript
EMR = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.EMR.__super__"></a>[function <span class="apidocSignatureSpan">s3.AWS.EMR.</span>__super__ (config)](#apidoc.element.s3.AWS.EMR.__super__)
- description and source-code
```javascript
function Service(config) {
  if (!this.loadServiceClass) {
    throw AWS.util.error(new Error(),
      'Service must be constructed with 'new\' operator');
  }
  var ServiceClass = this.loadServiceClass(config || {});
  if (ServiceClass) return new ServiceClass(config);
  this.initialize(config);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.EMR.prototype"></a>[module s3.AWS.EMR.prototype](#apidoc.module.s3.AWS.EMR.prototype)

#### <a name="apidoc.element.s3.AWS.EMR.prototype.constructor"></a>[function <span class="apidocSignatureSpan">s3.AWS.EMR.prototype.</span>constructor ()](#apidoc.element.s3.AWS.EMR.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.ElastiCache"></a>[module s3.AWS.ElastiCache](#apidoc.module.s3.AWS.ElastiCache)

#### <a name="apidoc.element.s3.AWS.ElastiCache.ElastiCache"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>ElastiCache ()](#apidoc.element.s3.AWS.ElastiCache.ElastiCache)
- description and source-code
```javascript
ElastiCache = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.ElastiCache.__super__"></a>[function <span class="apidocSignatureSpan">s3.AWS.ElastiCache.</span>__super__ (config)](#apidoc.element.s3.AWS.ElastiCache.__super__)
- description and source-code
```javascript
function Service(config) {
  if (!this.loadServiceClass) {
    throw AWS.util.error(new Error(),
      'Service must be constructed with 'new\' operator');
  }
  var ServiceClass = this.loadServiceClass(config || {});
  if (ServiceClass) return new ServiceClass(config);
  this.initialize(config);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.ElastiCache.prototype"></a>[module s3.AWS.ElastiCache.prototype](#apidoc.module.s3.AWS.ElastiCache.prototype)

#### <a name="apidoc.element.s3.AWS.ElastiCache.prototype.constructor"></a>[function <span class="apidocSignatureSpan">s3.AWS.ElastiCache.prototype.</span>constructor ()](#apidoc.element.s3.AWS.ElastiCache.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.ElasticBeanstalk"></a>[module s3.AWS.ElasticBeanstalk](#apidoc.module.s3.AWS.ElasticBeanstalk)

#### <a name="apidoc.element.s3.AWS.ElasticBeanstalk.ElasticBeanstalk"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>ElasticBeanstalk ()](#apidoc.element.s3.AWS.ElasticBeanstalk.ElasticBeanstalk)
- description and source-code
```javascript
ElasticBeanstalk = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.ElasticBeanstalk.__super__"></a>[function <span class="apidocSignatureSpan">s3.AWS.ElasticBeanstalk.</span>__super__ (config)](#apidoc.element.s3.AWS.ElasticBeanstalk.__super__)
- description and source-code
```javascript
function Service(config) {
  if (!this.loadServiceClass) {
    throw AWS.util.error(new Error(),
      'Service must be constructed with 'new\' operator');
  }
  var ServiceClass = this.loadServiceClass(config || {});
  if (ServiceClass) return new ServiceClass(config);
  this.initialize(config);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.ElasticBeanstalk.prototype"></a>[module s3.AWS.ElasticBeanstalk.prototype](#apidoc.module.s3.AWS.ElasticBeanstalk.prototype)

#### <a name="apidoc.element.s3.AWS.ElasticBeanstalk.prototype.constructor"></a>[function <span class="apidocSignatureSpan">s3.AWS.ElasticBeanstalk.prototype.</span>constructor ()](#apidoc.element.s3.AWS.ElasticBeanstalk.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.ElasticTranscoder"></a>[module s3.AWS.ElasticTranscoder](#apidoc.module.s3.AWS.ElasticTranscoder)

#### <a name="apidoc.element.s3.AWS.ElasticTranscoder.ElasticTranscoder"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>ElasticTranscoder ()](#apidoc.element.s3.AWS.ElasticTranscoder.ElasticTranscoder)
- description and source-code
```javascript
ElasticTranscoder = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.ElasticTranscoder.__super__"></a>[function <span class="apidocSignatureSpan">s3.AWS.ElasticTranscoder.</span>__super__ (config)](#apidoc.element.s3.AWS.ElasticTranscoder.__super__)
- description and source-code
```javascript
function Service(config) {
  if (!this.loadServiceClass) {
    throw AWS.util.error(new Error(),
      'Service must be constructed with 'new\' operator');
  }
  var ServiceClass = this.loadServiceClass(config || {});
  if (ServiceClass) return new ServiceClass(config);
  this.initialize(config);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.ElasticTranscoder.prototype"></a>[module s3.AWS.ElasticTranscoder.prototype](#apidoc.module.s3.AWS.ElasticTranscoder.prototype)

#### <a name="apidoc.element.s3.AWS.ElasticTranscoder.prototype.constructor"></a>[function <span class="apidocSignatureSpan">s3.AWS.ElasticTranscoder.prototype.</span>constructor ()](#apidoc.element.s3.AWS.ElasticTranscoder.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.Endpoint"></a>[module s3.AWS.Endpoint](#apidoc.module.s3.AWS.Endpoint)

#### <a name="apidoc.element.s3.AWS.Endpoint.Endpoint"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>Endpoint (endpoint, config)](#apidoc.element.s3.AWS.Endpoint.Endpoint)
- description and source-code
```javascript
function Endpoint(endpoint, config) {
  AWS.util.hideProperties(this, ['slashes', 'auth', 'hash', 'search', 'query']);

  if (typeof endpoint === 'undefined' || endpoint === null) {
    throw new Error('Invalid endpoint: ' + endpoint);
  } else if (typeof endpoint !== 'string') {
    return AWS.util.copy(endpoint);
  }

  if (!endpoint.match(/^http/)) {
    var useSSL = config && config.sslEnabled !== undefined ?
      config.sslEnabled : AWS.config.sslEnabled;
    endpoint = (useSSL ? 'https' : 'http') + '://' + endpoint;
  }

  AWS.util.update(this, AWS.util.urlParse(endpoint));

  // Ensure the port property is set as an integer
  if (this.port) {
    this.port = parseInt(this.port, 10);
  } else {
    this.port = this.protocol === 'https:' ? 443 : 80;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Endpoint.__super__"></a>[function <span class="apidocSignatureSpan">s3.AWS.Endpoint.</span>__super__ ()](#apidoc.element.s3.AWS.Endpoint.__super__)
- description and source-code
```javascript
function Object() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.Endpoint.prototype"></a>[module s3.AWS.Endpoint.prototype](#apidoc.module.s3.AWS.Endpoint.prototype)

#### <a name="apidoc.element.s3.AWS.Endpoint.prototype.constructor"></a>[function <span class="apidocSignatureSpan">s3.AWS.Endpoint.prototype.</span>constructor (endpoint, config)](#apidoc.element.s3.AWS.Endpoint.prototype.constructor)
- description and source-code
```javascript
function Endpoint(endpoint, config) {
  AWS.util.hideProperties(this, ['slashes', 'auth', 'hash', 'search', 'query']);

  if (typeof endpoint === 'undefined' || endpoint === null) {
    throw new Error('Invalid endpoint: ' + endpoint);
  } else if (typeof endpoint !== 'string') {
    return AWS.util.copy(endpoint);
  }

  if (!endpoint.match(/^http/)) {
    var useSSL = config && config.sslEnabled !== undefined ?
      config.sslEnabled : AWS.config.sslEnabled;
    endpoint = (useSSL ? 'https' : 'http') + '://' + endpoint;
  }

  AWS.util.update(this, AWS.util.urlParse(endpoint));

  // Ensure the port property is set as an integer
  if (this.port) {
    this.port = parseInt(this.port, 10);
  } else {
    this.port = this.protocol === 'https:' ? 443 : 80;
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.EnvironmentCredentials"></a>[module s3.AWS.EnvironmentCredentials](#apidoc.module.s3.AWS.EnvironmentCredentials)

#### <a name="apidoc.element.s3.AWS.EnvironmentCredentials.EnvironmentCredentials"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>EnvironmentCredentials (envPrefix)](#apidoc.element.s3.AWS.EnvironmentCredentials.EnvironmentCredentials)
- description and source-code
```javascript
function EnvironmentCredentials(envPrefix) {
  AWS.Credentials.call(this);
  this.envPrefix = envPrefix;
  this.get(function() {});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.EnvironmentCredentials.__super__"></a>[function <span class="apidocSignatureSpan">s3.AWS.EnvironmentCredentials.</span>__super__ ()](#apidoc.element.s3.AWS.EnvironmentCredentials.__super__)
- description and source-code
```javascript
function Credentials() {
  // hide secretAccessKey from being displayed with util.inspect
  AWS.util.hideProperties(this, ['secretAccessKey']);

  this.expired = false;
  this.expireTime = null;
  if (arguments.length === 1 && typeof arguments[0] === 'object') {
    var creds = arguments[0].credentials || arguments[0];
    this.accessKeyId = creds.accessKeyId;
    this.secretAccessKey = creds.secretAccessKey;
    this.sessionToken = creds.sessionToken;
  } else {
    this.accessKeyId = arguments[0];
    this.secretAccessKey = arguments[1];
    this.sessionToken = arguments[2];
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.EnvironmentCredentials.prototype"></a>[module s3.AWS.EnvironmentCredentials.prototype](#apidoc.module.s3.AWS.EnvironmentCredentials.prototype)

#### <a name="apidoc.element.s3.AWS.EnvironmentCredentials.prototype.constructor"></a>[function <span class="apidocSignatureSpan">s3.AWS.EnvironmentCredentials.prototype.</span>constructor (envPrefix)](#apidoc.element.s3.AWS.EnvironmentCredentials.prototype.constructor)
- description and source-code
```javascript
function EnvironmentCredentials(envPrefix) {
  AWS.Credentials.call(this);
  this.envPrefix = envPrefix;
  this.get(function() {});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.EnvironmentCredentials.prototype.refresh"></a>[function <span class="apidocSignatureSpan">s3.AWS.EnvironmentCredentials.prototype.</span>refresh (callback)](#apidoc.element.s3.AWS.EnvironmentCredentials.prototype.refresh)
- description and source-code
```javascript
function refresh(callback) {
  if (!callback) callback = function(err) { if (err) throw err; };

  if (process === undefined) {
    callback(new Error('No process info available'));
    return;
  }

  var keys = ['ACCESS_KEY_ID', 'SECRET_ACCESS_KEY', 'SESSION_TOKEN'];
  var values = [];

  for (var i = 0; i < keys.length; i++) {
    var prefix = '';
    if (this.envPrefix) prefix = this.envPrefix + '_';
    values[i] = process.env[prefix + keys[i]];
    if (!values[i] && keys[i] !== 'SESSION_TOKEN') {
      callback(new Error('Variable ' + prefix + keys[i] + ' not set.'));
      return;
    }
  }

  this.expired = false;
  AWS.Credentials.apply(this, values);
  callback();
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.FileSystemCredentials"></a>[module s3.AWS.FileSystemCredentials](#apidoc.module.s3.AWS.FileSystemCredentials)

#### <a name="apidoc.element.s3.AWS.FileSystemCredentials.FileSystemCredentials"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>FileSystemCredentials (filename)](#apidoc.element.s3.AWS.FileSystemCredentials.FileSystemCredentials)
- description and source-code
```javascript
function FileSystemCredentials(filename) {
  AWS.Credentials.call(this);
  this.filename = filename;
  this.get(function() {});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.FileSystemCredentials.__super__"></a>[function <span class="apidocSignatureSpan">s3.AWS.FileSystemCredentials.</span>__super__ ()](#apidoc.element.s3.AWS.FileSystemCredentials.__super__)
- description and source-code
```javascript
function Credentials() {
  // hide secretAccessKey from being displayed with util.inspect
  AWS.util.hideProperties(this, ['secretAccessKey']);

  this.expired = false;
  this.expireTime = null;
  if (arguments.length === 1 && typeof arguments[0] === 'object') {
    var creds = arguments[0].credentials || arguments[0];
    this.accessKeyId = creds.accessKeyId;
    this.secretAccessKey = creds.secretAccessKey;
    this.sessionToken = creds.sessionToken;
  } else {
    this.accessKeyId = arguments[0];
    this.secretAccessKey = arguments[1];
    this.sessionToken = arguments[2];
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.FileSystemCredentials.prototype"></a>[module s3.AWS.FileSystemCredentials.prototype](#apidoc.module.s3.AWS.FileSystemCredentials.prototype)

#### <a name="apidoc.element.s3.AWS.FileSystemCredentials.prototype.constructor"></a>[function <span class="apidocSignatureSpan">s3.AWS.FileSystemCredentials.prototype.</span>constructor (filename)](#apidoc.element.s3.AWS.FileSystemCredentials.prototype.constructor)
- description and source-code
```javascript
function FileSystemCredentials(filename) {
  AWS.Credentials.call(this);
  this.filename = filename;
  this.get(function() {});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.FileSystemCredentials.prototype.refresh"></a>[function <span class="apidocSignatureSpan">s3.AWS.FileSystemCredentials.prototype.</span>refresh (callback)](#apidoc.element.s3.AWS.FileSystemCredentials.prototype.refresh)
- description and source-code
```javascript
function refresh(callback) {
  if (!callback) callback = function(err) { if (err) throw err; };
  try {
    var creds = JSON.parse(AWS.util.readFileSync(this.filename));
    AWS.Credentials.call(this, creds);
    if (!this.accessKeyId || !this.secretAccessKey) {
      throw new Error('Credentials not set in ' + this.filename);
    }
    this.expired = false;
    callback();
  } catch (err) {
    callback(err);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.Glacier"></a>[module s3.AWS.Glacier](#apidoc.module.s3.AWS.Glacier)

#### <a name="apidoc.element.s3.AWS.Glacier.Glacier"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>Glacier ()](#apidoc.element.s3.AWS.Glacier.Glacier)
- description and source-code
```javascript
Glacier = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Glacier.__super__"></a>[function <span class="apidocSignatureSpan">s3.AWS.Glacier.</span>__super__ (config)](#apidoc.element.s3.AWS.Glacier.__super__)
- description and source-code
```javascript
function Service(config) {
  if (!this.loadServiceClass) {
    throw AWS.util.error(new Error(),
      'Service must be constructed with 'new\' operator');
  }
  var ServiceClass = this.loadServiceClass(config || {});
  if (ServiceClass) return new ServiceClass(config);
  this.initialize(config);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.Glacier.prototype"></a>[module s3.AWS.Glacier.prototype](#apidoc.module.s3.AWS.Glacier.prototype)

#### <a name="apidoc.element.s3.AWS.Glacier.prototype.addGlacierApiVersion"></a>[function <span class="apidocSignatureSpan">s3.AWS.Glacier.prototype.</span>addGlacierApiVersion (request)](#apidoc.element.s3.AWS.Glacier.prototype.addGlacierApiVersion)
- description and source-code
```javascript
function addGlacierApiVersion(request) {
  var version = request.service.api.apiVersion;
  request.httpRequest.headers['x-amz-glacier-version'] = version;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Glacier.prototype.addTreeHashHeaders"></a>[function <span class="apidocSignatureSpan">s3.AWS.Glacier.prototype.</span>addTreeHashHeaders (request)](#apidoc.element.s3.AWS.Glacier.prototype.addTreeHashHeaders)
- description and source-code
```javascript
function addTreeHashHeaders(request) {
  if (request.params.body === undefined) return;

  var hashes = request.service.computeChecksums(request.params.body);
  request.httpRequest.headers['x-amz-content-sha256'] = hashes.linearHash;

  if (!request.httpRequest.headers['x-amz-sha256-tree-hash']) {
    request.httpRequest.headers['x-amz-sha256-tree-hash'] = hashes.treeHash;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Glacier.prototype.buildHashTree"></a>[function <span class="apidocSignatureSpan">s3.AWS.Glacier.prototype.</span>buildHashTree (hashes)](#apidoc.element.s3.AWS.Glacier.prototype.buildHashTree)
- description and source-code
```javascript
function buildHashTree(hashes) {
  // merge leaf nodes
  while (hashes.length > 1) {
    var tmpHashes = [];
    for (var i = 0; i < hashes.length; i += 2) {
      if (hashes[i + 1]) {
        var tmpHash = new AWS.util.Buffer(64);
        tmpHash.write(hashes[i], 0, 32, 'binary');
        tmpHash.write(hashes[i + 1], 32, 32, 'binary');
        tmpHashes.push(AWS.util.crypto.sha256(tmpHash));
      } else {
        tmpHashes.push(hashes[i]);
      }
    }
    hashes = tmpHashes;
  }

  return AWS.util.crypto.toHex(hashes[0]);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Glacier.prototype.computeChecksums"></a>[function <span class="apidocSignatureSpan">s3.AWS.Glacier.prototype.</span>computeChecksums (data)](#apidoc.element.s3.AWS.Glacier.prototype.computeChecksums)
- description and source-code
```javascript
function computeChecksums(data) {
  if (!AWS.util.Buffer.isBuffer(data)) data = new AWS.util.Buffer(data);

  var mb = 1024 * 1024;
  var hashes = [];
  var hash = AWS.util.crypto.createHash('sha256');

  // build leaf nodes in 1mb chunks
  for (var i = 0; i < data.length; i += mb) {
    var chunk = data.slice(i, Math.min(i + mb, data.length));
    hash.update(chunk);
    hashes.push(AWS.util.crypto.sha256(chunk));
  }

  return {
    linearHash: hash.digest('hex'),
    treeHash: this.buildHashTree(hashes)
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Glacier.prototype.constructor"></a>[function <span class="apidocSignatureSpan">s3.AWS.Glacier.prototype.</span>constructor ()](#apidoc.element.s3.AWS.Glacier.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Glacier.prototype.setupRequestListeners"></a>[function <span class="apidocSignatureSpan">s3.AWS.Glacier.prototype.</span>setupRequestListeners (request)](#apidoc.element.s3.AWS.Glacier.prototype.setupRequestListeners)
- description and source-code
```javascript
function setupRequestListeners(request) {
  if (Array.isArray(request._events.validate)) {
    request._events.validate.unshift(this.validateAccountId);
  } else {
    request.on('validate', this.validateAccountId);
  }

  request.on('build', this.addGlacierApiVersion);
  request.on('build', this.addTreeHashHeaders);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Glacier.prototype.validateAccountId"></a>[function <span class="apidocSignatureSpan">s3.AWS.Glacier.prototype.</span>validateAccountId (request)](#apidoc.element.s3.AWS.Glacier.prototype.validateAccountId)
- description and source-code
```javascript
function validateAccountId(request) {
  if (request.params.accountId !== undefined) return;
  request.params = AWS.util.copy(request.params);
  request.params.accountId = '-';
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.HttpClient"></a>[module s3.AWS.HttpClient](#apidoc.module.s3.AWS.HttpClient)

#### <a name="apidoc.element.s3.AWS.HttpClient.HttpClient"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>HttpClient ()](#apidoc.element.s3.AWS.HttpClient.HttpClient)
- description and source-code
```javascript
HttpClient = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.HttpClient.__super__"></a>[function <span class="apidocSignatureSpan">s3.AWS.HttpClient.</span>__super__ ()](#apidoc.element.s3.AWS.HttpClient.__super__)
- description and source-code
```javascript
function Object() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.HttpClient.getInstance"></a>[function <span class="apidocSignatureSpan">s3.AWS.HttpClient.</span>getInstance ()](#apidoc.element.s3.AWS.HttpClient.getInstance)
- description and source-code
```javascript
function getInstance() {
  if (this.singleton === undefined) {
    this.singleton = new this();
  }
  return this.singleton;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.HttpClient.prototype"></a>[module s3.AWS.HttpClient.prototype](#apidoc.module.s3.AWS.HttpClient.prototype)

#### <a name="apidoc.element.s3.AWS.HttpClient.prototype.constructor"></a>[function <span class="apidocSignatureSpan">s3.AWS.HttpClient.prototype.</span>constructor ()](#apidoc.element.s3.AWS.HttpClient.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.HttpClient.prototype.handleRequest"></a>[function <span class="apidocSignatureSpan">s3.AWS.HttpClient.prototype.</span>handleRequest (httpRequest, httpOptions, callback, errCallback)](#apidoc.element.s3.AWS.HttpClient.prototype.handleRequest)
- description and source-code
```javascript
function handleRequest(httpRequest, httpOptions, callback, errCallback) {
  var cbAlreadyCalled = false;
  var endpoint = httpRequest.endpoint;
  var pathPrefix = '';
  if (!httpOptions) httpOptions = {};
  if (httpOptions.proxy) {
    pathPrefix = endpoint.protocol + '//' + endpoint.hostname;
    if (endpoint.port !== 80 && endpoint.port !== 443) {
      pathPrefix += ':' + endpoint.port;
    }
    endpoint = new AWS.Endpoint(httpOptions.proxy);
  }

  var useSSL = endpoint.protocol === 'https:';
  var http = useSSL ? require('https') : require('http');
  var options = {
    host: endpoint.hostname,
    port: endpoint.port,
    method: httpRequest.method,
    headers: httpRequest.headers,
    path: pathPrefix + httpRequest.path
  };

  if (useSSL && !httpOptions.agent) {
    options.agent = this.sslAgent();
  }

  AWS.util.update(options, httpOptions);
  delete options.proxy; // proxy isn't an HTTP option
  delete options.timeout; // timeout isn't an HTTP option

  var stream = http.request(options, function (httpResp) {
    if (cbAlreadyCalled) return; cbAlreadyCalled = true;

    callback(httpResp);
    httpResp.emit('headers', httpResp.statusCode, httpResp.headers);
  });
  httpRequest.stream = stream; // attach stream to httpRequest

  // timeout support
  stream.setTimeout(httpOptions.timeout || 0, function() {
    if (cbAlreadyCalled) return; cbAlreadyCalled = true;

    var msg = 'Connection timed out after ' + httpOptions.timeout + 'ms';
    errCallback(AWS.util.error(new Error(msg), {code: 'TimeoutError'}));
    stream.abort();
  });

  stream.on('error', function() {
    if (cbAlreadyCalled) return; cbAlreadyCalled = true;
    errCallback.apply(this, arguments);
  });

  this.writeBody(stream, httpRequest);
  return stream;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.HttpClient.prototype.progressStream"></a>[function <span class="apidocSignatureSpan">s3.AWS.HttpClient.prototype.</span>progressStream (stream, httpRequest)](#apidoc.element.s3.AWS.HttpClient.prototype.progressStream)
- description and source-code
```javascript
function progressStream(stream, httpRequest) {
  var numBytes = 0;
  var totalBytes = httpRequest.headers['Content-Length'];
  var writer = new WritableStream();
  writer._write = function(chunk, encoding, callback) {
    if (chunk) {
      numBytes += chunk.length;
      stream.emit('sendProgress', {
        loaded: numBytes, total: totalBytes
      });
    }
    callback();
  };
  return writer;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.HttpClient.prototype.sslAgent"></a>[function <span class="apidocSignatureSpan">s3.AWS.HttpClient.prototype.</span>sslAgent ()](#apidoc.element.s3.AWS.HttpClient.prototype.sslAgent)
- description and source-code
```javascript
function sslAgent() {
  var https = require('https');

  if (!AWS.NodeHttpClient.sslAgent) {
    AWS.NodeHttpClient.sslAgent = new https.Agent({rejectUnauthorized: true});
    AWS.NodeHttpClient.sslAgent.setMaxListeners(0);

    // delegate maxSockets to globalAgent
    Object.defineProperty(AWS.NodeHttpClient.sslAgent, 'maxSockets', {
      enumerable: true,
      get: function() { return https.globalAgent.maxSockets; }
    });
  }
  return AWS.NodeHttpClient.sslAgent;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.HttpClient.prototype.writeBody"></a>[function <span class="apidocSignatureSpan">s3.AWS.HttpClient.prototype.</span>writeBody (stream, httpRequest)](#apidoc.element.s3.AWS.HttpClient.prototype.writeBody)
- description and source-code
```javascript
function writeBody(stream, httpRequest) {
  var body = httpRequest.body;

  if (body && WritableStream && ReadableStream) { // progress support
    if (!(body instanceof Stream)) body = AWS.util.buffer.toStream(body);
    body.pipe(this.progressStream(stream, httpRequest));
  }

  if (body instanceof Stream) {
    body.pipe(stream);
  } else if (body) {
    stream.end(body);
  } else {
    stream.end();
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.HttpRequest"></a>[module s3.AWS.HttpRequest](#apidoc.module.s3.AWS.HttpRequest)

#### <a name="apidoc.element.s3.AWS.HttpRequest.HttpRequest"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>HttpRequest (endpoint, region)](#apidoc.element.s3.AWS.HttpRequest.HttpRequest)
- description and source-code
```javascript
function HttpRequest(endpoint, region) {
  endpoint = new AWS.Endpoint(endpoint);
  this.method = 'POST';
  this.path = endpoint.path || '/';
  this.headers = {};
  this.body = '';
  this.endpoint = endpoint;
  this.region = region;
  this.setUserAgent();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.HttpRequest.__super__"></a>[function <span class="apidocSignatureSpan">s3.AWS.HttpRequest.</span>__super__ ()](#apidoc.element.s3.AWS.HttpRequest.__super__)
- description and source-code
```javascript
function Object() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.HttpRequest.prototype"></a>[module s3.AWS.HttpRequest.prototype](#apidoc.module.s3.AWS.HttpRequest.prototype)

#### <a name="apidoc.element.s3.AWS.HttpRequest.prototype.constructor"></a>[function <span class="apidocSignatureSpan">s3.AWS.HttpRequest.prototype.</span>constructor (endpoint, region)](#apidoc.element.s3.AWS.HttpRequest.prototype.constructor)
- description and source-code
```javascript
function HttpRequest(endpoint, region) {
  endpoint = new AWS.Endpoint(endpoint);
  this.method = 'POST';
  this.path = endpoint.path || '/';
  this.headers = {};
  this.body = '';
  this.endpoint = endpoint;
  this.region = region;
  this.setUserAgent();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.HttpRequest.prototype.pathname"></a>[function <span class="apidocSignatureSpan">s3.AWS.HttpRequest.prototype.</span>pathname ()](#apidoc.element.s3.AWS.HttpRequest.prototype.pathname)
- description and source-code
```javascript
function pathname() {
  return this.path.split('?', 1)[0];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.HttpRequest.prototype.search"></a>[function <span class="apidocSignatureSpan">s3.AWS.HttpRequest.prototype.</span>search ()](#apidoc.element.s3.AWS.HttpRequest.prototype.search)
- description and source-code
```javascript
function search() {
  var query = this.path.split('?', 2)[1];
  if (query) {
    query = AWS.util.queryStringParse(query);
    return AWS.util.queryParamsToString(query);
  }
  return '';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.HttpRequest.prototype.setUserAgent"></a>[function <span class="apidocSignatureSpan">s3.AWS.HttpRequest.prototype.</span>setUserAgent ()](#apidoc.element.s3.AWS.HttpRequest.prototype.setUserAgent)
- description and source-code
```javascript
function setUserAgent() {
  var prefix = AWS.util.isBrowser() ? 'X-Amz-' : '';
  this.headers[prefix + 'User-Agent'] = AWS.util.userAgent();
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.HttpResponse"></a>[module s3.AWS.HttpResponse](#apidoc.module.s3.AWS.HttpResponse)

#### <a name="apidoc.element.s3.AWS.HttpResponse.HttpResponse"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>HttpResponse ()](#apidoc.element.s3.AWS.HttpResponse.HttpResponse)
- description and source-code
```javascript
function HttpResponse() {
  this.statusCode = undefined;
  this.headers = {};
  this.body = undefined;
  this.streaming = false;
  this.stream = null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.HttpResponse.__super__"></a>[function <span class="apidocSignatureSpan">s3.AWS.HttpResponse.</span>__super__ ()](#apidoc.element.s3.AWS.HttpResponse.__super__)
- description and source-code
```javascript
function Object() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.HttpResponse.prototype"></a>[module s3.AWS.HttpResponse.prototype](#apidoc.module.s3.AWS.HttpResponse.prototype)

#### <a name="apidoc.element.s3.AWS.HttpResponse.prototype.constructor"></a>[function <span class="apidocSignatureSpan">s3.AWS.HttpResponse.prototype.</span>constructor ()](#apidoc.element.s3.AWS.HttpResponse.prototype.constructor)
- description and source-code
```javascript
function HttpResponse() {
  this.statusCode = undefined;
  this.headers = {};
  this.body = undefined;
  this.streaming = false;
  this.stream = null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.HttpResponse.prototype.createUnbufferedStream"></a>[function <span class="apidocSignatureSpan">s3.AWS.HttpResponse.prototype.</span>createUnbufferedStream ()](#apidoc.element.s3.AWS.HttpResponse.prototype.createUnbufferedStream)
- description and source-code
```javascript
function createUnbufferedStream() {
  this.streaming = true;
  return this.stream;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.IAM"></a>[module s3.AWS.IAM](#apidoc.module.s3.AWS.IAM)

#### <a name="apidoc.element.s3.AWS.IAM.IAM"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>IAM ()](#apidoc.element.s3.AWS.IAM.IAM)
- description and source-code
```javascript
IAM = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.IAM.__super__"></a>[function <span class="apidocSignatureSpan">s3.AWS.IAM.</span>__super__ (config)](#apidoc.element.s3.AWS.IAM.__super__)
- description and source-code
```javascript
function Service(config) {
  if (!this.loadServiceClass) {
    throw AWS.util.error(new Error(),
      'Service must be constructed with 'new\' operator');
  }
  var ServiceClass = this.loadServiceClass(config || {});
  if (ServiceClass) return new ServiceClass(config);
  this.initialize(config);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.IAM.prototype"></a>[module s3.AWS.IAM.prototype](#apidoc.module.s3.AWS.IAM.prototype)

#### <a name="apidoc.element.s3.AWS.IAM.prototype.constructor"></a>[function <span class="apidocSignatureSpan">s3.AWS.IAM.prototype.</span>constructor ()](#apidoc.element.s3.AWS.IAM.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.ImportExport"></a>[module s3.AWS.ImportExport](#apidoc.module.s3.AWS.ImportExport)

#### <a name="apidoc.element.s3.AWS.ImportExport.ImportExport"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>ImportExport ()](#apidoc.element.s3.AWS.ImportExport.ImportExport)
- description and source-code
```javascript
ImportExport = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.ImportExport.__super__"></a>[function <span class="apidocSignatureSpan">s3.AWS.ImportExport.</span>__super__ (config)](#apidoc.element.s3.AWS.ImportExport.__super__)
- description and source-code
```javascript
function Service(config) {
  if (!this.loadServiceClass) {
    throw AWS.util.error(new Error(),
      'Service must be constructed with 'new\' operator');
  }
  var ServiceClass = this.loadServiceClass(config || {});
  if (ServiceClass) return new ServiceClass(config);
  this.initialize(config);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.ImportExport.prototype"></a>[module s3.AWS.ImportExport.prototype](#apidoc.module.s3.AWS.ImportExport.prototype)

#### <a name="apidoc.element.s3.AWS.ImportExport.prototype.constructor"></a>[function <span class="apidocSignatureSpan">s3.AWS.ImportExport.prototype.</span>constructor ()](#apidoc.element.s3.AWS.ImportExport.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.JSON"></a>[module s3.AWS.JSON](#apidoc.module.s3.AWS.JSON)

#### <a name="apidoc.element.s3.AWS.JSON.Builder"></a>[function <span class="apidocSignatureSpan">s3.AWS.JSON.</span>Builder ()](#apidoc.element.s3.AWS.JSON.Builder)
- description and source-code
```javascript
function JsonBuilder() { }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.JSON.Parser"></a>[function <span class="apidocSignatureSpan">s3.AWS.JSON.</span>Parser ()](#apidoc.element.s3.AWS.JSON.Parser)
- description and source-code
```javascript
function JsonParser() { }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.JSON.Builder.prototype"></a>[module s3.AWS.JSON.Builder.prototype](#apidoc.module.s3.AWS.JSON.Builder.prototype)

#### <a name="apidoc.element.s3.AWS.JSON.Builder.prototype.build"></a>[function <span class="apidocSignatureSpan">s3.AWS.JSON.Builder.prototype.</span>build (value, shape)](#apidoc.element.s3.AWS.JSON.Builder.prototype.build)
- description and source-code
```javascript
build = function (value, shape) {
  return JSON.stringify(translate(value, shape));
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.JSON.Parser.prototype"></a>[module s3.AWS.JSON.Parser.prototype](#apidoc.module.s3.AWS.JSON.Parser.prototype)

#### <a name="apidoc.element.s3.AWS.JSON.Parser.prototype.parse"></a>[function <span class="apidocSignatureSpan">s3.AWS.JSON.Parser.prototype.</span>parse (value, shape)](#apidoc.element.s3.AWS.JSON.Parser.prototype.parse)
- description and source-code
```javascript
parse = function (value, shape) {
  return translate(JSON.parse(value), shape);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.KMS"></a>[module s3.AWS.KMS](#apidoc.module.s3.AWS.KMS)

#### <a name="apidoc.element.s3.AWS.KMS.KMS"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>KMS ()](#apidoc.element.s3.AWS.KMS.KMS)
- description and source-code
```javascript
KMS = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.KMS.__super__"></a>[function <span class="apidocSignatureSpan">s3.AWS.KMS.</span>__super__ (config)](#apidoc.element.s3.AWS.KMS.__super__)
- description and source-code
```javascript
function Service(config) {
  if (!this.loadServiceClass) {
    throw AWS.util.error(new Error(),
      'Service must be constructed with 'new\' operator');
  }
  var ServiceClass = this.loadServiceClass(config || {});
  if (ServiceClass) return new ServiceClass(config);
  this.initialize(config);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.KMS.prototype"></a>[module s3.AWS.KMS.prototype](#apidoc.module.s3.AWS.KMS.prototype)

#### <a name="apidoc.element.s3.AWS.KMS.prototype.constructor"></a>[function <span class="apidocSignatureSpan">s3.AWS.KMS.prototype.</span>constructor ()](#apidoc.element.s3.AWS.KMS.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.Kinesis"></a>[module s3.AWS.Kinesis](#apidoc.module.s3.AWS.Kinesis)

#### <a name="apidoc.element.s3.AWS.Kinesis.Kinesis"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>Kinesis ()](#apidoc.element.s3.AWS.Kinesis.Kinesis)
- description and source-code
```javascript
Kinesis = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Kinesis.__super__"></a>[function <span class="apidocSignatureSpan">s3.AWS.Kinesis.</span>__super__ (config)](#apidoc.element.s3.AWS.Kinesis.__super__)
- description and source-code
```javascript
function Service(config) {
  if (!this.loadServiceClass) {
    throw AWS.util.error(new Error(),
      'Service must be constructed with 'new\' operator');
  }
  var ServiceClass = this.loadServiceClass(config || {});
  if (ServiceClass) return new ServiceClass(config);
  this.initialize(config);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.Kinesis.prototype"></a>[module s3.AWS.Kinesis.prototype](#apidoc.module.s3.AWS.Kinesis.prototype)

#### <a name="apidoc.element.s3.AWS.Kinesis.prototype.constructor"></a>[function <span class="apidocSignatureSpan">s3.AWS.Kinesis.prototype.</span>constructor ()](#apidoc.element.s3.AWS.Kinesis.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.Lambda"></a>[module s3.AWS.Lambda](#apidoc.module.s3.AWS.Lambda)

#### <a name="apidoc.element.s3.AWS.Lambda.Lambda"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>Lambda ()](#apidoc.element.s3.AWS.Lambda.Lambda)
- description and source-code
```javascript
Lambda = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Lambda.__super__"></a>[function <span class="apidocSignatureSpan">s3.AWS.Lambda.</span>__super__ (config)](#apidoc.element.s3.AWS.Lambda.__super__)
- description and source-code
```javascript
function Service(config) {
  if (!this.loadServiceClass) {
    throw AWS.util.error(new Error(),
      'Service must be constructed with 'new\' operator');
  }
  var ServiceClass = this.loadServiceClass(config || {});
  if (ServiceClass) return new ServiceClass(config);
  this.initialize(config);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.Lambda.prototype"></a>[module s3.AWS.Lambda.prototype](#apidoc.module.s3.AWS.Lambda.prototype)

#### <a name="apidoc.element.s3.AWS.Lambda.prototype.constructor"></a>[function <span class="apidocSignatureSpan">s3.AWS.Lambda.prototype.</span>constructor ()](#apidoc.element.s3.AWS.Lambda.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.MetadataService"></a>[module s3.AWS.MetadataService](#apidoc.module.s3.AWS.MetadataService)

#### <a name="apidoc.element.s3.AWS.MetadataService.MetadataService"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>MetadataService (options)](#apidoc.element.s3.AWS.MetadataService.MetadataService)
- description and source-code
```javascript
function MetadataService(options) {
  AWS.util.update(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.MetadataService.__super__"></a>[function <span class="apidocSignatureSpan">s3.AWS.MetadataService.</span>__super__ ()](#apidoc.element.s3.AWS.MetadataService.__super__)
- description and source-code
```javascript
function Object() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.MetadataService.prototype"></a>[module s3.AWS.MetadataService.prototype](#apidoc.module.s3.AWS.MetadataService.prototype)

#### <a name="apidoc.element.s3.AWS.MetadataService.prototype.constructor"></a>[function <span class="apidocSignatureSpan">s3.AWS.MetadataService.prototype.</span>constructor (options)](#apidoc.element.s3.AWS.MetadataService.prototype.constructor)
- description and source-code
```javascript
function MetadataService(options) {
  AWS.util.update(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.MetadataService.prototype.loadCredentials"></a>[function <span class="apidocSignatureSpan">s3.AWS.MetadataService.prototype.</span>loadCredentials (callback)](#apidoc.element.s3.AWS.MetadataService.prototype.loadCredentials)
- description and source-code
```javascript
function loadCredentials(callback) {
  var self = this;
  var basePath = '/latest/meta-data/iam/security-credentials/';
  self.request(basePath, function (err, roleName) {
    if (err) callback(err);
    else {
      roleName = roleName.split('\n')[0]; // grab first (and only) role
      self.request(basePath + roleName, function (credErr, credData) {
        if (credErr) callback(credErr);
        else {
          try {
            var credentials = JSON.parse(credData);
            callback(null, credentials);
          } catch (parseError) {
            callback(parseError);
          }
        }
      });
    }
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.MetadataService.prototype.request"></a>[function <span class="apidocSignatureSpan">s3.AWS.MetadataService.prototype.</span>request (path, callback)](#apidoc.element.s3.AWS.MetadataService.prototype.request)
- description and source-code
```javascript
function request(path, callback) {
  path = path || '/';

  var data = '';
  var http = AWS.HttpClient.getInstance();
  var httpRequest = new AWS.HttpRequest('http://' + this.host + path);
  httpRequest.method = 'GET';

  http.handleRequest(httpRequest, this.httpOptions, function(httpResponse) {
    httpResponse.on('data', function(chunk) { data += chunk.toString(); });
    httpResponse.on('end', function() { callback(null, data); });
  }, callback);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.Model"></a>[module s3.AWS.Model](#apidoc.module.s3.AWS.Model)

#### <a name="apidoc.element.s3.AWS.Model.Api"></a>[function <span class="apidocSignatureSpan">s3.AWS.Model.</span>Api (api, options)](#apidoc.element.s3.AWS.Model.Api)
- description and source-code
```javascript
function Api(api, options) {
  api = api || {};
  options = options || {};
  options.api = this;

  api.metadata = api.metadata || {};

  property(this, 'isApi', true, false);
  property(this, 'apiVersion', api.metadata.apiVersion);
  property(this, 'endpointPrefix', api.metadata.endpointPrefix);
  property(this, 'signingName', api.metadata.signingName);
  property(this, 'globalEndpoint', api.metadata.globalEndpoint);
  property(this, 'signatureVersion', api.metadata.signatureVersion);
  property(this, 'jsonVersion', api.metadata.jsonVersion);
  property(this, 'targetPrefix', api.metadata.targetPrefix);
  property(this, 'protocol', api.metadata.protocol);
  property(this, 'timestampFormat', api.metadata.timestampFormat);
  property(this, 'xmlNamespaceUri', api.metadata.xmlNamespace);
  property(this, 'abbreviation', api.metadata.serviceAbbreviation);
  property(this, 'fullName', api.metadata.serviceFullName);

  memoizedProperty(this, 'className', function() {
    var name = api.metadata.serviceAbbreviation || api.metadata.serviceFullName;
    if (!name) return null;

    name = name.replace(/^Amazon|AWS\s*|\(.*|\s+|\W+/g, '');
    if (name === 'ElasticLoadBalancing') name = 'ELB';
    return name;
  });

  property(this, 'operations', new Collection(api.operations, options, function(name, operation) {
    return new Operation(name, operation, options);
  }, util.string.lowerFirst));

  property(this, 'shapes', new Collection(api.shapes, options, function(name, shape) {
    return Shape.create(shape, options);
  }));

  property(this, 'paginators', new Collection(api.paginators, options, function(name, paginator) {
    return new Paginator(name, paginator, options);
  }));

  property(this, 'waiters', new Collection(api.waiters, options, function(name, waiter) {
    return new ResourceWaiter(name, waiter, options);
  }, util.string.lowerFirst));

  if (options.documentation) {
    property(this, 'documentation', api.documentation);
    property(this, 'documentationUrl', api.documentationUrl);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Model.Operation"></a>[function <span class="apidocSignatureSpan">s3.AWS.Model.</span>Operation (name, operation, options)](#apidoc.element.s3.AWS.Model.Operation)
- description and source-code
```javascript
function Operation(name, operation, options) {
  options = options || {};

  property(this, 'name', operation.name || name);
  property(this, 'api', options.api, false);

  operation.http = operation.http || {};
  property(this, 'httpMethod', operation.http.method || 'POST');
  property(this, 'httpPath', operation.http.requestUri || '/');

  memoizedProperty(this, 'input', function() {
    if (!operation.input) {
      return new Shape.create({type: 'structure'}, options);
    }
    return Shape.create(operation.input, options);
  });

  memoizedProperty(this, 'output', function() {
    if (!operation.output) {
      return new Shape.create({type: 'structure'}, options);
    }
    return Shape.create(operation.output, options);
  });

  memoizedProperty(this, 'errors', function() {
    var list = [];
    if (!operation.errors) return null;

    for (var i = 0; i < operation.errors.length; i++) {
      list.push(Shape.create(operation.errors[i], options));
    }

    return list;
  });

  memoizedProperty(this, 'paginator', function() {
    return options.api.paginators[name];
  });

  if (options.documentation) {
    property(this, 'documentation', operation.documentation);
    property(this, 'documentationUrl', operation.documentationUrl);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Model.Paginator"></a>[function <span class="apidocSignatureSpan">s3.AWS.Model.</span>Paginator (name, paginator)](#apidoc.element.s3.AWS.Model.Paginator)
- description and source-code
```javascript
function Paginator(name, paginator) {
  property(this, 'inputToken', paginator.input_token);
  property(this, 'limitKey', paginator.limit_key);
  property(this, 'moreResults', paginator.more_results);
  property(this, 'outputToken', paginator.output_token);
  property(this, 'resultKey', paginator.result_key);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Model.ResourceWaiter"></a>[function <span class="apidocSignatureSpan">s3.AWS.Model.</span>ResourceWaiter (name, waiter, options)](#apidoc.element.s3.AWS.Model.ResourceWaiter)
- description and source-code
```javascript
function ResourceWaiter(name, waiter, options) {
  options = options || {};

  function InnerResourceWaiter() {
    property(this, 'name', name);
    property(this, 'api', options.api, false);

    if (waiter.operation) {
      property(this, 'operation', util.string.lowerFirst(waiter.operation));
    }

    var self = this, map = {
      ignoreErrors: 'ignore_errors',
      successType: 'success_type',
      successValue: 'success_value',
      successPath: 'success_path',
      acceptorType: 'acceptor_type',
      acceptorValue: 'acceptor_value',
      acceptorPath: 'acceptor_path',
      failureType: 'failure_type',
      failureValue: 'failure_value',
      failurePath: 'success_path',
      interval: 'interval',
      maxAttempts: 'max_attempts'
    };
    Object.keys(map).forEach(function(key) {
      var value = waiter[map[key]];
      if (value) property(self, key, value);
    });
  }

  if (options.api) {
    var proto = null;
    if (waiter['extends']) {
      proto = options.api.waiters[waiter['extends']];
    } else if (name !== '__default__') {
      proto = options.api.waiters['__default__'];
    }

    if (proto) InnerResourceWaiter.prototype = proto;
  }

  return new InnerResourceWaiter();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Model.Shape"></a>[function <span class="apidocSignatureSpan">s3.AWS.Model.</span>Shape (shape, options, memberName)](#apidoc.element.s3.AWS.Model.Shape)
- description and source-code
```javascript
function Shape(shape, options, memberName) {
  options = options || {};

  property(this, 'shape', shape.shape);
  property(this, 'api', options.api, false);
  property(this, 'type', shape.type);
  property(this, 'location', shape.location || 'body');
  property(this, 'name', this.name || shape.xmlName || shape.queryName ||
    shape.locationName || memberName);
  property(this, 'isStreaming', shape.streaming || false);
  property(this, 'isComposite', shape.isComposite || false);
  property(this, 'isShape', true, false);
  property(this, 'isQueryName', shape.queryName ? true : false, false);

  if (options.documentation) {
    property(this, 'documentation', shape.documentation);
    property(this, 'documentationUrl', shape.documentationUrl);
  }

  if (shape.xmlAttribute) {
    property(this, 'isXmlAttribute', shape.xmlAttribute || false);
  }

  // type conversion and parsing
  property(this, 'defaultValue', null);
  this.toWireFormat = function(value) {
    if (value === null || value === undefined) return '';
    return value;
  };
  this.toType = function(value) { return value; };
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.NodeHttpClient"></a>[module s3.AWS.NodeHttpClient](#apidoc.module.s3.AWS.NodeHttpClient)

#### <a name="apidoc.element.s3.AWS.NodeHttpClient.NodeHttpClient"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>NodeHttpClient ()](#apidoc.element.s3.AWS.NodeHttpClient.NodeHttpClient)
- description and source-code
```javascript
NodeHttpClient = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.NodeHttpClient.__super__"></a>[function <span class="apidocSignatureSpan">s3.AWS.NodeHttpClient.</span>__super__ ()](#apidoc.element.s3.AWS.NodeHttpClient.__super__)
- description and source-code
```javascript
function Object() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.OpsWorks"></a>[module s3.AWS.OpsWorks](#apidoc.module.s3.AWS.OpsWorks)

#### <a name="apidoc.element.s3.AWS.OpsWorks.OpsWorks"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>OpsWorks ()](#apidoc.element.s3.AWS.OpsWorks.OpsWorks)
- description and source-code
```javascript
OpsWorks = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.OpsWorks.__super__"></a>[function <span class="apidocSignatureSpan">s3.AWS.OpsWorks.</span>__super__ (config)](#apidoc.element.s3.AWS.OpsWorks.__super__)
- description and source-code
```javascript
function Service(config) {
  if (!this.loadServiceClass) {
    throw AWS.util.error(new Error(),
      'Service must be constructed with 'new\' operator');
  }
  var ServiceClass = this.loadServiceClass(config || {});
  if (ServiceClass) return new ServiceClass(config);
  this.initialize(config);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.OpsWorks.prototype"></a>[module s3.AWS.OpsWorks.prototype](#apidoc.module.s3.AWS.OpsWorks.prototype)

#### <a name="apidoc.element.s3.AWS.OpsWorks.prototype.constructor"></a>[function <span class="apidocSignatureSpan">s3.AWS.OpsWorks.prototype.</span>constructor ()](#apidoc.element.s3.AWS.OpsWorks.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.ParamValidator"></a>[module s3.AWS.ParamValidator](#apidoc.module.s3.AWS.ParamValidator)

#### <a name="apidoc.element.s3.AWS.ParamValidator.ParamValidator"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>ParamValidator ()](#apidoc.element.s3.AWS.ParamValidator.ParamValidator)
- description and source-code
```javascript
ParamValidator = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.ParamValidator.__super__"></a>[function <span class="apidocSignatureSpan">s3.AWS.ParamValidator.</span>__super__ ()](#apidoc.element.s3.AWS.ParamValidator.__super__)
- description and source-code
```javascript
function Object() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.ParamValidator.prototype"></a>[module s3.AWS.ParamValidator.prototype](#apidoc.module.s3.AWS.ParamValidator.prototype)

#### <a name="apidoc.element.s3.AWS.ParamValidator.prototype.constructor"></a>[function <span class="apidocSignatureSpan">s3.AWS.ParamValidator.prototype.</span>constructor ()](#apidoc.element.s3.AWS.ParamValidator.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.ParamValidator.prototype.fail"></a>[function <span class="apidocSignatureSpan">s3.AWS.ParamValidator.prototype.</span>fail (code, message)](#apidoc.element.s3.AWS.ParamValidator.prototype.fail)
- description and source-code
```javascript
function fail(code, message) {
  this.errors.push(AWS.util.error(new Error(message), {code: code}));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.ParamValidator.prototype.validate"></a>[function <span class="apidocSignatureSpan">s3.AWS.ParamValidator.prototype.</span>validate (shape, params, context)](#apidoc.element.s3.AWS.ParamValidator.prototype.validate)
- description and source-code
```javascript
function validate(shape, params, context) {
  this.errors = [];
  this.validateMember(shape, params || {}, context || 'params');

  if (this.errors.length > 1) {
    var msg = this.errors.join('\n* ');
    if (this.errors.length > 1) {
      msg = 'There were ' + this.errors.length +
            ' validation errors:\n* ' + msg;
      throw AWS.util.error(new Error(msg),
        {code: 'MultipleValidationErrors', errors: this.errors});
    }
  } else if (this.errors.length === 1) {
    throw this.errors[0];
  } else {
    return true;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.ParamValidator.prototype.validateList"></a>[function <span class="apidocSignatureSpan">s3.AWS.ParamValidator.prototype.</span>validateList (shape, params, context)](#apidoc.element.s3.AWS.ParamValidator.prototype.validateList)
- description and source-code
```javascript
function validateList(shape, params, context) {
  this.validateType(context, params, [Array]);

  // validate array members
  for (var i = 0; i < params.length; i++) {
    this.validateMember(shape.member, params[i], context + '[' + i + ']');
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.ParamValidator.prototype.validateMap"></a>[function <span class="apidocSignatureSpan">s3.AWS.ParamValidator.prototype.</span>validateMap (shape, params, context)](#apidoc.element.s3.AWS.ParamValidator.prototype.validateMap)
- description and source-code
```javascript
function validateMap(shape, params, context) {
  this.validateType(context, params, ['object'], 'map');

  for (var param in params) {
    if (!params.hasOwnProperty(param)) continue;
    this.validateMember(shape.value, params[param],
                        context + '[\'' + param + '\']');
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.ParamValidator.prototype.validateMember"></a>[function <span class="apidocSignatureSpan">s3.AWS.ParamValidator.prototype.</span>validateMember (shape, param, context)](#apidoc.element.s3.AWS.ParamValidator.prototype.validateMember)
- description and source-code
```javascript
function validateMember(shape, param, context) {
  switch (shape.type) {
    case 'structure':
      return this.validateStructure(shape, param, context);
    case 'list':
      return this.validateList(shape, param, context);
    case 'map':
      return this.validateMap(shape, param, context);
    default:
      return this.validateScalar(shape, param, context);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.ParamValidator.prototype.validateNumber"></a>[function <span class="apidocSignatureSpan">s3.AWS.ParamValidator.prototype.</span>validateNumber (context, value)](#apidoc.element.s3.AWS.ParamValidator.prototype.validateNumber)
- description and source-code
```javascript
function validateNumber(context, value) {
  if (value === null || value === undefined) return;
  if (typeof value === 'string') {
    var castedValue = parseFloat(value);
    if (castedValue.toString() === value) value = castedValue;
  }
  this.validateType(context, value, ['number']);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.ParamValidator.prototype.validatePayload"></a>[function <span class="apidocSignatureSpan">s3.AWS.ParamValidator.prototype.</span>validatePayload (context, value)](#apidoc.element.s3.AWS.ParamValidator.prototype.validatePayload)
- description and source-code
```javascript
function validatePayload(context, value) {
  if (value === null || value === undefined) return;
  if (typeof value === 'string') return;
  if (value && typeof value.byteLength === 'number') return; // typed arrays
  if (AWS.util.isNode()) { // special check for buffer/stream in Node.js
    var Stream = AWS.util.nodeRequire('stream').Stream;
    if (AWS.util.Buffer.isBuffer(value) || value instanceof Stream) return;
  }

  var types = ['Buffer', 'Stream', 'File', 'Blob', 'ArrayBuffer', 'DataView'];
  if (value) {
    for (var i = 0; i < types.length; i++) {
      if (AWS.util.isType(value, types[i])) return;
      if (AWS.util.typeName(value.constructor) === types[i]) return;
    }
  }

  this.fail('InvalidParameterType', 'Expected ' + context + ' to be a ' +
    'string, Buffer, Stream, Blob, or typed array object');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.ParamValidator.prototype.validateScalar"></a>[function <span class="apidocSignatureSpan">s3.AWS.ParamValidator.prototype.</span>validateScalar (shape, value, context)](#apidoc.element.s3.AWS.ParamValidator.prototype.validateScalar)
- description and source-code
```javascript
function validateScalar(shape, value, context) {
  switch (shape.type) {
    case null:
    case undefined:
    case 'string':
      return this.validateType(context, value, ['string']);
    case 'base64':
    case 'binary':
      return this.validatePayload(context, value);
    case 'integer':
    case 'float':
      return this.validateNumber(context, value);
    case 'boolean':
      return this.validateType(context, value, ['boolean']);
    case 'timestamp':
      return this.validateType(context, value, [Date,
        /^\d{4}-\d{2}-\d{2}T\d{2}:\d{2}:\d{2}(\.\d+)?Z$/, 'number'],
        'Date object, ISO-8601 string, or a UNIX timestamp');
    default:
      return this.fail('UnkownType', 'Unhandled type ' +
                       shape.type + ' for ' + context);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.ParamValidator.prototype.validateStructure"></a>[function <span class="apidocSignatureSpan">s3.AWS.ParamValidator.prototype.</span>validateStructure (shape, params, context)](#apidoc.element.s3.AWS.ParamValidator.prototype.validateStructure)
- description and source-code
```javascript
function validateStructure(shape, params, context) {
  this.validateType(context, params, ['object'], 'structure');

  var paramName;
  for (var i = 0; shape.required && i < shape.required.length; i++) {
    paramName = shape.required[i];
    var value = params[paramName];
    if (value === undefined || value === null) {
      this.fail('MissingRequiredParameter',
        'Missing required key \'' + paramName + '\' in ' + context);
    }
  }

  // validate hash members
  for (paramName in params) {
    if (!params.hasOwnProperty(paramName)) continue;

    var paramValue = params[paramName],
        memberShape = shape.members[paramName];

    if (memberShape !== undefined) {
      var memberContext = [context, paramName].join('.');
      this.validateMember(memberShape, paramValue, memberContext);
    } else {
      this.fail('UnexpectedParameter',
        'Unexpected key \'' + paramName + '\' found in ' + context);
    }
  }

  return true;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.ParamValidator.prototype.validateType"></a>[function <span class="apidocSignatureSpan">s3.AWS.ParamValidator.prototype.</span>validateType (context, value, acceptedTypes, type)](#apidoc.element.s3.AWS.ParamValidator.prototype.validateType)
- description and source-code
```javascript
function validateType(context, value, acceptedTypes, type) {
  if (value === null || value === undefined) return;

  var foundInvalidType = false;
  for (var i = 0; i < acceptedTypes.length; i++) {
    if (typeof acceptedTypes[i] === 'string') {
      if (typeof value === acceptedTypes[i]) return;
    } else if (acceptedTypes[i] instanceof RegExp) {
      if ((value || '').toString().match(acceptedTypes[i])) return;
    } else {
      if (value instanceof acceptedTypes[i]) return;
      if (AWS.util.isType(value, acceptedTypes[i])) return;
      if (!type && !foundInvalidType) acceptedTypes = acceptedTypes.slice();
      acceptedTypes[i] = AWS.util.typeName(acceptedTypes[i]);
    }
    foundInvalidType = true;
  }

  var acceptedType = type;
  if (!acceptedType) {
    acceptedType = acceptedTypes.join(', ').replace(/,([^,]+)$/, ', or$1');
  }

  var vowel = acceptedType.match(/^[aeiou]/i) ? 'n' : '';
  this.fail('InvalidParameterType', 'Expected ' + context + ' to be a' +
            vowel + ' ' + acceptedType);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.RDS"></a>[module s3.AWS.RDS](#apidoc.module.s3.AWS.RDS)

#### <a name="apidoc.element.s3.AWS.RDS.RDS"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>RDS ()](#apidoc.element.s3.AWS.RDS.RDS)
- description and source-code
```javascript
RDS = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.RDS.__super__"></a>[function <span class="apidocSignatureSpan">s3.AWS.RDS.</span>__super__ (config)](#apidoc.element.s3.AWS.RDS.__super__)
- description and source-code
```javascript
function Service(config) {
  if (!this.loadServiceClass) {
    throw AWS.util.error(new Error(),
      'Service must be constructed with 'new\' operator');
  }
  var ServiceClass = this.loadServiceClass(config || {});
  if (ServiceClass) return new ServiceClass(config);
  this.initialize(config);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.RDS.prototype"></a>[module s3.AWS.RDS.prototype](#apidoc.module.s3.AWS.RDS.prototype)

#### <a name="apidoc.element.s3.AWS.RDS.prototype.constructor"></a>[function <span class="apidocSignatureSpan">s3.AWS.RDS.prototype.</span>constructor ()](#apidoc.element.s3.AWS.RDS.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.Redshift"></a>[module s3.AWS.Redshift](#apidoc.module.s3.AWS.Redshift)

#### <a name="apidoc.element.s3.AWS.Redshift.Redshift"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>Redshift ()](#apidoc.element.s3.AWS.Redshift.Redshift)
- description and source-code
```javascript
Redshift = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Redshift.__super__"></a>[function <span class="apidocSignatureSpan">s3.AWS.Redshift.</span>__super__ (config)](#apidoc.element.s3.AWS.Redshift.__super__)
- description and source-code
```javascript
function Service(config) {
  if (!this.loadServiceClass) {
    throw AWS.util.error(new Error(),
      'Service must be constructed with 'new\' operator');
  }
  var ServiceClass = this.loadServiceClass(config || {});
  if (ServiceClass) return new ServiceClass(config);
  this.initialize(config);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.Redshift.prototype"></a>[module s3.AWS.Redshift.prototype](#apidoc.module.s3.AWS.Redshift.prototype)

#### <a name="apidoc.element.s3.AWS.Redshift.prototype.constructor"></a>[function <span class="apidocSignatureSpan">s3.AWS.Redshift.prototype.</span>constructor ()](#apidoc.element.s3.AWS.Redshift.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.Request"></a>[module s3.AWS.Request](#apidoc.module.s3.AWS.Request)

#### <a name="apidoc.element.s3.AWS.Request.Request"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>Request (service, operation, params)](#apidoc.element.s3.AWS.Request.Request)
- description and source-code
```javascript
function Request(service, operation, params) {
  var endpoint = service.endpoint;
  var region = service.config.region;

  // global endpoints sign as us-east-1
  if (service.isGlobalEndpoint) region = 'us-east-1';

  this.domain = domain && domain.active;
  this.service = service;
  this.operation = operation;
  this.params = params || {};
  this.httpRequest = new AWS.HttpRequest(endpoint, region);
  this.startTime = AWS.util.date.getDate();

  this.response = new AWS.Response(this);
  this._asm = new AcceptorStateMachine(fsm.states, 'validate');

  AWS.SequentialExecutor.call(this);
  this.emit = this.emitEvent;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Request.__super__"></a>[function <span class="apidocSignatureSpan">s3.AWS.Request.</span>__super__ ()](#apidoc.element.s3.AWS.Request.__super__)
- description and source-code
```javascript
function Object() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.Request.prototype"></a>[module s3.AWS.Request.prototype](#apidoc.module.s3.AWS.Request.prototype)

#### <a name="apidoc.element.s3.AWS.Request.prototype.abort"></a>[function <span class="apidocSignatureSpan">s3.AWS.Request.prototype.</span>abort ()](#apidoc.element.s3.AWS.Request.prototype.abort)
- description and source-code
```javascript
function abort() {
  this.removeAllListeners('validateResponse');
  this.removeAllListeners('extractError');
  this.on('validateResponse', function addAbortedError(resp) {
    resp.error = AWS.util.error(new Error('Request aborted by user'), {
       code: 'RequestAbortedError', retryable: false
    });
  });

  if (this.httpRequest.stream) { // abort HTTP stream
    this.httpRequest.stream.abort();
    if (this.httpRequest._abortCallback) {
       this.httpRequest._abortCallback();
    } else {
      this.removeAllListeners('send'); // haven't sent yet, so let's not
    }
  }

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Request.prototype.addListener"></a>[function <span class="apidocSignatureSpan">s3.AWS.Request.prototype.</span>addListener (eventName, listener)](#apidoc.element.s3.AWS.Request.prototype.addListener)
- description and source-code
```javascript
function on(eventName, listener) {
  if (this._events[eventName]) {
    this._events[eventName].push(listener);
  } else {
    this._events[eventName] = [listener];
  }
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Request.prototype.addListeners"></a>[function <span class="apidocSignatureSpan">s3.AWS.Request.prototype.</span>addListeners (listeners)](#apidoc.element.s3.AWS.Request.prototype.addListeners)
- description and source-code
```javascript
function addListeners(listeners) {
  var self = this;

  // extract listeners if parameter is an SequentialExecutor object
  if (listeners._events) listeners = listeners._events;

  AWS.util.each(listeners, function(event, callbacks) {
    if (typeof callbacks === 'function') callbacks = [callbacks];
    AWS.util.arrayEach(callbacks, function(callback) {
      self.on(event, callback);
    });
  });

  return self;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Request.prototype.addNamedAsyncListener"></a>[function <span class="apidocSignatureSpan">s3.AWS.Request.prototype.</span>addNamedAsyncListener (name, eventName, callback)](#apidoc.element.s3.AWS.Request.prototype.addNamedAsyncListener)
- description and source-code
```javascript
function addNamedAsyncListener(name, eventName, callback) {
  callback._isAsync = true;
  return this.addNamedListener(name, eventName, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Request.prototype.addNamedListener"></a>[function <span class="apidocSignatureSpan">s3.AWS.Request.prototype.</span>addNamedListener (name, eventName, callback)](#apidoc.element.s3.AWS.Request.prototype.addNamedListener)
- description and source-code
```javascript
function addNamedListener(name, eventName, callback) {
  this[name] = callback;
  this.addListener(eventName, callback);
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Request.prototype.addNamedListeners"></a>[function <span class="apidocSignatureSpan">s3.AWS.Request.prototype.</span>addNamedListeners (callback)](#apidoc.element.s3.AWS.Request.prototype.addNamedListeners)
- description and source-code
```javascript
function addNamedListeners(callback) {
  var self = this;
  callback(
    function() {
      self.addNamedListener.apply(self, arguments);
    },
    function() {
      self.addNamedAsyncListener.apply(self, arguments);
    }
  );
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Request.prototype.build"></a>[function <span class="apidocSignatureSpan">s3.AWS.Request.prototype.</span>build (callback)](#apidoc.element.s3.AWS.Request.prototype.build)
- description and source-code
```javascript
function build(callback) {
  return this.runTo('send', callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Request.prototype.buildAsGet"></a>[function <span class="apidocSignatureSpan">s3.AWS.Request.prototype.</span>buildAsGet (request)](#apidoc.element.s3.AWS.Request.prototype.buildAsGet)
- description and source-code
```javascript
function buildAsGet(request) {
  request.httpRequest.method = 'GET';
  request.httpRequest.path = request.service.endpoint.path +
                             '?' + request.httpRequest.body;
  request.httpRequest.body = '';

  // don't need these headers on a GET request
  delete request.httpRequest.headers['Content-Length'];
  delete request.httpRequest.headers['Content-Type'];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Request.prototype.callListeners"></a>[function <span class="apidocSignatureSpan">s3.AWS.Request.prototype.</span>callListeners (listeners, args, doneCallback)](#apidoc.element.s3.AWS.Request.prototype.callListeners)
- description and source-code
```javascript
function callListeners(listeners, args, doneCallback) {
  var self = this;
  function callNextListener(err) {
    if (err) {
      doneCallback.call(self, err);
    } else {
      self.callListeners(listeners, args, doneCallback);
    }
  }

  while (listeners.length > 0) {
    var listener = listeners.shift();
    if (listener._isAsync) { // asynchronous listener
      listener.apply(self, args.concat([callNextListener]));
      return; // stop here, callNextListener will continue
    } else { // synchronous listener
      listener.apply(self, args);
    }
  }

  doneCallback.call(self);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Request.prototype.constructor"></a>[function <span class="apidocSignatureSpan">s3.AWS.Request.prototype.</span>constructor (service, operation, params)](#apidoc.element.s3.AWS.Request.prototype.constructor)
- description and source-code
```javascript
function Request(service, operation, params) {
  var endpoint = service.endpoint;
  var region = service.config.region;

  // global endpoints sign as us-east-1
  if (service.isGlobalEndpoint) region = 'us-east-1';

  this.domain = domain && domain.active;
  this.service = service;
  this.operation = operation;
  this.params = params || {};
  this.httpRequest = new AWS.HttpRequest(endpoint, region);
  this.startTime = AWS.util.date.getDate();

  this.response = new AWS.Response(this);
  this._asm = new AcceptorStateMachine(fsm.states, 'validate');

  AWS.SequentialExecutor.call(this);
  this.emit = this.emitEvent;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Request.prototype.createReadStream"></a>[function <span class="apidocSignatureSpan">s3.AWS.Request.prototype.</span>createReadStream ()](#apidoc.element.s3.AWS.Request.prototype.createReadStream)
- description and source-code
```javascript
function createReadStream() {
  var streams = AWS.util.nodeRequire('stream');
  var req = this;
  var stream = null;
  var legacyStreams = false;

  if (AWS.HttpClient.streamsApiVersion === 2) {
    stream = new streams.Readable();
    stream._read = function() {};
  } else {
    stream = new streams.Stream();
    stream.readable = true;
  }

  stream.sent = false;
  stream.on('newListener', function(event) {
    if (!stream.sent && (event === 'data' || event === 'readable')) {
      if (event === 'data') legacyStreams = true;
      stream.sent = true;
      process.nextTick(function() { req.send(function() { }); });
    }
  });

  this.on('httpHeaders', function streamHeaders(statusCode, headers, resp) {
    if (statusCode < 300) {
      req.removeListener('httpData', AWS.EventListeners.Core.HTTP_DATA);
      req.removeListener('httpError', AWS.EventListeners.Core.HTTP_ERROR);
      req.on('httpError', function streamHttpError(error, resp) {
        resp.error = error;
        resp.error.retryable = false;
      });

      var httpStream = resp.httpResponse.createUnbufferedStream();
      if (legacyStreams) {
        httpStream.on('data', function(arg) {
          stream.emit('data', arg);
        });
        httpStream.on('end', function() {
          stream.emit('end');
        });
      } else {
        httpStream.on('readable', function() {
          var chunk;
          do {
            chunk = httpStream.read();
            if (chunk !== null) stream.push(chunk);
          } while (chunk !== null);
          stream.read(0);
        });
        httpStream.on('end', function() {
          stream.push(null);
        });
      }

      httpStream.on('error', function(err) {
        stream.emit('error', err);
      });
    }
  });

  this.on('error', function(err) {
    stream.emit('error', err);
  });

  return stream;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Request.prototype.eachItem"></a>[function <span class="apidocSignatureSpan">s3.AWS.Request.prototype.</span>eachItem (callback)](#apidoc.element.s3.AWS.Request.prototype.eachItem)
- description and source-code
```javascript
function eachItem(callback) {
  var self = this;
  function wrappedCallback(err, data) {
    if (err) return callback(err, null);
    if (data === null) return callback(null, null);

    var config = self.service.paginationConfig(self.operation);
    var resultKey = config.resultKey;
    if (Array.isArray(resultKey)) resultKey = resultKey[0];
    var results = AWS.util.jamespath.query(resultKey, data);
    AWS.util.arrayEach(results, function(result) {
      AWS.util.arrayEach(result, function(item) { callback(null, item); });
    });
  }

  this.eachPage(wrappedCallback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Request.prototype.eachPage"></a>[function <span class="apidocSignatureSpan">s3.AWS.Request.prototype.</span>eachPage (callback)](#apidoc.element.s3.AWS.Request.prototype.eachPage)
- description and source-code
```javascript
function eachPage(callback) {
  // Make all callbacks async-ish
  callback = AWS.util.fn.makeAsync(callback, 3);

  function wrappedCallback(response) {
    callback.call(response, response.error, response.data, function (result) {
      if (result === false) return;

      if (response.hasNextPage()) {
        response.nextPage().on('complete', wrappedCallback).send();
      } else {
        callback.call(response, null, null, AWS.util.fn.noop);
      }
    });
  }

  this.on('complete', wrappedCallback).send();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Request.prototype.emit"></a>[function <span class="apidocSignatureSpan">s3.AWS.Request.prototype.</span>emit (eventName, eventArgs, doneCallback)](#apidoc.element.s3.AWS.Request.prototype.emit)
- description and source-code
```javascript
function emit(eventName, eventArgs, doneCallback) {
  if (!doneCallback) doneCallback = function() { };
  var listeners = this.listeners(eventName);
  var count = listeners.length;
  this.callListeners(listeners, eventArgs, doneCallback);
  return count > 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Request.prototype.emitEvent"></a>[function <span class="apidocSignatureSpan">s3.AWS.Request.prototype.</span>emitEvent (eventName, args, done)](#apidoc.element.s3.AWS.Request.prototype.emitEvent)
- description and source-code
```javascript
function emit(eventName, args, done) {
  if (typeof args === 'function') { done = args; args = null; }
  if (!done) done = function() { };
  if (!args) args = this.eventParameters(eventName, this.response);

  var origEmit = AWS.SequentialExecutor.prototype.emit;
  origEmit.call(this, eventName, args, function (err) {
    if (err) this.response.error = err;
    done.call(this, err);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Request.prototype.eventParameters"></a>[function <span class="apidocSignatureSpan">s3.AWS.Request.prototype.</span>eventParameters (eventName)](#apidoc.element.s3.AWS.Request.prototype.eventParameters)
- description and source-code
```javascript
function eventParameters(eventName) {
  switch (eventName) {
    case 'restart':
    case 'validate':
    case 'sign':
    case 'build':
    case 'afterValidate':
    case 'afterBuild':
      return [this];
    case 'error':
      return [this.response.error, this.response];
    default:
      return [this.response];
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Request.prototype.isPageable"></a>[function <span class="apidocSignatureSpan">s3.AWS.Request.prototype.</span>isPageable ()](#apidoc.element.s3.AWS.Request.prototype.isPageable)
- description and source-code
```javascript
function isPageable() {
  return this.service.paginationConfig(this.operation) ? true : false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Request.prototype.listeners"></a>[function <span class="apidocSignatureSpan">s3.AWS.Request.prototype.</span>listeners (eventName)](#apidoc.element.s3.AWS.Request.prototype.listeners)
- description and source-code
```javascript
function listeners(eventName) {
  return this._events[eventName] ? this._events[eventName].slice(0) : [];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Request.prototype.on"></a>[function <span class="apidocSignatureSpan">s3.AWS.Request.prototype.</span>on (eventName, listener)](#apidoc.element.s3.AWS.Request.prototype.on)
- description and source-code
```javascript
function on(eventName, listener) {
  if (this._events[eventName]) {
    this._events[eventName].push(listener);
  } else {
    this._events[eventName] = [listener];
  }
  return this;
}
```
- example usage
```shell
...
    Bucket: "s3 bucket name",
    Key: "some/remote/file",
    // other options supported by putObject, except Body and ContentLength.
    // See: http://docs.aws.amazon.com/AWSJavaScriptSDK/latest/AWS/S3.html#putObject-property
  },
};
var uploader = client.uploadFile(params);
uploader.on('error', function(err) {
  console.error("unable to upload:", err.stack);
});
uploader.on('progress', function() {
  console.log("progress", uploader.progressMd5Amount,
            uploader.progressAmount, uploader.progressTotal);
});
uploader.on('end', function() {
...
```

#### <a name="apidoc.element.s3.AWS.Request.prototype.onAsync"></a>[function <span class="apidocSignatureSpan">s3.AWS.Request.prototype.</span>onAsync (eventName, listener)](#apidoc.element.s3.AWS.Request.prototype.onAsync)
- description and source-code
```javascript
function onAsync(eventName, listener) {
  listener._isAsync = true;
  return this.on(eventName, listener);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Request.prototype.presign"></a>[function <span class="apidocSignatureSpan">s3.AWS.Request.prototype.</span>presign (expires, callback)](#apidoc.element.s3.AWS.Request.prototype.presign)
- description and source-code
```javascript
function presign(expires, callback) {
  if (!callback && typeof expires === 'function') {
    callback = expires;
    expires = null;
  }
  return new AWS.Signers.Presign().sign(this.toGet(), expires, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Request.prototype.removeAllListeners"></a>[function <span class="apidocSignatureSpan">s3.AWS.Request.prototype.</span>removeAllListeners (eventName)](#apidoc.element.s3.AWS.Request.prototype.removeAllListeners)
- description and source-code
```javascript
function removeAllListeners(eventName) {
  if (eventName) {
    delete this._events[eventName];
  } else {
    this._events = {};
  }
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Request.prototype.removeListener"></a>[function <span class="apidocSignatureSpan">s3.AWS.Request.prototype.</span>removeListener (eventName, listener)](#apidoc.element.s3.AWS.Request.prototype.removeListener)
- description and source-code
```javascript
function removeListener(eventName, listener) {
  var listeners = this._events[eventName];
  if (listeners) {
    var length = listeners.length;
    var position = -1;
    for (var i = 0; i < length; ++i) {
      if (listeners[i] === listener) {
        position = i;
      }
    }
    if (position > -1) {
      listeners.splice(position, 1);
    }
  }
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Request.prototype.runTo"></a>[function <span class="apidocSignatureSpan">s3.AWS.Request.prototype.</span>runTo (state, done)](#apidoc.element.s3.AWS.Request.prototype.runTo)
- description and source-code
```javascript
function runTo(state, done) {
  this._asm.runTo(state, done, this);
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Request.prototype.send"></a>[function <span class="apidocSignatureSpan">s3.AWS.Request.prototype.</span>send (callback)](#apidoc.element.s3.AWS.Request.prototype.send)
- description and source-code
```javascript
function send(callback) {
  if (callback) {
    this.on('complete', function (resp) {
      callback.call(resp, resp.error, resp.data);
    });
  }
  this.runTo();

  return this.response;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Request.prototype.toGet"></a>[function <span class="apidocSignatureSpan">s3.AWS.Request.prototype.</span>toGet ()](#apidoc.element.s3.AWS.Request.prototype.toGet)
- description and source-code
```javascript
function toGet() {
  if (this.service.api.protocol === 'query' ||
      this.service.api.protocol === 'ec2') {
    this.removeListener('build', this.buildAsGet);
    this.addListener('build', this.buildAsGet);
  }
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Request.prototype.toUnauthenticated"></a>[function <span class="apidocSignatureSpan">s3.AWS.Request.prototype.</span>toUnauthenticated ()](#apidoc.element.s3.AWS.Request.prototype.toUnauthenticated)
- description and source-code
```javascript
function toUnauthenticated() {
  this.removeListener('validate', AWS.EventListeners.Core.VALIDATE_CREDENTIALS);
  this.removeListener('sign', AWS.EventListeners.Core.SIGN);
  return this.toGet();
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.ResourceWaiter"></a>[module s3.AWS.ResourceWaiter](#apidoc.module.s3.AWS.ResourceWaiter)

#### <a name="apidoc.element.s3.AWS.ResourceWaiter.ResourceWaiter"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>ResourceWaiter (service, state)](#apidoc.element.s3.AWS.ResourceWaiter.ResourceWaiter)
- description and source-code
```javascript
function constructor(service, state) {
  this.service = service;
  this.state = state;

  if (typeof this.state === 'object') {
    AWS.util.each.call(this, this.state, function (key, value) {
      this.state = key;
      this.expectedValue = value;
    });
  }

  this.loadWaiterConfig(this.state);
  if (!this.expectedValue) {
    this.expectedValue = this.config.successValue;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.ResourceWaiter.__super__"></a>[function <span class="apidocSignatureSpan">s3.AWS.ResourceWaiter.</span>__super__ ()](#apidoc.element.s3.AWS.ResourceWaiter.__super__)
- description and source-code
```javascript
function Object() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.ResourceWaiter.prototype"></a>[module s3.AWS.ResourceWaiter.prototype](#apidoc.module.s3.AWS.ResourceWaiter.prototype)

#### <a name="apidoc.element.s3.AWS.ResourceWaiter.prototype.checkError"></a>[function <span class="apidocSignatureSpan">s3.AWS.ResourceWaiter.prototype.</span>checkError (resp)](#apidoc.element.s3.AWS.ResourceWaiter.prototype.checkError)
- description and source-code
```javascript
function checkError(resp) {
  var value = this.config.successValue;
  if (typeof value === 'number') {
    return resp.httpResponse.statusCode === value;
  } else {
    return resp.error && resp.error.code === value;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.ResourceWaiter.prototype.checkSuccess"></a>[function <span class="apidocSignatureSpan">s3.AWS.ResourceWaiter.prototype.</span>checkSuccess (resp)](#apidoc.element.s3.AWS.ResourceWaiter.prototype.checkSuccess)
- description and source-code
```javascript
function checkSuccess(resp) {
  if (!this.config.successPath) {
    return resp.httpResponse.statusCode < 300;
  }

  var r = AWS.util.jamespath.find(this.config.successPath, resp.data);

  if (this.config.failureValue &&
      this.config.failureValue.indexOf(r) >= 0) {
    return null; // fast fail
  }

  if (this.expectedValue) {
    return r === this.expectedValue;
  } else {
    return r ? true : false;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.ResourceWaiter.prototype.constructor"></a>[function <span class="apidocSignatureSpan">s3.AWS.ResourceWaiter.prototype.</span>constructor (service, state)](#apidoc.element.s3.AWS.ResourceWaiter.prototype.constructor)
- description and source-code
```javascript
function constructor(service, state) {
  this.service = service;
  this.state = state;

  if (typeof this.state === 'object') {
    AWS.util.each.call(this, this.state, function (key, value) {
      this.state = key;
      this.expectedValue = value;
    });
  }

  this.loadWaiterConfig(this.state);
  if (!this.expectedValue) {
    this.expectedValue = this.config.successValue;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.ResourceWaiter.prototype.loadWaiterConfig"></a>[function <span class="apidocSignatureSpan">s3.AWS.ResourceWaiter.prototype.</span>loadWaiterConfig (state, noException)](#apidoc.element.s3.AWS.ResourceWaiter.prototype.loadWaiterConfig)
- description and source-code
```javascript
function loadWaiterConfig(state, noException) {
  if (!this.service.api.waiters[state]) {
    if (noException) return;
    throw new AWS.util.error(new Error(), {
      code: 'StateNotFoundError',
      message: 'State ' + state + ' not found.'
    });
  }

  this.config = this.service.api.waiters[state];
  var config = this.config;

  // inherit acceptor data
  (function () { // anonymous function to avoid max complexity count
    config.successType = config.successType || config.acceptorType;
    config.successPath = config.successPath || config.acceptorPath;
    config.successValue = config.successValue || config.acceptorValue;
    config.failureType = config.failureType || config.acceptorType;
    config.failurePath = config.failurePath || config.acceptorPath;
    config.failureValue = config.failureValue || config.acceptorValue;
  })();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.ResourceWaiter.prototype.setError"></a>[function <span class="apidocSignatureSpan">s3.AWS.ResourceWaiter.prototype.</span>setError (resp, retryable)](#apidoc.element.s3.AWS.ResourceWaiter.prototype.setError)
- description and source-code
```javascript
function setError(resp, retryable) {
  resp.data = null;
  resp.error = AWS.util.error(resp.error || new Error(), {
    code: 'ResourceNotReady',
    message: 'Resource is not in the state ' + this.state,
    retryable: retryable
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.ResourceWaiter.prototype.wait"></a>[function <span class="apidocSignatureSpan">s3.AWS.ResourceWaiter.prototype.</span>wait (params, callback)](#apidoc.element.s3.AWS.ResourceWaiter.prototype.wait)
- description and source-code
```javascript
function wait(params, callback) {
  if (typeof params === 'function') {
    callback = params; params = undefined;
  }

  var request = this.service.makeRequest(this.config.operation, params);
  var listeners = this.Listeners[this.config.successType];
  request._waiter = this;
  request.response.maxRetries = this.config.maxAttempts;
  request.addListeners(this.Listeners.retry);
  if (listeners) request.addListeners(listeners);

  if (callback) request.send(callback);
  return request;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.Response"></a>[module s3.AWS.Response](#apidoc.module.s3.AWS.Response)

#### <a name="apidoc.element.s3.AWS.Response.Response"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>Response (request)](#apidoc.element.s3.AWS.Response.Response)
- description and source-code
```javascript
function Response(request) {
  this.request = request;
  this.data = null;
  this.error = null;
  this.retryCount = 0;
  this.redirectCount = 0;
  this.httpResponse = new AWS.HttpResponse();
  if (request) {
    this.maxRetries = request.service.numRetries();
    this.maxRedirects = request.service.config.maxRedirects;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Response.__super__"></a>[function <span class="apidocSignatureSpan">s3.AWS.Response.</span>__super__ ()](#apidoc.element.s3.AWS.Response.__super__)
- description and source-code
```javascript
function Object() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.Response.prototype"></a>[module s3.AWS.Response.prototype](#apidoc.module.s3.AWS.Response.prototype)

#### <a name="apidoc.element.s3.AWS.Response.prototype.cacheNextPageTokens"></a>[function <span class="apidocSignatureSpan">s3.AWS.Response.prototype.</span>cacheNextPageTokens ()](#apidoc.element.s3.AWS.Response.prototype.cacheNextPageTokens)
- description and source-code
```javascript
function cacheNextPageTokens() {
  if (this.hasOwnProperty('nextPageTokens')) return this.nextPageTokens;
  this.nextPageTokens = undefined;

  var config = this.request.service.paginationConfig(this.request.operation);
  if (!config) return this.nextPageTokens;

  this.nextPageTokens = null;
  if (config.moreResults) {
    if (!AWS.util.jamespath.find(config.moreResults, this.data)) {
      return this.nextPageTokens;
    }
  }

  var exprs = config.outputToken;
  if (typeof exprs === 'string') exprs = [exprs];
  AWS.util.arrayEach.call(this, exprs, function (expr) {
    var output = AWS.util.jamespath.find(expr, this.data);
    if (output) {
      this.nextPageTokens = this.nextPageTokens || [];
      this.nextPageTokens.push(output);
    }
  });

  return this.nextPageTokens;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Response.prototype.constructor"></a>[function <span class="apidocSignatureSpan">s3.AWS.Response.prototype.</span>constructor (request)](#apidoc.element.s3.AWS.Response.prototype.constructor)
- description and source-code
```javascript
function Response(request) {
  this.request = request;
  this.data = null;
  this.error = null;
  this.retryCount = 0;
  this.redirectCount = 0;
  this.httpResponse = new AWS.HttpResponse();
  if (request) {
    this.maxRetries = request.service.numRetries();
    this.maxRedirects = request.service.config.maxRedirects;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Response.prototype.hasNextPage"></a>[function <span class="apidocSignatureSpan">s3.AWS.Response.prototype.</span>hasNextPage ()](#apidoc.element.s3.AWS.Response.prototype.hasNextPage)
- description and source-code
```javascript
function hasNextPage() {
  this.cacheNextPageTokens();
  if (this.nextPageTokens) return true;
  if (this.nextPageTokens === undefined) return undefined;
  else return false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Response.prototype.nextPage"></a>[function <span class="apidocSignatureSpan">s3.AWS.Response.prototype.</span>nextPage (callback)](#apidoc.element.s3.AWS.Response.prototype.nextPage)
- description and source-code
```javascript
function nextPage(callback) {
  var config;
  var service = this.request.service;
  var operation = this.request.operation;
  try {
    config = service.paginationConfig(operation, true);
  } catch (e) { this.error = e; }

  if (!this.hasNextPage()) {
    if (callback) callback(this.error, null);
    else if (this.error) throw this.error;
    return null;
  }

  var params = AWS.util.copy(this.request.params);
  if (!this.nextPageTokens) {
    return callback ? callback(null, null) : null;
  } else {
    var inputTokens = config.inputToken;
    if (typeof inputTokens === 'string') inputTokens = [inputTokens];
    for (var i = 0; i < inputTokens.length; i++) {
      params[inputTokens[i]] = this.nextPageTokens[i];
    }
    return service.makeRequest(this.request.operation, params, callback);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.Route53"></a>[module s3.AWS.Route53](#apidoc.module.s3.AWS.Route53)

#### <a name="apidoc.element.s3.AWS.Route53.Route53"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>Route53 ()](#apidoc.element.s3.AWS.Route53.Route53)
- description and source-code
```javascript
Route53 = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Route53.__super__"></a>[function <span class="apidocSignatureSpan">s3.AWS.Route53.</span>__super__ (config)](#apidoc.element.s3.AWS.Route53.__super__)
- description and source-code
```javascript
function Service(config) {
  if (!this.loadServiceClass) {
    throw AWS.util.error(new Error(),
      'Service must be constructed with 'new\' operator');
  }
  var ServiceClass = this.loadServiceClass(config || {});
  if (ServiceClass) return new ServiceClass(config);
  this.initialize(config);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.Route53.prototype"></a>[module s3.AWS.Route53.prototype](#apidoc.module.s3.AWS.Route53.prototype)

#### <a name="apidoc.element.s3.AWS.Route53.prototype.constructor"></a>[function <span class="apidocSignatureSpan">s3.AWS.Route53.prototype.</span>constructor ()](#apidoc.element.s3.AWS.Route53.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Route53.prototype.sanitizeUrl"></a>[function <span class="apidocSignatureSpan">s3.AWS.Route53.prototype.</span>sanitizeUrl (request)](#apidoc.element.s3.AWS.Route53.prototype.sanitizeUrl)
- description and source-code
```javascript
function sanitizeUrl(request) {
  var path = request.httpRequest.path;
  request.httpRequest.path = path.replace(/\/%2F\w+%2F/, '/');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Route53.prototype.setupRequestListeners"></a>[function <span class="apidocSignatureSpan">s3.AWS.Route53.prototype.</span>setupRequestListeners (request)](#apidoc.element.s3.AWS.Route53.prototype.setupRequestListeners)
- description and source-code
```javascript
function setupRequestListeners(request) {
  request.on('build', this.sanitizeUrl);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.Route53Domains"></a>[module s3.AWS.Route53Domains](#apidoc.module.s3.AWS.Route53Domains)

#### <a name="apidoc.element.s3.AWS.Route53Domains.Route53Domains"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>Route53Domains ()](#apidoc.element.s3.AWS.Route53Domains.Route53Domains)
- description and source-code
```javascript
Route53Domains = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Route53Domains.__super__"></a>[function <span class="apidocSignatureSpan">s3.AWS.Route53Domains.</span>__super__ (config)](#apidoc.element.s3.AWS.Route53Domains.__super__)
- description and source-code
```javascript
function Service(config) {
  if (!this.loadServiceClass) {
    throw AWS.util.error(new Error(),
      'Service must be constructed with 'new\' operator');
  }
  var ServiceClass = this.loadServiceClass(config || {});
  if (ServiceClass) return new ServiceClass(config);
  this.initialize(config);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.Route53Domains.prototype"></a>[module s3.AWS.Route53Domains.prototype](#apidoc.module.s3.AWS.Route53Domains.prototype)

#### <a name="apidoc.element.s3.AWS.Route53Domains.prototype.constructor"></a>[function <span class="apidocSignatureSpan">s3.AWS.Route53Domains.prototype.</span>constructor ()](#apidoc.element.s3.AWS.Route53Domains.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.S3"></a>[module s3.AWS.S3](#apidoc.module.s3.AWS.S3)

#### <a name="apidoc.element.s3.AWS.S3.S3"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>S3 ()](#apidoc.element.s3.AWS.S3.S3)
- description and source-code
```javascript
S3 = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
...
  s3RetryCount: 3,    // this is the default
  s3RetryDelay: 1000, // this is the default
  multipartUploadThreshold: 20971520, // this is the default (20 MB)
  multipartUploadSize: 15728640, // this is the default (15 MB)
  s3Options: {
    accessKeyId: "your s3 key",
    secretAccessKey: "your s3 secret",
    // any other options are passed to new AWS.S3()
    // See: http://docs.aws.amazon.com/AWSJavaScriptSDK/latest/AWS/Config.html#constructor-property
  },
});
'''

### Create a client from existing AWS.S3 object
...
```

#### <a name="apidoc.element.s3.AWS.S3.__super__"></a>[function <span class="apidocSignatureSpan">s3.AWS.S3.</span>__super__ (config)](#apidoc.element.s3.AWS.S3.__super__)
- description and source-code
```javascript
function Service(config) {
  if (!this.loadServiceClass) {
    throw AWS.util.error(new Error(),
      'Service must be constructed with 'new\' operator');
  }
  var ServiceClass = this.loadServiceClass(config || {});
  if (ServiceClass) return new ServiceClass(config);
  this.initialize(config);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.S3.prototype"></a>[module s3.AWS.S3.prototype](#apidoc.module.s3.AWS.S3.prototype)

#### <a name="apidoc.element.s3.AWS.S3.prototype.addContentType"></a>[function <span class="apidocSignatureSpan">s3.AWS.S3.prototype.</span>addContentType (req)](#apidoc.element.s3.AWS.S3.prototype.addContentType)
- description and source-code
```javascript
function addContentType(req) {
  var httpRequest = req.httpRequest;
  if (httpRequest.method === 'GET' || httpRequest.method === 'HEAD') {
    // Content-Type is not set in GET/HEAD requests
    delete httpRequest.headers['Content-Type'];
    return;
  }

  if (!httpRequest.headers['Content-Type']) { // always have a Content-Type
    httpRequest.headers['Content-Type'] = 'application/octet-stream';
  }

  var contentType = httpRequest.headers['Content-Type'];
  if (AWS.util.isBrowser()) {
    if (typeof httpRequest.body === 'string' && !contentType.match(/;\s*charset=/)) {
      var charset = '; charset=UTF-8';
      httpRequest.headers['Content-Type'] += charset;
    } else {
      var replaceFn = function(_, prefix, charset) {
        return prefix + charset.toUpperCase();
      };

      httpRequest.headers['Content-Type'] =
        contentType.replace(/(;\s*charset=)(.+)$/, replaceFn);
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.S3.prototype.computeContentMd5"></a>[function <span class="apidocSignatureSpan">s3.AWS.S3.prototype.</span>computeContentMd5 (req)](#apidoc.element.s3.AWS.S3.prototype.computeContentMd5)
- description and source-code
```javascript
function computeContentMd5(req) {
  if (req.service.willComputeChecksums(req)) {
    var md5 = AWS.util.crypto.md5(req.httpRequest.body, 'base64');
    req.httpRequest.headers['Content-MD5'] = md5;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.S3.prototype.computeSha256"></a>[function <span class="apidocSignatureSpan">s3.AWS.S3.prototype.</span>computeSha256 (req, done)](#apidoc.element.s3.AWS.S3.prototype.computeSha256)
- description and source-code
```javascript
function computeSha256(req, done) {
  if (req.service.getSignerClass(req) === AWS.Signers.V4) {
    var body = req.httpRequest.body || '';

    if (AWS.util.isNode()) {
      var Stream = AWS.util.nodeRequire('stream').Stream;
      var fs = AWS.util.nodeRequire('fs');
      if (body instanceof Stream) {
        if (typeof body.path === 'string') { // assume file object
          body = fs.createReadStream(body.path);
        } else { // TODO support other stream types
          done(new Error('Non-file stream objects are ' +
                         'not supported with SigV4 in AWS.S3'));
          return;
        }
      }
    }

    AWS.util.crypto.sha256(body, 'hex', function(err, sha) {
      if (!err) {
        req.httpRequest.headers['X-Amz-Content-Sha256'] = sha;
      }
      done(err);
    });
  } else {
    done();
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.S3.prototype.computeSseCustomerKeyMd5"></a>[function <span class="apidocSignatureSpan">s3.AWS.S3.prototype.</span>computeSseCustomerKeyMd5 (req)](#apidoc.element.s3.AWS.S3.prototype.computeSseCustomerKeyMd5)
- description and source-code
```javascript
function computeSseCustomerKeyMd5(req) {
  var headers = [
    'x-amz-server-side-encryption-customer-key',
    'x-amz-copy-source-server-side-encryption-customer-key'
  ];
  AWS.util.arrayEach(headers, function(header) {
    if (req.httpRequest.headers[header]) {
      var key = req.httpRequest.headers[header];
      var md5header = header + '-MD5';

      req.httpRequest.headers[header] = AWS.util.base64.encode(key);
      if (!req.httpRequest.headers[md5header]) {
        var value = AWS.util.crypto.md5(key, 'base64');
        req.httpRequest.headers[md5header] = AWS.util.base64.encode(value);
      }

    }
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.S3.prototype.constructor"></a>[function <span class="apidocSignatureSpan">s3.AWS.S3.prototype.</span>constructor ()](#apidoc.element.s3.AWS.S3.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.S3.prototype.createBucket"></a>[function <span class="apidocSignatureSpan">s3.AWS.S3.prototype.</span>createBucket (params, callback)](#apidoc.element.s3.AWS.S3.prototype.createBucket)
- description and source-code
```javascript
function createBucket(params, callback) {
  // When creating a bucket *outside* the classic region, the location
  // constraint must be set for the bucket and it must match the endpoint.
  // This chunk of code will set the location constraint param based
  // on the region (when possible), but it will not override a passed-in
  // location constraint.
  if (!params) params = {};
  var hostname = this.endpoint.hostname;
  if (hostname !== this.api.globalEndpoint && !params.CreateBucketConfiguration) {
    params.CreateBucketConfiguration = { LocationConstraint: this.config.region };
  }
  return this.makeRequest('createBucket', params, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.S3.prototype.dnsCompatibleBucketName"></a>[function <span class="apidocSignatureSpan">s3.AWS.S3.prototype.</span>dnsCompatibleBucketName (bucketName)](#apidoc.element.s3.AWS.S3.prototype.dnsCompatibleBucketName)
- description and source-code
```javascript
function dnsCompatibleBucketName(bucketName) {
  var b = bucketName;
  var domain = new RegExp(/^[a-z0-9][a-z0-9\.\-]{1,61}[a-z0-9]$/);
  var ipAddress = new RegExp(/(\d+\.){3}\d+/);
  var dots = new RegExp(/\.\./);
  return (b.match(domain) && !b.match(ipAddress) && !b.match(dots)) ? true : false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.S3.prototype.extractData"></a>[function <span class="apidocSignatureSpan">s3.AWS.S3.prototype.</span>extractData (resp)](#apidoc.element.s3.AWS.S3.prototype.extractData)
- description and source-code
```javascript
function extractData(resp) {
  var req = resp.request;
  if (req.operation === 'getBucketLocation') {
    var match = resp.httpResponse.body.toString().match(/>(.+)<\/Location/);
    if (match) {
      delete resp.data['_'];
      resp.data.LocationConstraint = match[1];
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.S3.prototype.extractError"></a>[function <span class="apidocSignatureSpan">s3.AWS.S3.prototype.</span>extractError (resp)](#apidoc.element.s3.AWS.S3.prototype.extractError)
- description and source-code
```javascript
function extractError(resp) {
  var codes = {
    304: 'NotModified',
    403: 'Forbidden',
    400: 'BadRequest',
    404: 'NotFound'
  };

  var code = resp.httpResponse.statusCode;
  var body = resp.httpResponse.body || '';
  if (codes[code] && body.length === 0) {
    resp.error = AWS.util.error(new Error(), {
      code: codes[resp.httpResponse.statusCode],
      message: null
    });
  } else {
    var data = new AWS.XML.Parser().parse(body.toString());
    resp.error = AWS.util.error(new Error(), {
      code: data.Code || code,
      message: data.Message || null
    });
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.S3.prototype.getSignedUrl"></a>[function <span class="apidocSignatureSpan">s3.AWS.S3.prototype.</span>getSignedUrl (operation, params, callback)](#apidoc.element.s3.AWS.S3.prototype.getSignedUrl)
- description and source-code
```javascript
function getSignedUrl(operation, params, callback) {
  params = AWS.util.copy(params || {});
  var expires = params.Expires || 900;
  delete params.Expires; // we can't validate this
  var request = this.makeRequest(operation, params);
  return request.presign(expires, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.S3.prototype.pathStyleBucketName"></a>[function <span class="apidocSignatureSpan">s3.AWS.S3.prototype.</span>pathStyleBucketName (bucketName)](#apidoc.element.s3.AWS.S3.prototype.pathStyleBucketName)
- description and source-code
```javascript
function pathStyleBucketName(bucketName) {
  // user can force path style requests via the configuration
  if (this.config.s3ForcePathStyle) return true;
  if (this.config.s3BucketEndpoint) return false;

  if (this.dnsCompatibleBucketName(bucketName)) {
    return (this.config.sslEnabled && bucketName.match(/\./)) ? true : false;
  } else {
    return true; // not dns compatible names must always use path style
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.S3.prototype.populateURI"></a>[function <span class="apidocSignatureSpan">s3.AWS.S3.prototype.</span>populateURI (req)](#apidoc.element.s3.AWS.S3.prototype.populateURI)
- description and source-code
```javascript
function populateURI(req) {
  var httpRequest = req.httpRequest;
  var b = req.params.Bucket;

  if (b) {
    if (!req.service.pathStyleBucketName(b)) {
      if (!req.service.config.s3BucketEndpoint) {
        httpRequest.endpoint.hostname =
          b + '.' + httpRequest.endpoint.hostname;

        var port = httpRequest.endpoint.port;
        if (port !== 80 && port !== 443) {
          httpRequest.endpoint.host = httpRequest.endpoint.hostname + ':' +
            httpRequest.endpoint.port;
        } else {
          httpRequest.endpoint.host = httpRequest.endpoint.hostname;
        }
      }

      httpRequest.virtualHostedBucket = b; // needed for signing the request
      httpRequest.path = httpRequest.path.replace(new RegExp('/' + b), '');
      if (httpRequest.path[0] !== '/') {
        httpRequest.path = '/' + httpRequest.path;
      }
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.S3.prototype.prepareSignedUrl"></a>[function <span class="apidocSignatureSpan">s3.AWS.S3.prototype.</span>prepareSignedUrl (request)](#apidoc.element.s3.AWS.S3.prototype.prepareSignedUrl)
- description and source-code
```javascript
function prepareSignedUrl(request) {
  request.removeListener('build', request.service.addContentType);
  if (!request.params.Body) {
    // no Content-MD5/SHA-256 if body is not provided
    request.removeListener('build', request.service.computeContentMd5);
    request.removeListener('build', request.service.computeSha256);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.S3.prototype.retryableError"></a>[function <span class="apidocSignatureSpan">s3.AWS.S3.prototype.</span>retryableError (error, request)](#apidoc.element.s3.AWS.S3.prototype.retryableError)
- description and source-code
```javascript
function retryableError(error, request) {
  if (request.operation === 'completeMultipartUpload' &&
      error.statusCode === 200) {
    return true;
  } else if (error && error.code === 'RequestTimeout') {
    return true;
  } else {
    var _super = AWS.Service.prototype.retryableError;
    return _super.call(this, error, request);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.S3.prototype.setupRequestListeners"></a>[function <span class="apidocSignatureSpan">s3.AWS.S3.prototype.</span>setupRequestListeners (request)](#apidoc.element.s3.AWS.S3.prototype.setupRequestListeners)
- description and source-code
```javascript
function setupRequestListeners(request) {
  request.addListener('validate', this.validateScheme);
  request.addListener('validate', this.validateBucketEndpoint);
  request.addListener('build', this.addContentType);
  request.addListener('build', this.populateURI);
  request.addListener('build', this.computeContentMd5);
  request.onAsync('build', this.computeSha256);
  request.addListener('build', this.computeSseCustomerKeyMd5);
  request.removeListener('validate',
    AWS.EventListeners.Core.VALIDATE_REGION);
  request.addListener('extractError', this.extractError);
  request.addListener('extractData', this.extractData);
  request.addListener('beforePresign', this.prepareSignedUrl);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.S3.prototype.successfulResponse"></a>[function <span class="apidocSignatureSpan">s3.AWS.S3.prototype.</span>successfulResponse (resp)](#apidoc.element.s3.AWS.S3.prototype.successfulResponse)
- description and source-code
```javascript
function successfulResponse(resp) {
  var req = resp.request;
  var httpResponse = resp.httpResponse;
  if (req.operation === 'completeMultipartUpload' &&
      httpResponse.body.toString().match('<Error>'))
    return false;
  else
    return httpResponse.statusCode < 300;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.S3.prototype.validateBucketEndpoint"></a>[function <span class="apidocSignatureSpan">s3.AWS.S3.prototype.</span>validateBucketEndpoint (req)](#apidoc.element.s3.AWS.S3.prototype.validateBucketEndpoint)
- description and source-code
```javascript
validateBucketEndpoint = function (req) {
  if (!req.params.Bucket && req.service.config.s3BucketEndpoint) {
    var msg = 'Cannot send requests to root API with 's3BucketEndpoint' set.';
    throw AWS.util.error(new Error(),
      { code: 'ConfigError', message: msg });
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.S3.prototype.validateScheme"></a>[function <span class="apidocSignatureSpan">s3.AWS.S3.prototype.</span>validateScheme (req)](#apidoc.element.s3.AWS.S3.prototype.validateScheme)
- description and source-code
```javascript
validateScheme = function (req) {
  var params = req.params,
      scheme = req.httpRequest.endpoint.protocol,
      sensitive = params.SSECustomerKey || params.CopySourceSSECustomerKey;
  if (sensitive && scheme !== 'https:') {
    var msg = 'Cannot send SSE keys over HTTP. Set \'sslEnabled\'' +
      'to \'true\' in your configuration';
    throw AWS.util.error(new Error(),
      { code: 'ConfigError', message: msg });
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.S3.prototype.validateService"></a>[function <span class="apidocSignatureSpan">s3.AWS.S3.prototype.</span>validateService ()](#apidoc.element.s3.AWS.S3.prototype.validateService)
- description and source-code
```javascript
function validateService() {
  // default to us-east-1 when no region is provided
  if (!this.config.region) this.config.region = 'us-east-1';

  if (!this.config.endpoint && this.config.s3BucketEndpoint) {
    var msg = 'An endpoint must be provided when configuring ' +
              ''s3BucketEndpoint' to true.';
    throw AWS.util.error(new Error(),
      {name: 'InvalidEndpoint', message: msg});
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.S3.prototype.willComputeChecksums"></a>[function <span class="apidocSignatureSpan">s3.AWS.S3.prototype.</span>willComputeChecksums (req)](#apidoc.element.s3.AWS.S3.prototype.willComputeChecksums)
- description and source-code
```javascript
function willComputeChecksums(req) {
  if (this.computableChecksumOperations[req.operation]) return true;
  if (!this.config.computeChecksums) return false;

  // TODO: compute checksums for Stream objects
  if (!AWS.util.Buffer.isBuffer(req.httpRequest.body) &&
      typeof req.httpRequest.body !== 'string') {
    return false;
  }

  var rules = req.service.api.operations[req.operation].input.members;

  // V4 signer uses SHA256 signatures so only compute MD5 if it is required
  if (req.service.getSignerClass(req) === AWS.Signers.V4) {
    if (rules.ContentMD5 && !rules.ContentMD5.required) return false;
  }

  if (rules.ContentMD5 && !req.params.ContentMD5) return true;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.SAMLCredentials"></a>[module s3.AWS.SAMLCredentials](#apidoc.module.s3.AWS.SAMLCredentials)

#### <a name="apidoc.element.s3.AWS.SAMLCredentials.SAMLCredentials"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>SAMLCredentials (params)](#apidoc.element.s3.AWS.SAMLCredentials.SAMLCredentials)
- description and source-code
```javascript
function SAMLCredentials(params) {
  AWS.Credentials.call(this);
  this.expired = true;
  this.params = params;
  this.service = new AWS.STS({params: this.params});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.SAMLCredentials.__super__"></a>[function <span class="apidocSignatureSpan">s3.AWS.SAMLCredentials.</span>__super__ ()](#apidoc.element.s3.AWS.SAMLCredentials.__super__)
- description and source-code
```javascript
function Credentials() {
  // hide secretAccessKey from being displayed with util.inspect
  AWS.util.hideProperties(this, ['secretAccessKey']);

  this.expired = false;
  this.expireTime = null;
  if (arguments.length === 1 && typeof arguments[0] === 'object') {
    var creds = arguments[0].credentials || arguments[0];
    this.accessKeyId = creds.accessKeyId;
    this.secretAccessKey = creds.secretAccessKey;
    this.sessionToken = creds.sessionToken;
  } else {
    this.accessKeyId = arguments[0];
    this.secretAccessKey = arguments[1];
    this.sessionToken = arguments[2];
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.SAMLCredentials.prototype"></a>[module s3.AWS.SAMLCredentials.prototype](#apidoc.module.s3.AWS.SAMLCredentials.prototype)

#### <a name="apidoc.element.s3.AWS.SAMLCredentials.prototype.constructor"></a>[function <span class="apidocSignatureSpan">s3.AWS.SAMLCredentials.prototype.</span>constructor (params)](#apidoc.element.s3.AWS.SAMLCredentials.prototype.constructor)
- description and source-code
```javascript
function SAMLCredentials(params) {
  AWS.Credentials.call(this);
  this.expired = true;
  this.params = params;
  this.service = new AWS.STS({params: this.params});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.SAMLCredentials.prototype.refresh"></a>[function <span class="apidocSignatureSpan">s3.AWS.SAMLCredentials.prototype.</span>refresh (callback)](#apidoc.element.s3.AWS.SAMLCredentials.prototype.refresh)
- description and source-code
```javascript
function refresh(callback) {
  var self = this;
  if (!callback) callback = function(err) { if (err) throw err; };

  self.service.assumeRoleWithSAML(function (err, data) {
    if (!err) {
      self.service.credentialsFrom(data, self);
    }
    callback(err);
  });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.SES"></a>[module s3.AWS.SES](#apidoc.module.s3.AWS.SES)

#### <a name="apidoc.element.s3.AWS.SES.SES"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>SES ()](#apidoc.element.s3.AWS.SES.SES)
- description and source-code
```javascript
SES = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.SES.__super__"></a>[function <span class="apidocSignatureSpan">s3.AWS.SES.</span>__super__ (config)](#apidoc.element.s3.AWS.SES.__super__)
- description and source-code
```javascript
function Service(config) {
  if (!this.loadServiceClass) {
    throw AWS.util.error(new Error(),
      'Service must be constructed with 'new\' operator');
  }
  var ServiceClass = this.loadServiceClass(config || {});
  if (ServiceClass) return new ServiceClass(config);
  this.initialize(config);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.SES.prototype"></a>[module s3.AWS.SES.prototype](#apidoc.module.s3.AWS.SES.prototype)

#### <a name="apidoc.element.s3.AWS.SES.prototype.constructor"></a>[function <span class="apidocSignatureSpan">s3.AWS.SES.prototype.</span>constructor ()](#apidoc.element.s3.AWS.SES.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.SNS"></a>[module s3.AWS.SNS](#apidoc.module.s3.AWS.SNS)

#### <a name="apidoc.element.s3.AWS.SNS.SNS"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>SNS ()](#apidoc.element.s3.AWS.SNS.SNS)
- description and source-code
```javascript
SNS = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.SNS.__super__"></a>[function <span class="apidocSignatureSpan">s3.AWS.SNS.</span>__super__ (config)](#apidoc.element.s3.AWS.SNS.__super__)
- description and source-code
```javascript
function Service(config) {
  if (!this.loadServiceClass) {
    throw AWS.util.error(new Error(),
      'Service must be constructed with 'new\' operator');
  }
  var ServiceClass = this.loadServiceClass(config || {});
  if (ServiceClass) return new ServiceClass(config);
  this.initialize(config);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.SNS.prototype"></a>[module s3.AWS.SNS.prototype](#apidoc.module.s3.AWS.SNS.prototype)

#### <a name="apidoc.element.s3.AWS.SNS.prototype.constructor"></a>[function <span class="apidocSignatureSpan">s3.AWS.SNS.prototype.</span>constructor ()](#apidoc.element.s3.AWS.SNS.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.SQS"></a>[module s3.AWS.SQS](#apidoc.module.s3.AWS.SQS)

#### <a name="apidoc.element.s3.AWS.SQS.SQS"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>SQS ()](#apidoc.element.s3.AWS.SQS.SQS)
- description and source-code
```javascript
SQS = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.SQS.__super__"></a>[function <span class="apidocSignatureSpan">s3.AWS.SQS.</span>__super__ (config)](#apidoc.element.s3.AWS.SQS.__super__)
- description and source-code
```javascript
function Service(config) {
  if (!this.loadServiceClass) {
    throw AWS.util.error(new Error(),
      'Service must be constructed with 'new\' operator');
  }
  var ServiceClass = this.loadServiceClass(config || {});
  if (ServiceClass) return new ServiceClass(config);
  this.initialize(config);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.SQS.prototype"></a>[module s3.AWS.SQS.prototype](#apidoc.module.s3.AWS.SQS.prototype)

#### <a name="apidoc.element.s3.AWS.SQS.prototype.buildEndpoint"></a>[function <span class="apidocSignatureSpan">s3.AWS.SQS.prototype.</span>buildEndpoint (request)](#apidoc.element.s3.AWS.SQS.prototype.buildEndpoint)
- description and source-code
```javascript
function buildEndpoint(request) {
  var url = request.httpRequest.params.QueueUrl;
  if (url) {
    request.httpRequest.endpoint = new AWS.Endpoint(url);

    // signature version 4 requires the region name to be set,
    // sqs queue urls contain the region name
    var matches = request.httpRequest.endpoint.host.match(/^sqs\.(.+?)\./);
    if (matches) request.httpRequest.region = matches[1];
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.SQS.prototype.calculateChecksum"></a>[function <span class="apidocSignatureSpan">s3.AWS.SQS.prototype.</span>calculateChecksum (data)](#apidoc.element.s3.AWS.SQS.prototype.calculateChecksum)
- description and source-code
```javascript
function calculateChecksum(data) {
  return AWS.util.crypto.md5(data, 'hex');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.SQS.prototype.constructor"></a>[function <span class="apidocSignatureSpan">s3.AWS.SQS.prototype.</span>constructor ()](#apidoc.element.s3.AWS.SQS.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.SQS.prototype.isChecksumValid"></a>[function <span class="apidocSignatureSpan">s3.AWS.SQS.prototype.</span>isChecksumValid (checksum, data)](#apidoc.element.s3.AWS.SQS.prototype.isChecksumValid)
- description and source-code
```javascript
function isChecksumValid(checksum, data) {
  return this.calculateChecksum(data) === checksum;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.SQS.prototype.setupRequestListeners"></a>[function <span class="apidocSignatureSpan">s3.AWS.SQS.prototype.</span>setupRequestListeners (request)](#apidoc.element.s3.AWS.SQS.prototype.setupRequestListeners)
- description and source-code
```javascript
function setupRequestListeners(request) {
  request.addListener('build', this.buildEndpoint);

  if (request.service.config.computeChecksums) {
    if (request.operation === 'sendMessage') {
      request.addListener('extractData', this.verifySendMessageChecksum);
    } else if (request.operation === 'sendMessageBatch') {
      request.addListener('extractData', this.verifySendMessageBatchChecksum);
    } else if (request.operation === 'receiveMessage') {
      request.addListener('extractData', this.verifyReceiveMessageChecksum);
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.SQS.prototype.throwInvalidChecksumError"></a>[function <span class="apidocSignatureSpan">s3.AWS.SQS.prototype.</span>throwInvalidChecksumError (response, ids, message)](#apidoc.element.s3.AWS.SQS.prototype.throwInvalidChecksumError)
- description and source-code
```javascript
function throwInvalidChecksumError(response, ids, message) {
  response.error = AWS.util.error(new Error(), {
    retryable: true,
    code: 'InvalidChecksum',
    messageIds: ids,
    message: response.request.operation +
             ' returned an invalid MD5 response. ' + message
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.SQS.prototype.verifyReceiveMessageChecksum"></a>[function <span class="apidocSignatureSpan">s3.AWS.SQS.prototype.</span>verifyReceiveMessageChecksum (response)](#apidoc.element.s3.AWS.SQS.prototype.verifyReceiveMessageChecksum)
- description and source-code
```javascript
function verifyReceiveMessageChecksum(response) {
  if (!response.data) return;

  var service = this.service;
  var messageIds = [];
  AWS.util.arrayEach(response.data.Messages, function(message) {
    var md5 = message.MD5OfBody;
    var body = message.Body;
    if (!service.isChecksumValid(md5, body)) {
      messageIds.push(message.MessageId);
    }
  });

  if (messageIds.length > 0) {
    service.throwInvalidChecksumError(response, messageIds,
      'Invalid messages: ' + messageIds.join(', '));
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.SQS.prototype.verifySendMessageBatchChecksum"></a>[function <span class="apidocSignatureSpan">s3.AWS.SQS.prototype.</span>verifySendMessageBatchChecksum (response)](#apidoc.element.s3.AWS.SQS.prototype.verifySendMessageBatchChecksum)
- description and source-code
```javascript
function verifySendMessageBatchChecksum(response) {
  if (!response.data) return;

  var service = this.service;
  var entries = {};
  var errors = [];
  var messageIds = [];
  AWS.util.arrayEach(response.data.Successful, function (entry) {
    entries[entry.Id] = entry;
  });
  AWS.util.arrayEach(this.params.Entries, function (entry) {
    if (entries[entry.Id]) {
      var md5 = entries[entry.Id].MD5OfMessageBody;
      var body = entry.MessageBody;
      if (!service.isChecksumValid(md5, body)) {
        errors.push(entry.Id);
        messageIds.push(entries[entry.Id].MessageId);
      }
    }
  });

  if (errors.length > 0) {
    service.throwInvalidChecksumError(response, messageIds,
      'Invalid messages: ' + errors.join(', '));
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.SQS.prototype.verifySendMessageChecksum"></a>[function <span class="apidocSignatureSpan">s3.AWS.SQS.prototype.</span>verifySendMessageChecksum (response)](#apidoc.element.s3.AWS.SQS.prototype.verifySendMessageChecksum)
- description and source-code
```javascript
function verifySendMessageChecksum(response) {
  if (!response.data) return;

  var md5 = response.data.MD5OfMessageBody;
  var body = this.params.MessageBody;
  var calculatedMd5 = this.service.calculateChecksum(body);
  if (calculatedMd5 !== md5) {
    var msg = 'Got "' + response.data.MD5OfMessageBody +
      '", expecting "' + calculatedMd5 + '".';
    this.service.throwInvalidChecksumError(response,
      [response.data.MessageId], msg);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.STS"></a>[module s3.AWS.STS](#apidoc.module.s3.AWS.STS)

#### <a name="apidoc.element.s3.AWS.STS.STS"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>STS ()](#apidoc.element.s3.AWS.STS.STS)
- description and source-code
```javascript
STS = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.STS.__super__"></a>[function <span class="apidocSignatureSpan">s3.AWS.STS.</span>__super__ (config)](#apidoc.element.s3.AWS.STS.__super__)
- description and source-code
```javascript
function Service(config) {
  if (!this.loadServiceClass) {
    throw AWS.util.error(new Error(),
      'Service must be constructed with 'new\' operator');
  }
  var ServiceClass = this.loadServiceClass(config || {});
  if (ServiceClass) return new ServiceClass(config);
  this.initialize(config);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.STS.prototype"></a>[module s3.AWS.STS.prototype](#apidoc.module.s3.AWS.STS.prototype)

#### <a name="apidoc.element.s3.AWS.STS.prototype.assumeRoleWithSAML"></a>[function <span class="apidocSignatureSpan">s3.AWS.STS.prototype.</span>assumeRoleWithSAML (params, callback)](#apidoc.element.s3.AWS.STS.prototype.assumeRoleWithSAML)
- description and source-code
```javascript
function assumeRoleWithSAML(params, callback) {
  return this.makeUnauthenticatedRequest('assumeRoleWithSAML', params, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.STS.prototype.assumeRoleWithWebIdentity"></a>[function <span class="apidocSignatureSpan">s3.AWS.STS.prototype.</span>assumeRoleWithWebIdentity (params, callback)](#apidoc.element.s3.AWS.STS.prototype.assumeRoleWithWebIdentity)
- description and source-code
```javascript
function assumeRoleWithWebIdentity(params, callback) {
  return this.makeUnauthenticatedRequest('assumeRoleWithWebIdentity', params, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.STS.prototype.constructor"></a>[function <span class="apidocSignatureSpan">s3.AWS.STS.prototype.</span>constructor ()](#apidoc.element.s3.AWS.STS.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.STS.prototype.credentialsFrom"></a>[function <span class="apidocSignatureSpan">s3.AWS.STS.prototype.</span>credentialsFrom (data, credentials)](#apidoc.element.s3.AWS.STS.prototype.credentialsFrom)
- description and source-code
```javascript
function credentialsFrom(data, credentials) {
  if (!data) return null;
  if (!credentials) credentials = new AWS.TemporaryCredentials();
  credentials.expired = false;
  credentials.accessKeyId = data.Credentials.AccessKeyId;
  credentials.secretAccessKey = data.Credentials.SecretAccessKey;
  credentials.sessionToken = data.Credentials.SessionToken;
  credentials.expireTime = data.Credentials.Expiration;
  return credentials;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.SWF"></a>[module s3.AWS.SWF](#apidoc.module.s3.AWS.SWF)

#### <a name="apidoc.element.s3.AWS.SWF.SWF"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>SWF ()](#apidoc.element.s3.AWS.SWF.SWF)
- description and source-code
```javascript
SWF = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.SWF.__super__"></a>[function <span class="apidocSignatureSpan">s3.AWS.SWF.</span>__super__ (config)](#apidoc.element.s3.AWS.SWF.__super__)
- description and source-code
```javascript
function Service(config) {
  if (!this.loadServiceClass) {
    throw AWS.util.error(new Error(),
      'Service must be constructed with 'new\' operator');
  }
  var ServiceClass = this.loadServiceClass(config || {});
  if (ServiceClass) return new ServiceClass(config);
  this.initialize(config);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.SWF.prototype"></a>[module s3.AWS.SWF.prototype](#apidoc.module.s3.AWS.SWF.prototype)

#### <a name="apidoc.element.s3.AWS.SWF.prototype.constructor"></a>[function <span class="apidocSignatureSpan">s3.AWS.SWF.prototype.</span>constructor ()](#apidoc.element.s3.AWS.SWF.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.SequentialExecutor"></a>[module s3.AWS.SequentialExecutor](#apidoc.module.s3.AWS.SequentialExecutor)

#### <a name="apidoc.element.s3.AWS.SequentialExecutor.SequentialExecutor"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>SequentialExecutor ()](#apidoc.element.s3.AWS.SequentialExecutor.SequentialExecutor)
- description and source-code
```javascript
function SequentialExecutor() {
  this._events = {};
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.SequentialExecutor.__super__"></a>[function <span class="apidocSignatureSpan">s3.AWS.SequentialExecutor.</span>__super__ ()](#apidoc.element.s3.AWS.SequentialExecutor.__super__)
- description and source-code
```javascript
function Object() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.SequentialExecutor.prototype"></a>[module s3.AWS.SequentialExecutor.prototype](#apidoc.module.s3.AWS.SequentialExecutor.prototype)

#### <a name="apidoc.element.s3.AWS.SequentialExecutor.prototype.addListener"></a>[function <span class="apidocSignatureSpan">s3.AWS.SequentialExecutor.prototype.</span>addListener (eventName, listener)](#apidoc.element.s3.AWS.SequentialExecutor.prototype.addListener)
- description and source-code
```javascript
function on(eventName, listener) {
  if (this._events[eventName]) {
    this._events[eventName].push(listener);
  } else {
    this._events[eventName] = [listener];
  }
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.SequentialExecutor.prototype.addListeners"></a>[function <span class="apidocSignatureSpan">s3.AWS.SequentialExecutor.prototype.</span>addListeners (listeners)](#apidoc.element.s3.AWS.SequentialExecutor.prototype.addListeners)
- description and source-code
```javascript
function addListeners(listeners) {
  var self = this;

  // extract listeners if parameter is an SequentialExecutor object
  if (listeners._events) listeners = listeners._events;

  AWS.util.each(listeners, function(event, callbacks) {
    if (typeof callbacks === 'function') callbacks = [callbacks];
    AWS.util.arrayEach(callbacks, function(callback) {
      self.on(event, callback);
    });
  });

  return self;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.SequentialExecutor.prototype.addNamedAsyncListener"></a>[function <span class="apidocSignatureSpan">s3.AWS.SequentialExecutor.prototype.</span>addNamedAsyncListener (name, eventName, callback)](#apidoc.element.s3.AWS.SequentialExecutor.prototype.addNamedAsyncListener)
- description and source-code
```javascript
function addNamedAsyncListener(name, eventName, callback) {
  callback._isAsync = true;
  return this.addNamedListener(name, eventName, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.SequentialExecutor.prototype.addNamedListener"></a>[function <span class="apidocSignatureSpan">s3.AWS.SequentialExecutor.prototype.</span>addNamedListener (name, eventName, callback)](#apidoc.element.s3.AWS.SequentialExecutor.prototype.addNamedListener)
- description and source-code
```javascript
function addNamedListener(name, eventName, callback) {
  this[name] = callback;
  this.addListener(eventName, callback);
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.SequentialExecutor.prototype.addNamedListeners"></a>[function <span class="apidocSignatureSpan">s3.AWS.SequentialExecutor.prototype.</span>addNamedListeners (callback)](#apidoc.element.s3.AWS.SequentialExecutor.prototype.addNamedListeners)
- description and source-code
```javascript
function addNamedListeners(callback) {
  var self = this;
  callback(
    function() {
      self.addNamedListener.apply(self, arguments);
    },
    function() {
      self.addNamedAsyncListener.apply(self, arguments);
    }
  );
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.SequentialExecutor.prototype.callListeners"></a>[function <span class="apidocSignatureSpan">s3.AWS.SequentialExecutor.prototype.</span>callListeners (listeners, args, doneCallback)](#apidoc.element.s3.AWS.SequentialExecutor.prototype.callListeners)
- description and source-code
```javascript
function callListeners(listeners, args, doneCallback) {
  var self = this;
  function callNextListener(err) {
    if (err) {
      doneCallback.call(self, err);
    } else {
      self.callListeners(listeners, args, doneCallback);
    }
  }

  while (listeners.length > 0) {
    var listener = listeners.shift();
    if (listener._isAsync) { // asynchronous listener
      listener.apply(self, args.concat([callNextListener]));
      return; // stop here, callNextListener will continue
    } else { // synchronous listener
      listener.apply(self, args);
    }
  }

  doneCallback.call(self);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.SequentialExecutor.prototype.constructor"></a>[function <span class="apidocSignatureSpan">s3.AWS.SequentialExecutor.prototype.</span>constructor ()](#apidoc.element.s3.AWS.SequentialExecutor.prototype.constructor)
- description and source-code
```javascript
function SequentialExecutor() {
  this._events = {};
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.SequentialExecutor.prototype.emit"></a>[function <span class="apidocSignatureSpan">s3.AWS.SequentialExecutor.prototype.</span>emit (eventName, eventArgs, doneCallback)](#apidoc.element.s3.AWS.SequentialExecutor.prototype.emit)
- description and source-code
```javascript
function emit(eventName, eventArgs, doneCallback) {
  if (!doneCallback) doneCallback = function() { };
  var listeners = this.listeners(eventName);
  var count = listeners.length;
  this.callListeners(listeners, eventArgs, doneCallback);
  return count > 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.SequentialExecutor.prototype.listeners"></a>[function <span class="apidocSignatureSpan">s3.AWS.SequentialExecutor.prototype.</span>listeners (eventName)](#apidoc.element.s3.AWS.SequentialExecutor.prototype.listeners)
- description and source-code
```javascript
function listeners(eventName) {
  return this._events[eventName] ? this._events[eventName].slice(0) : [];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.SequentialExecutor.prototype.on"></a>[function <span class="apidocSignatureSpan">s3.AWS.SequentialExecutor.prototype.</span>on (eventName, listener)](#apidoc.element.s3.AWS.SequentialExecutor.prototype.on)
- description and source-code
```javascript
function on(eventName, listener) {
  if (this._events[eventName]) {
    this._events[eventName].push(listener);
  } else {
    this._events[eventName] = [listener];
  }
  return this;
}
```
- example usage
```shell
...
    Bucket: "s3 bucket name",
    Key: "some/remote/file",
    // other options supported by putObject, except Body and ContentLength.
    // See: http://docs.aws.amazon.com/AWSJavaScriptSDK/latest/AWS/S3.html#putObject-property
  },
};
var uploader = client.uploadFile(params);
uploader.on('error', function(err) {
  console.error("unable to upload:", err.stack);
});
uploader.on('progress', function() {
  console.log("progress", uploader.progressMd5Amount,
            uploader.progressAmount, uploader.progressTotal);
});
uploader.on('end', function() {
...
```

#### <a name="apidoc.element.s3.AWS.SequentialExecutor.prototype.onAsync"></a>[function <span class="apidocSignatureSpan">s3.AWS.SequentialExecutor.prototype.</span>onAsync (eventName, listener)](#apidoc.element.s3.AWS.SequentialExecutor.prototype.onAsync)
- description and source-code
```javascript
function onAsync(eventName, listener) {
  listener._isAsync = true;
  return this.on(eventName, listener);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.SequentialExecutor.prototype.removeAllListeners"></a>[function <span class="apidocSignatureSpan">s3.AWS.SequentialExecutor.prototype.</span>removeAllListeners (eventName)](#apidoc.element.s3.AWS.SequentialExecutor.prototype.removeAllListeners)
- description and source-code
```javascript
function removeAllListeners(eventName) {
  if (eventName) {
    delete this._events[eventName];
  } else {
    this._events = {};
  }
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.SequentialExecutor.prototype.removeListener"></a>[function <span class="apidocSignatureSpan">s3.AWS.SequentialExecutor.prototype.</span>removeListener (eventName, listener)](#apidoc.element.s3.AWS.SequentialExecutor.prototype.removeListener)
- description and source-code
```javascript
function removeListener(eventName, listener) {
  var listeners = this._events[eventName];
  if (listeners) {
    var length = listeners.length;
    var position = -1;
    for (var i = 0; i < length; ++i) {
      if (listeners[i] === listener) {
        position = i;
      }
    }
    if (position > -1) {
      listeners.splice(position, 1);
    }
  }
  return this;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.Service"></a>[module s3.AWS.Service](#apidoc.module.s3.AWS.Service)

#### <a name="apidoc.element.s3.AWS.Service.Service"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>Service (config)](#apidoc.element.s3.AWS.Service.Service)
- description and source-code
```javascript
function Service(config) {
  if (!this.loadServiceClass) {
    throw AWS.util.error(new Error(),
      'Service must be constructed with 'new\' operator');
  }
  var ServiceClass = this.loadServiceClass(config || {});
  if (ServiceClass) return new ServiceClass(config);
  this.initialize(config);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Service.__super__"></a>[function <span class="apidocSignatureSpan">s3.AWS.Service.</span>__super__ ()](#apidoc.element.s3.AWS.Service.__super__)
- description and source-code
```javascript
function Object() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Service.addVersions"></a>[function <span class="apidocSignatureSpan">s3.AWS.Service.</span>addVersions (svc, versions)](#apidoc.element.s3.AWS.Service.addVersions)
- description and source-code
```javascript
function addVersions(svc, versions) {
  if (!Array.isArray(versions)) versions = [versions];

  svc.services = svc.services || {};
  for (var i = 0; i < versions.length; i++) {
    if (svc.services[versions[i]] === undefined) {
      svc.services[versions[i]] = null;
    }
  }

  svc.apiVersions = Object.keys(svc.services).sort();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Service.defineMethods"></a>[function <span class="apidocSignatureSpan">s3.AWS.Service.</span>defineMethods (svc)](#apidoc.element.s3.AWS.Service.defineMethods)
- description and source-code
```javascript
function defineMethods(svc) {
  AWS.util.each(svc.prototype.api.operations, function iterator(method) {
    if (svc.prototype[method]) return;
    svc.prototype[method] = function (params, callback) {
      return this.makeRequest(method, params, callback);
    };
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Service.defineService"></a>[function <span class="apidocSignatureSpan">s3.AWS.Service.</span>defineService (serviceIdentifier, versions, features)](#apidoc.element.s3.AWS.Service.defineService)
- description and source-code
```javascript
function defineService(serviceIdentifier, versions, features) {
  AWS.Service._serviceMap[serviceIdentifier] = true;
  if (!Array.isArray(versions)) {
    features = versions;
    versions = [];
  }

  var svc = inherit(AWS.Service, features || {});

  if (typeof serviceIdentifier === 'string') {
    AWS.Service.addVersions(svc, versions);

    var identifier = svc.serviceIdentifier || serviceIdentifier;
    svc.serviceIdentifier = identifier;
  } else { // defineService called with an API
    svc.prototype.api = serviceIdentifier;
    AWS.Service.defineMethods(svc);
  }

  return svc;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Service.defineServiceApi"></a>[function <span class="apidocSignatureSpan">s3.AWS.Service.</span>defineServiceApi (superclass, version, apiConfig)](#apidoc.element.s3.AWS.Service.defineServiceApi)
- description and source-code
```javascript
function defineServiceApi(superclass, version, apiConfig) {
  var svc = inherit(superclass, {
    serviceIdentifier: superclass.serviceIdentifier
  });

  function setApi(api) {
    if (api.isApi) {
      svc.prototype.api = api;
    } else {
      svc.prototype.api = new Api(api);
    }
  }

  if (typeof version === 'string') {
    if (apiConfig) {
      setApi(apiConfig);
    } else {
      try {
        setApi(AWS.apiLoader(superclass.serviceIdentifier, version));
      } catch (err) {
        throw AWS.util.error(err, {
          message: 'Could not find API configuration ' +
            superclass.serviceIdentifier + '-' + version
        });
      }
    }
    if (!superclass.services.hasOwnProperty(version)) {
      superclass.apiVersions = superclass.apiVersions.concat(version).sort();
    }
    superclass.services[version] = svc;
  } else {
    setApi(version);
  }

  AWS.Service.defineMethods(svc);
  return svc;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Service.hasService"></a>[function <span class="apidocSignatureSpan">s3.AWS.Service.</span>hasService (identifier)](#apidoc.element.s3.AWS.Service.hasService)
- description and source-code
```javascript
hasService = function (identifier) {
  return AWS.Service._serviceMap.hasOwnProperty(identifier);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.Service.prototype"></a>[module s3.AWS.Service.prototype](#apidoc.module.s3.AWS.Service.prototype)

#### <a name="apidoc.element.s3.AWS.Service.prototype.addAllRequestListeners"></a>[function <span class="apidocSignatureSpan">s3.AWS.Service.prototype.</span>addAllRequestListeners (request)](#apidoc.element.s3.AWS.Service.prototype.addAllRequestListeners)
- description and source-code
```javascript
function addAllRequestListeners(request) {
  var list = [AWS.events, AWS.EventListeners.Core, this.serviceInterface(),
              AWS.EventListeners.CorePost];
  for (var i = 0; i < list.length; i++) {
    if (list[i]) request.addListeners(list[i]);
  }

  // disable parameter validation
  if (!this.config.paramValidation) {
    request.removeListener('validate',
      AWS.EventListeners.Core.VALIDATE_PARAMETERS);
  }

  if (this.config.logger) { // add logging events
    request.addListeners(AWS.EventListeners.Logger);
  }

  this.setupRequestListeners(request);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Service.prototype.constructor"></a>[function <span class="apidocSignatureSpan">s3.AWS.Service.prototype.</span>constructor (config)](#apidoc.element.s3.AWS.Service.prototype.constructor)
- description and source-code
```javascript
function Service(config) {
  if (!this.loadServiceClass) {
    throw AWS.util.error(new Error(),
      'Service must be constructed with 'new\' operator');
  }
  var ServiceClass = this.loadServiceClass(config || {});
  if (ServiceClass) return new ServiceClass(config);
  this.initialize(config);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Service.prototype.endpointFromTemplate"></a>[function <span class="apidocSignatureSpan">s3.AWS.Service.prototype.</span>endpointFromTemplate (endpoint)](#apidoc.element.s3.AWS.Service.prototype.endpointFromTemplate)
- description and source-code
```javascript
function endpointFromTemplate(endpoint) {
  if (typeof endpoint !== 'string') return endpoint;

  var e = endpoint;
  e = e.replace(/\{service\}/g, this.api.endpointPrefix);
  e = e.replace(/\{region\}/g, this.config.region);
  e = e.replace(/\{scheme\}/g, this.config.sslEnabled ? 'https' : 'http');
  return e;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Service.prototype.expiredCredentialsError"></a>[function <span class="apidocSignatureSpan">s3.AWS.Service.prototype.</span>expiredCredentialsError (error)](#apidoc.element.s3.AWS.Service.prototype.expiredCredentialsError)
- description and source-code
```javascript
function expiredCredentialsError(error) {
  // TODO : this only handles *one* of the expired credential codes
  return (error.code === 'ExpiredTokenException');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Service.prototype.getLatestServiceClass"></a>[function <span class="apidocSignatureSpan">s3.AWS.Service.prototype.</span>getLatestServiceClass (version)](#apidoc.element.s3.AWS.Service.prototype.getLatestServiceClass)
- description and source-code
```javascript
function getLatestServiceClass(version) {
  version = this.getLatestServiceVersion(version);
  if (this.constructor.services[version] === null) {
    AWS.Service.defineServiceApi(this.constructor, version);
  }

  return this.constructor.services[version];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Service.prototype.getLatestServiceVersion"></a>[function <span class="apidocSignatureSpan">s3.AWS.Service.prototype.</span>getLatestServiceVersion (version)](#apidoc.element.s3.AWS.Service.prototype.getLatestServiceVersion)
- description and source-code
```javascript
function getLatestServiceVersion(version) {
  if (!this.constructor.services || this.constructor.services.length === 0) {
    throw new Error('No services defined on ' +
                    this.constructor.serviceIdentifier);
  }

  if (!version) {
    version = 'latest';
  } else if (AWS.util.isType(version, Date)) {
    version = AWS.util.date.iso8601(version).split('T')[0];
  }

  if (Object.hasOwnProperty(this.constructor.services, version)) {
    return version;
  }

  var keys = Object.keys(this.constructor.services).sort();
  var selectedVersion = null;
  for (var i = keys.length - 1; i >= 0; i--) {
    // versions that end in "*" are not available on disk and can be
    // skipped, so do not choose these as selectedVersions
    if (keys[i][keys[i].length - 1] !== '*') {
      selectedVersion = keys[i];
    }
    if (keys[i].substr(0, 10) <= version) {
      return selectedVersion;
    }
  }

  throw new Error('Could not find ' + this.constructor.serviceIdentifier +
                  ' API to satisfy version constraint '' + version + '\'');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Service.prototype.getSignerClass"></a>[function <span class="apidocSignatureSpan">s3.AWS.Service.prototype.</span>getSignerClass ()](#apidoc.element.s3.AWS.Service.prototype.getSignerClass)
- description and source-code
```javascript
function getSignerClass() {
  var version;
  if (this.config.signatureVersion) {
    version = this.config.signatureVersion;
  } else {
    version = this.api.signatureVersion;
  }
  return AWS.Signers.RequestSigner.getVersion(version);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Service.prototype.initialize"></a>[function <span class="apidocSignatureSpan">s3.AWS.Service.prototype.</span>initialize (config)](#apidoc.element.s3.AWS.Service.prototype.initialize)
- description and source-code
```javascript
function initialize(config) {
  var svcConfig = AWS.config[this.serviceIdentifier];

  this.config = new AWS.Config(AWS.config);
  if (svcConfig) this.config.update(svcConfig, true);
  if (config) this.config.update(config, true);

  this.validateService();
  if (!this.config.endpoint) regionConfig(this);

  this.config.endpoint = this.endpointFromTemplate(this.config.endpoint);
  this.setEndpoint(this.config.endpoint);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Service.prototype.loadServiceClass"></a>[function <span class="apidocSignatureSpan">s3.AWS.Service.prototype.</span>loadServiceClass (serviceConfig)](#apidoc.element.s3.AWS.Service.prototype.loadServiceClass)
- description and source-code
```javascript
function loadServiceClass(serviceConfig) {
  var config = serviceConfig;
  if (!AWS.util.isEmpty(this.api)) {
    return null;
  } else if (config.apiConfig) {
    return AWS.Service.defineServiceApi(this.constructor, config.apiConfig);
  } else if (!this.constructor.services) {
    return null;
  } else {
    config = new AWS.Config(AWS.config);
    config.update(serviceConfig, true);
    var version = config.apiVersions[this.constructor.serviceIdentifier];
    version = version || config.apiVersion;
    return this.getLatestServiceClass(version);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Service.prototype.makeRequest"></a>[function <span class="apidocSignatureSpan">s3.AWS.Service.prototype.</span>makeRequest (operation, params, callback)](#apidoc.element.s3.AWS.Service.prototype.makeRequest)
- description and source-code
```javascript
function makeRequest(operation, params, callback) {
  if (typeof params === 'function') {
    callback = params;
    params = null;
  }

  params = params || {};
  if (this.config.params) { // copy only toplevel bound params
    var rules = this.api.operations[operation];
    if (rules) {
      params = AWS.util.copy(params);
      AWS.util.each(this.config.params, function(key, value) {
        if (rules.input.members[key]) {
          if (params[key] === undefined || params[key] === null) {
            params[key] = value;
          }
        }
      });
    }
  }

  var request = new AWS.Request(this, operation, params);
  this.addAllRequestListeners(request);

  if (callback) request.send(callback);
  return request;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Service.prototype.makeUnauthenticatedRequest"></a>[function <span class="apidocSignatureSpan">s3.AWS.Service.prototype.</span>makeUnauthenticatedRequest (operation, params, callback)](#apidoc.element.s3.AWS.Service.prototype.makeUnauthenticatedRequest)
- description and source-code
```javascript
function makeUnauthenticatedRequest(operation, params, callback) {
  if (typeof params === 'function') {
    callback = params;
    params = {};
  }

  var request = this.makeRequest(operation, params).toUnauthenticated();
  return callback ? request.send(callback) : request;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Service.prototype.networkingError"></a>[function <span class="apidocSignatureSpan">s3.AWS.Service.prototype.</span>networkingError (error)](#apidoc.element.s3.AWS.Service.prototype.networkingError)
- description and source-code
```javascript
function networkingError(error) {
  return error.code === 'NetworkingError';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Service.prototype.numRetries"></a>[function <span class="apidocSignatureSpan">s3.AWS.Service.prototype.</span>numRetries ()](#apidoc.element.s3.AWS.Service.prototype.numRetries)
- description and source-code
```javascript
function numRetries() {
  if (this.config.maxRetries !== undefined) {
    return this.config.maxRetries;
  } else {
    return this.defaultRetryCount;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Service.prototype.paginationConfig"></a>[function <span class="apidocSignatureSpan">s3.AWS.Service.prototype.</span>paginationConfig (operation, throwException)](#apidoc.element.s3.AWS.Service.prototype.paginationConfig)
- description and source-code
```javascript
function paginationConfig(operation, throwException) {
  var paginator = this.api.operations[operation].paginator;
  if (!paginator) {
    if (throwException) {
      var e = new Error();
      throw AWS.util.error(e, 'No pagination configuration for ' + operation);
    }
    return null;
  }

  return paginator;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Service.prototype.retryDelays"></a>[function <span class="apidocSignatureSpan">s3.AWS.Service.prototype.</span>retryDelays ()](#apidoc.element.s3.AWS.Service.prototype.retryDelays)
- description and source-code
```javascript
function retryDelays() {
  var retryCount = this.numRetries();
  var delays = [];
  for (var i = 0; i < retryCount; ++i) {
    delays[i] = Math.pow(2, i) * 30;
  }
  return delays;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Service.prototype.retryableError"></a>[function <span class="apidocSignatureSpan">s3.AWS.Service.prototype.</span>retryableError (error)](#apidoc.element.s3.AWS.Service.prototype.retryableError)
- description and source-code
```javascript
function retryableError(error) {
  if (this.networkingError(error)) return true;
  if (this.expiredCredentialsError(error)) return true;
  if (this.throttledError(error)) return true;
  if (error.statusCode >= 500) return true;
  return false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Service.prototype.serviceInterface"></a>[function <span class="apidocSignatureSpan">s3.AWS.Service.prototype.</span>serviceInterface ()](#apidoc.element.s3.AWS.Service.prototype.serviceInterface)
- description and source-code
```javascript
function serviceInterface() {
  switch (this.api.protocol) {
    case 'ec2': return AWS.EventListeners.Query;
    case 'query': return AWS.EventListeners.Query;
    case 'json': return AWS.EventListeners.Json;
    case 'rest-json': return AWS.EventListeners.RestJson;
    case 'rest-xml': return AWS.EventListeners.RestXml;
  }
  if (this.api.protocol) {
    throw new Error('Invalid service 'protocol\' ' +
      this.api.protocol + ' in API config');
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Service.prototype.setEndpoint"></a>[function <span class="apidocSignatureSpan">s3.AWS.Service.prototype.</span>setEndpoint (endpoint)](#apidoc.element.s3.AWS.Service.prototype.setEndpoint)
- description and source-code
```javascript
function setEndpoint(endpoint) {
  this.endpoint = new AWS.Endpoint(endpoint, this.config);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Service.prototype.setupRequestListeners"></a>[function <span class="apidocSignatureSpan">s3.AWS.Service.prototype.</span>setupRequestListeners ()](#apidoc.element.s3.AWS.Service.prototype.setupRequestListeners)
- description and source-code
```javascript
function setupRequestListeners() {
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Service.prototype.successfulResponse"></a>[function <span class="apidocSignatureSpan">s3.AWS.Service.prototype.</span>successfulResponse (resp)](#apidoc.element.s3.AWS.Service.prototype.successfulResponse)
- description and source-code
```javascript
function successfulResponse(resp) {
  return resp.httpResponse.statusCode < 300;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Service.prototype.throttledError"></a>[function <span class="apidocSignatureSpan">s3.AWS.Service.prototype.</span>throttledError (error)](#apidoc.element.s3.AWS.Service.prototype.throttledError)
- description and source-code
```javascript
function throttledError(error) {
  // this logic varies between services
  switch (error.code) {
    case 'ProvisionedThroughputExceededException':
    case 'Throttling':
      return true;
    default:
      return false;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Service.prototype.validateService"></a>[function <span class="apidocSignatureSpan">s3.AWS.Service.prototype.</span>validateService ()](#apidoc.element.s3.AWS.Service.prototype.validateService)
- description and source-code
```javascript
function validateService() {
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Service.prototype.waitFor"></a>[function <span class="apidocSignatureSpan">s3.AWS.Service.prototype.</span>waitFor (state, params, callback)](#apidoc.element.s3.AWS.Service.prototype.waitFor)
- description and source-code
```javascript
function waitFor(state, params, callback) {
  var waiter = new AWS.ResourceWaiter(this, state);
  return waiter.wait(params, callback);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.SharedIniFileCredentials"></a>[module s3.AWS.SharedIniFileCredentials](#apidoc.module.s3.AWS.SharedIniFileCredentials)

#### <a name="apidoc.element.s3.AWS.SharedIniFileCredentials.SharedIniFileCredentials"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>SharedIniFileCredentials (options)](#apidoc.element.s3.AWS.SharedIniFileCredentials.SharedIniFileCredentials)
- description and source-code
```javascript
function SharedIniFileCredentials(options) {
  AWS.Credentials.call(this);

  options = options || {};

  this.filename = options.filename;
  this.profile = options.profile || process.env.AWS_PROFILE || 'default';
  this.get(function() {});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.SharedIniFileCredentials.__super__"></a>[function <span class="apidocSignatureSpan">s3.AWS.SharedIniFileCredentials.</span>__super__ ()](#apidoc.element.s3.AWS.SharedIniFileCredentials.__super__)
- description and source-code
```javascript
function Credentials() {
  // hide secretAccessKey from being displayed with util.inspect
  AWS.util.hideProperties(this, ['secretAccessKey']);

  this.expired = false;
  this.expireTime = null;
  if (arguments.length === 1 && typeof arguments[0] === 'object') {
    var creds = arguments[0].credentials || arguments[0];
    this.accessKeyId = creds.accessKeyId;
    this.secretAccessKey = creds.secretAccessKey;
    this.sessionToken = creds.sessionToken;
  } else {
    this.accessKeyId = arguments[0];
    this.secretAccessKey = arguments[1];
    this.sessionToken = arguments[2];
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.SharedIniFileCredentials.prototype"></a>[module s3.AWS.SharedIniFileCredentials.prototype](#apidoc.module.s3.AWS.SharedIniFileCredentials.prototype)

#### <a name="apidoc.element.s3.AWS.SharedIniFileCredentials.prototype.constructor"></a>[function <span class="apidocSignatureSpan">s3.AWS.SharedIniFileCredentials.prototype.</span>constructor (options)](#apidoc.element.s3.AWS.SharedIniFileCredentials.prototype.constructor)
- description and source-code
```javascript
function SharedIniFileCredentials(options) {
  AWS.Credentials.call(this);

  options = options || {};

  this.filename = options.filename;
  this.profile = options.profile || process.env.AWS_PROFILE || 'default';
  this.get(function() {});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.SharedIniFileCredentials.prototype.loadDefaultFilename"></a>[function <span class="apidocSignatureSpan">s3.AWS.SharedIniFileCredentials.prototype.</span>loadDefaultFilename ()](#apidoc.element.s3.AWS.SharedIniFileCredentials.prototype.loadDefaultFilename)
- description and source-code
```javascript
function loadDefaultFilename() {
  var env = process.env;
  var home = env.HOME ||
             env.USERPROFILE ||
             (env.HOMEPATH ? ((env.HOMEDRIVE || 'C:/') + env.HOMEPATH) : null);
  if (!home) {
    throw AWS.util.error(
      new Error('Cannot load credentials, HOME path not set'));
  }

  this.filename = path.join(home, '.aws', 'credentials');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.SharedIniFileCredentials.prototype.refresh"></a>[function <span class="apidocSignatureSpan">s3.AWS.SharedIniFileCredentials.prototype.</span>refresh (callback)](#apidoc.element.s3.AWS.SharedIniFileCredentials.prototype.refresh)
- description and source-code
```javascript
function refresh(callback) {
  if (!callback) callback = function(err) { if (err) throw err; };
  try {
    if (!this.filename) this.loadDefaultFilename();
    var creds = AWS.util.ini.parse(AWS.util.readFileSync(this.filename));
    if (typeof creds[this.profile] === 'object') {
      this.accessKeyId = creds[this.profile]['aws_access_key_id'];
      this.secretAccessKey = creds[this.profile]['aws_secret_access_key'];
      this.sessionToken = creds[this.profile]['aws_session_token'];
    }

    if (!this.accessKeyId || !this.secretAccessKey) {
      throw new Error('Credentials not set in ' + this.filename +
                      ' using profile ' + this.profile);
    }
    this.expired = false;
    callback();
  } catch (err) {
    callback(err);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.Signers"></a>[module s3.AWS.Signers](#apidoc.module.s3.AWS.Signers)

#### <a name="apidoc.element.s3.AWS.Signers.Presign"></a>[function <span class="apidocSignatureSpan">s3.AWS.Signers.</span>Presign ()](#apidoc.element.s3.AWS.Signers.Presign)
- description and source-code
```javascript
Presign = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Signers.RequestSigner"></a>[function <span class="apidocSignatureSpan">s3.AWS.Signers.</span>RequestSigner (request)](#apidoc.element.s3.AWS.Signers.RequestSigner)
- description and source-code
```javascript
function RequestSigner(request) {
  this.request = request;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Signers.S3"></a>[function <span class="apidocSignatureSpan">s3.AWS.Signers.</span>S3 ()](#apidoc.element.s3.AWS.Signers.S3)
- description and source-code
```javascript
S3 = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
...
  s3RetryCount: 3,    // this is the default
  s3RetryDelay: 1000, // this is the default
  multipartUploadThreshold: 20971520, // this is the default (20 MB)
  multipartUploadSize: 15728640, // this is the default (15 MB)
  s3Options: {
    accessKeyId: "your s3 key",
    secretAccessKey: "your s3 secret",
    // any other options are passed to new AWS.S3()
    // See: http://docs.aws.amazon.com/AWSJavaScriptSDK/latest/AWS/Config.html#constructor-property
  },
});
'''

### Create a client from existing AWS.S3 object
...
```

#### <a name="apidoc.element.s3.AWS.Signers.V2"></a>[function <span class="apidocSignatureSpan">s3.AWS.Signers.</span>V2 ()](#apidoc.element.s3.AWS.Signers.V2)
- description and source-code
```javascript
V2 = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Signers.V3"></a>[function <span class="apidocSignatureSpan">s3.AWS.Signers.</span>V3 ()](#apidoc.element.s3.AWS.Signers.V3)
- description and source-code
```javascript
V3 = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Signers.V3Https"></a>[function <span class="apidocSignatureSpan">s3.AWS.Signers.</span>V3Https ()](#apidoc.element.s3.AWS.Signers.V3Https)
- description and source-code
```javascript
V3Https = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Signers.V4"></a>[function <span class="apidocSignatureSpan">s3.AWS.Signers.</span>V4 (request, serviceName)](#apidoc.element.s3.AWS.Signers.V4)
- description and source-code
```javascript
function V4(request, serviceName) {
  AWS.Signers.RequestSigner.call(this, request);
  this.serviceName = serviceName;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.Signers.Presign.prototype"></a>[module s3.AWS.Signers.Presign.prototype](#apidoc.module.s3.AWS.Signers.Presign.prototype)

#### <a name="apidoc.element.s3.AWS.Signers.Presign.prototype.constructor"></a>[function <span class="apidocSignatureSpan">s3.AWS.Signers.Presign.prototype.</span>constructor ()](#apidoc.element.s3.AWS.Signers.Presign.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Signers.Presign.prototype.sign"></a>[function <span class="apidocSignatureSpan">s3.AWS.Signers.Presign.prototype.</span>sign (request, expireTime, callback)](#apidoc.element.s3.AWS.Signers.Presign.prototype.sign)
- description and source-code
```javascript
function sign(request, expireTime, callback) {
  request.httpRequest.headers[expiresHeader] = expireTime || 3600;
  request.on('build', signedUrlBuilder);
  request.on('sign', signedUrlSigner);
  request.removeListener('afterBuild',
    AWS.EventListeners.Core.SET_CONTENT_LENGTH);

  request.emit('beforePresign', [request]);

  if (callback) {
    request.build(function() {
      if (this.response.error) callback(this.response.error);
      else {
        callback(null, AWS.util.urlFormat(request.httpRequest.endpoint));
      }
    });
  } else {
    request.build();
    return AWS.util.urlFormat(request.httpRequest.endpoint);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.Signers.RequestSigner.prototype"></a>[module s3.AWS.Signers.RequestSigner.prototype](#apidoc.module.s3.AWS.Signers.RequestSigner.prototype)

#### <a name="apidoc.element.s3.AWS.Signers.RequestSigner.prototype.constructor"></a>[function <span class="apidocSignatureSpan">s3.AWS.Signers.RequestSigner.prototype.</span>constructor (request)](#apidoc.element.s3.AWS.Signers.RequestSigner.prototype.constructor)
- description and source-code
```javascript
function RequestSigner(request) {
  this.request = request;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.Signers.S3.prototype"></a>[module s3.AWS.Signers.S3.prototype](#apidoc.module.s3.AWS.Signers.S3.prototype)

#### <a name="apidoc.element.s3.AWS.Signers.S3.prototype.addAuthorization"></a>[function <span class="apidocSignatureSpan">s3.AWS.Signers.S3.prototype.</span>addAuthorization (credentials, date)](#apidoc.element.s3.AWS.Signers.S3.prototype.addAuthorization)
- description and source-code
```javascript
function addAuthorization(credentials, date) {
  if (!this.request.headers['presigned-expires']) {
    this.request.headers['X-Amz-Date'] = AWS.util.date.rfc822(date);
  }

  if (credentials.sessionToken) {
    // presigned URLs require this header to be lowercased
    this.request.headers['x-amz-security-token'] = credentials.sessionToken;
  }

  var signature = this.sign(credentials.secretAccessKey, this.stringToSign());
  var auth = 'AWS ' + credentials.accessKeyId + ':' + signature;

  this.request.headers['Authorization'] = auth;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Signers.S3.prototype.canonicalizedAmzHeaders"></a>[function <span class="apidocSignatureSpan">s3.AWS.Signers.S3.prototype.</span>canonicalizedAmzHeaders ()](#apidoc.element.s3.AWS.Signers.S3.prototype.canonicalizedAmzHeaders)
- description and source-code
```javascript
function canonicalizedAmzHeaders() {

  var amzHeaders = [];

  AWS.util.each(this.request.headers, function (name) {
    if (name.match(/^x-amz-/i))
      amzHeaders.push(name);
  });

  amzHeaders.sort(function (a, b) {
    return a.toLowerCase() < b.toLowerCase() ? -1 : 1;
  });

  var parts = [];
  AWS.util.arrayEach.call(this, amzHeaders, function (name) {
    parts.push(name.toLowerCase() + ':' + String(this.request.headers[name]));
  });

  return parts.join('\n');

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Signers.S3.prototype.canonicalizedResource"></a>[function <span class="apidocSignatureSpan">s3.AWS.Signers.S3.prototype.</span>canonicalizedResource ()](#apidoc.element.s3.AWS.Signers.S3.prototype.canonicalizedResource)
- description and source-code
```javascript
function canonicalizedResource() {

  var r = this.request;

  var parts = r.path.split('?');
  var path = parts[0];
  var querystring = parts[1];

  var resource = '';

  if (r.virtualHostedBucket)
    resource += '/' + r.virtualHostedBucket;

  resource += path;

  if (querystring) {

    // collect a list of sub resources and query params that need to be signed
    var resources = [];

    AWS.util.arrayEach.call(this, querystring.split('&'), function (param) {
      var name = param.split('=')[0];
      var value = param.split('=')[1];
      if (this.subResources[name] || this.responseHeaders[name]) {
        var subresource = { name: name };
        if (value !== undefined) {
          if (this.subResources[name]) {
            subresource.value = value;
          } else {
            subresource.value = decodeURIComponent(value);
          }
        }
        resources.push(subresource);
      }
    });

    resources.sort(function (a, b) { return a.name < b.name ? -1 : 1; });

    if (resources.length) {

      querystring = [];
      AWS.util.arrayEach(resources, function (resource) {
        if (resource.value === undefined)
          querystring.push(resource.name);
        else
          querystring.push(resource.name + '=' + resource.value);
      });

      resource += '?' + querystring.join('&');
    }

  }

  return resource;

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Signers.S3.prototype.constructor"></a>[function <span class="apidocSignatureSpan">s3.AWS.Signers.S3.prototype.</span>constructor ()](#apidoc.element.s3.AWS.Signers.S3.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Signers.S3.prototype.sign"></a>[function <span class="apidocSignatureSpan">s3.AWS.Signers.S3.prototype.</span>sign (secret, string)](#apidoc.element.s3.AWS.Signers.S3.prototype.sign)
- description and source-code
```javascript
function sign(secret, string) {
  return AWS.util.crypto.hmac(secret, string, 'base64', 'sha1');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Signers.S3.prototype.stringToSign"></a>[function <span class="apidocSignatureSpan">s3.AWS.Signers.S3.prototype.</span>stringToSign ()](#apidoc.element.s3.AWS.Signers.S3.prototype.stringToSign)
- description and source-code
```javascript
function stringToSign() {
  var r = this.request;

  var parts = [];
  parts.push(r.method);
  parts.push(r.headers['Content-MD5'] || '');
  parts.push(r.headers['Content-Type'] || '');

  // This is the "Date" header, but we use X-Amz-Date.
  // The S3 signing mechanism requires us to pass an empty
  // string for this Date header regardless.
  parts.push(r.headers['presigned-expires'] || '');

  var headers = this.canonicalizedAmzHeaders();
  if (headers) parts.push(headers);
  parts.push(this.canonicalizedResource());

  return parts.join('\n');

}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.Signers.V2.prototype"></a>[module s3.AWS.Signers.V2.prototype](#apidoc.module.s3.AWS.Signers.V2.prototype)

#### <a name="apidoc.element.s3.AWS.Signers.V2.prototype.addAuthorization"></a>[function <span class="apidocSignatureSpan">s3.AWS.Signers.V2.prototype.</span>addAuthorization (credentials, date)](#apidoc.element.s3.AWS.Signers.V2.prototype.addAuthorization)
- description and source-code
```javascript
function addAuthorization(credentials, date) {

  if (!date) date = AWS.util.date.getDate();

  var r = this.request;

  r.params.Timestamp = AWS.util.date.iso8601(date);
  r.params.SignatureVersion = '2';
  r.params.SignatureMethod = 'HmacSHA256';
  r.params.AWSAccessKeyId = credentials.accessKeyId;

  if (credentials.sessionToken) {
    r.params.SecurityToken = credentials.sessionToken;
  }

  delete r.params.Signature; // delete old Signature for re-signing
  r.params.Signature = this.signature(credentials);

  r.body = AWS.util.queryParamsToString(r.params);
  r.headers['Content-Length'] = r.body.length;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Signers.V2.prototype.constructor"></a>[function <span class="apidocSignatureSpan">s3.AWS.Signers.V2.prototype.</span>constructor ()](#apidoc.element.s3.AWS.Signers.V2.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Signers.V2.prototype.signature"></a>[function <span class="apidocSignatureSpan">s3.AWS.Signers.V2.prototype.</span>signature (credentials)](#apidoc.element.s3.AWS.Signers.V2.prototype.signature)
- description and source-code
```javascript
function signature(credentials) {
  return AWS.util.crypto.hmac(credentials.secretAccessKey, this.stringToSign(), 'base64');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Signers.V2.prototype.stringToSign"></a>[function <span class="apidocSignatureSpan">s3.AWS.Signers.V2.prototype.</span>stringToSign ()](#apidoc.element.s3.AWS.Signers.V2.prototype.stringToSign)
- description and source-code
```javascript
function stringToSign() {
  var parts = [];
  parts.push(this.request.method);
  parts.push(this.request.endpoint.host.toLowerCase());
  parts.push(this.request.pathname());
  parts.push(AWS.util.queryParamsToString(this.request.params));
  return parts.join('\n');
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.Signers.V3.prototype"></a>[module s3.AWS.Signers.V3.prototype](#apidoc.module.s3.AWS.Signers.V3.prototype)

#### <a name="apidoc.element.s3.AWS.Signers.V3.prototype.addAuthorization"></a>[function <span class="apidocSignatureSpan">s3.AWS.Signers.V3.prototype.</span>addAuthorization (credentials, date)](#apidoc.element.s3.AWS.Signers.V3.prototype.addAuthorization)
- description and source-code
```javascript
function addAuthorization(credentials, date) {

  var datetime = AWS.util.date.rfc822(date);

  this.request.headers['X-Amz-Date'] = datetime;

  if (credentials.sessionToken) {
    this.request.headers['x-amz-security-token'] = credentials.sessionToken;
  }

  this.request.headers['X-Amzn-Authorization'] =
    this.authorization(credentials, datetime);

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Signers.V3.prototype.authorization"></a>[function <span class="apidocSignatureSpan">s3.AWS.Signers.V3.prototype.</span>authorization (credentials)](#apidoc.element.s3.AWS.Signers.V3.prototype.authorization)
- description and source-code
```javascript
function authorization(credentials) {
  return 'AWS3 ' +
    'AWSAccessKeyId=' + credentials.accessKeyId + ',' +
    'Algorithm=HmacSHA256,' +
    'SignedHeaders=' + this.signedHeaders() + ',' +
    'Signature=' + this.signature(credentials);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Signers.V3.prototype.canonicalHeaders"></a>[function <span class="apidocSignatureSpan">s3.AWS.Signers.V3.prototype.</span>canonicalHeaders ()](#apidoc.element.s3.AWS.Signers.V3.prototype.canonicalHeaders)
- description and source-code
```javascript
function canonicalHeaders() {
  var headers = this.request.headers;
  var parts = [];
  AWS.util.arrayEach(this.headersToSign(), function iterator(h) {
    parts.push(h.toLowerCase().trim() + ':' + String(headers[h]).trim());
  });
  return parts.sort().join('\n') + '\n';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Signers.V3.prototype.constructor"></a>[function <span class="apidocSignatureSpan">s3.AWS.Signers.V3.prototype.</span>constructor ()](#apidoc.element.s3.AWS.Signers.V3.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Signers.V3.prototype.headersToSign"></a>[function <span class="apidocSignatureSpan">s3.AWS.Signers.V3.prototype.</span>headersToSign ()](#apidoc.element.s3.AWS.Signers.V3.prototype.headersToSign)
- description and source-code
```javascript
function headersToSign() {
  var headers = [];
  AWS.util.each(this.request.headers, function iterator(k) {
    if (k === 'Host' || k === 'Content-Encoding' || k.match(/^X-Amz/i)) {
      headers.push(k);
    }
  });
  return headers;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Signers.V3.prototype.signature"></a>[function <span class="apidocSignatureSpan">s3.AWS.Signers.V3.prototype.</span>signature (credentials)](#apidoc.element.s3.AWS.Signers.V3.prototype.signature)
- description and source-code
```javascript
function signature(credentials) {
  return AWS.util.crypto.hmac(credentials.secretAccessKey, this.stringToSign(), 'base64');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Signers.V3.prototype.signedHeaders"></a>[function <span class="apidocSignatureSpan">s3.AWS.Signers.V3.prototype.</span>signedHeaders ()](#apidoc.element.s3.AWS.Signers.V3.prototype.signedHeaders)
- description and source-code
```javascript
function signedHeaders() {
  var headers = [];
  AWS.util.arrayEach(this.headersToSign(), function iterator(h) {
    headers.push(h.toLowerCase());
  });
  return headers.sort().join(';');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Signers.V3.prototype.stringToSign"></a>[function <span class="apidocSignatureSpan">s3.AWS.Signers.V3.prototype.</span>stringToSign ()](#apidoc.element.s3.AWS.Signers.V3.prototype.stringToSign)
- description and source-code
```javascript
function stringToSign() {
  var parts = [];
  parts.push(this.request.method);
  parts.push('/');
  parts.push('');
  parts.push(this.canonicalHeaders());
  parts.push(this.request.body);
  return AWS.util.crypto.sha256(parts.join('\n'));
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.Signers.V3Https.prototype"></a>[module s3.AWS.Signers.V3Https.prototype](#apidoc.module.s3.AWS.Signers.V3Https.prototype)

#### <a name="apidoc.element.s3.AWS.Signers.V3Https.prototype.authorization"></a>[function <span class="apidocSignatureSpan">s3.AWS.Signers.V3Https.prototype.</span>authorization (credentials)](#apidoc.element.s3.AWS.Signers.V3Https.prototype.authorization)
- description and source-code
```javascript
function authorization(credentials) {
  return 'AWS3-HTTPS ' +
    'AWSAccessKeyId=' + credentials.accessKeyId + ',' +
    'Algorithm=HmacSHA256,' +
    'Signature=' + this.signature(credentials);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Signers.V3Https.prototype.constructor"></a>[function <span class="apidocSignatureSpan">s3.AWS.Signers.V3Https.prototype.</span>constructor ()](#apidoc.element.s3.AWS.Signers.V3Https.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Signers.V3Https.prototype.stringToSign"></a>[function <span class="apidocSignatureSpan">s3.AWS.Signers.V3Https.prototype.</span>stringToSign ()](#apidoc.element.s3.AWS.Signers.V3Https.prototype.stringToSign)
- description and source-code
```javascript
function stringToSign() {
  return this.request.headers['X-Amz-Date'];
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.Signers.V4.prototype"></a>[module s3.AWS.Signers.V4.prototype](#apidoc.module.s3.AWS.Signers.V4.prototype)

#### <a name="apidoc.element.s3.AWS.Signers.V4.prototype.addAuthorization"></a>[function <span class="apidocSignatureSpan">s3.AWS.Signers.V4.prototype.</span>addAuthorization (credentials, date)](#apidoc.element.s3.AWS.Signers.V4.prototype.addAuthorization)
- description and source-code
```javascript
function addAuthorization(credentials, date) {
  var datetime = AWS.util.date.iso8601(date).replace(/[:\-]|\.\d{3}/g, '');

  if (this.isPresigned()) {
    this.updateForPresigned(credentials, datetime);
  } else {
    this.addHeaders(credentials, datetime);
    this.updateBody(credentials);
  }

  this.request.headers['Authorization'] =
    this.authorization(credentials, datetime);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Signers.V4.prototype.addHeaders"></a>[function <span class="apidocSignatureSpan">s3.AWS.Signers.V4.prototype.</span>addHeaders (credentials, datetime)](#apidoc.element.s3.AWS.Signers.V4.prototype.addHeaders)
- description and source-code
```javascript
function addHeaders(credentials, datetime) {
  this.request.headers['X-Amz-Date'] = datetime;
  if (credentials.sessionToken) {
    this.request.headers['x-amz-security-token'] = credentials.sessionToken;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Signers.V4.prototype.authorization"></a>[function <span class="apidocSignatureSpan">s3.AWS.Signers.V4.prototype.</span>authorization (credentials, datetime)](#apidoc.element.s3.AWS.Signers.V4.prototype.authorization)
- description and source-code
```javascript
function authorization(credentials, datetime) {
  var parts = [];
  var credString = this.credentialString(datetime);
  parts.push(this.algorithm + ' Credential=' +
    credentials.accessKeyId + '/' + credString);
  parts.push('SignedHeaders=' + this.signedHeaders());
  parts.push('Signature=' + this.signature(credentials, datetime));
  return parts.join(', ');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Signers.V4.prototype.canonicalHeaderValues"></a>[function <span class="apidocSignatureSpan">s3.AWS.Signers.V4.prototype.</span>canonicalHeaderValues (values)](#apidoc.element.s3.AWS.Signers.V4.prototype.canonicalHeaderValues)
- description and source-code
```javascript
function canonicalHeaderValues(values) {
  return values.replace(/\s+/g, ' ').replace(/^\s+|\s+$/g, '');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Signers.V4.prototype.canonicalHeaders"></a>[function <span class="apidocSignatureSpan">s3.AWS.Signers.V4.prototype.</span>canonicalHeaders ()](#apidoc.element.s3.AWS.Signers.V4.prototype.canonicalHeaders)
- description and source-code
```javascript
function canonicalHeaders() {
  var headers = [];
  AWS.util.each.call(this, this.request.headers, function (key, item) {
    headers.push([key, item]);
  });
  headers.sort(function (a, b) {
    return a[0].toLowerCase() < b[0].toLowerCase() ? -1 : 1;
  });
  var parts = [];
  AWS.util.arrayEach.call(this, headers, function (item) {
    var key = item[0].toLowerCase();
    if (this.isSignableHeader(key)) {
      parts.push(key + ':' +
        this.canonicalHeaderValues(item[1].toString()));
    }
  });
  return parts.join('\n');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Signers.V4.prototype.canonicalString"></a>[function <span class="apidocSignatureSpan">s3.AWS.Signers.V4.prototype.</span>canonicalString ()](#apidoc.element.s3.AWS.Signers.V4.prototype.canonicalString)
- description and source-code
```javascript
function canonicalString() {
  var parts = [], pathname = this.request.pathname();
  if (this.serviceName !== 's3') pathname = AWS.util.uriEscapePath(pathname);

  parts.push(this.request.method);
  parts.push(pathname);
  parts.push(this.request.search());
  parts.push(this.canonicalHeaders() + '\n');
  parts.push(this.signedHeaders());
  parts.push(this.hexEncodedBodyHash());
  return parts.join('\n');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Signers.V4.prototype.constructor"></a>[function <span class="apidocSignatureSpan">s3.AWS.Signers.V4.prototype.</span>constructor (request, serviceName)](#apidoc.element.s3.AWS.Signers.V4.prototype.constructor)
- description and source-code
```javascript
function V4(request, serviceName) {
  AWS.Signers.RequestSigner.call(this, request);
  this.serviceName = serviceName;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Signers.V4.prototype.credentialString"></a>[function <span class="apidocSignatureSpan">s3.AWS.Signers.V4.prototype.</span>credentialString (datetime)](#apidoc.element.s3.AWS.Signers.V4.prototype.credentialString)
- description and source-code
```javascript
function credentialString(datetime) {
  var parts = [];
  parts.push(datetime.substr(0, 8));
  parts.push(this.request.region);
  parts.push(this.serviceName);
  parts.push('aws4_request');
  return parts.join('/');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Signers.V4.prototype.hexEncodedBodyHash"></a>[function <span class="apidocSignatureSpan">s3.AWS.Signers.V4.prototype.</span>hexEncodedBodyHash ()](#apidoc.element.s3.AWS.Signers.V4.prototype.hexEncodedBodyHash)
- description and source-code
```javascript
function hexEncodedBodyHash() {
  if (this.isPresigned() && this.serviceName === 's3') {
    return 'UNSIGNED-PAYLOAD';
  } else if (this.request.headers['X-Amz-Content-Sha256']) {
    return this.request.headers['X-Amz-Content-Sha256'];
  } else {
    return this.hexEncodedHash(this.request.body || '');
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Signers.V4.prototype.hexEncodedHash"></a>[function <span class="apidocSignatureSpan">s3.AWS.Signers.V4.prototype.</span>hexEncodedHash (string)](#apidoc.element.s3.AWS.Signers.V4.prototype.hexEncodedHash)
- description and source-code
```javascript
function hash(string) {
  return AWS.util.crypto.sha256(string, 'hex');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Signers.V4.prototype.isPresigned"></a>[function <span class="apidocSignatureSpan">s3.AWS.Signers.V4.prototype.</span>isPresigned ()](#apidoc.element.s3.AWS.Signers.V4.prototype.isPresigned)
- description and source-code
```javascript
function isPresigned() {
  return this.request.headers[expiresHeader] ? true : false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Signers.V4.prototype.isSignableHeader"></a>[function <span class="apidocSignatureSpan">s3.AWS.Signers.V4.prototype.</span>isSignableHeader (key)](#apidoc.element.s3.AWS.Signers.V4.prototype.isSignableHeader)
- description and source-code
```javascript
function isSignableHeader(key) {
  if (key.toLowerCase().indexOf('x-amz-') === 0) return true;
  return this.unsignableHeaders.indexOf(key) < 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Signers.V4.prototype.signature"></a>[function <span class="apidocSignatureSpan">s3.AWS.Signers.V4.prototype.</span>signature (credentials, datetime)](#apidoc.element.s3.AWS.Signers.V4.prototype.signature)
- description and source-code
```javascript
function signature(credentials, datetime) {
  var cache = cachedSecret[this.serviceName];
  var date = datetime.substr(0, 8);
  if (!cache ||
      cache.akid !== credentials.accessKeyId ||
      cache.region !== this.request.region ||
      cache.date !== date) {
    var kSecret = credentials.secretAccessKey;
    var kDate = AWS.util.crypto.hmac('AWS4' + kSecret, date, 'buffer');
    var kRegion = AWS.util.crypto.hmac(kDate, this.request.region, 'buffer');
    var kService = AWS.util.crypto.hmac(kRegion, this.serviceName, 'buffer');
    var kCredentials = AWS.util.crypto.hmac(kService, 'aws4_request', 'buffer');
    cachedSecret[this.serviceName] = {
      region: this.request.region, date: date,
      key: kCredentials, akid: credentials.accessKeyId
    };
  }

  var key = cachedSecret[this.serviceName].key;
  return AWS.util.crypto.hmac(key, this.stringToSign(datetime), 'hex');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Signers.V4.prototype.signedHeaders"></a>[function <span class="apidocSignatureSpan">s3.AWS.Signers.V4.prototype.</span>signedHeaders ()](#apidoc.element.s3.AWS.Signers.V4.prototype.signedHeaders)
- description and source-code
```javascript
function signedHeaders() {
  var keys = [];
  AWS.util.each.call(this, this.request.headers, function (key) {
    key = key.toLowerCase();
    if (this.isSignableHeader(key)) keys.push(key);
  });
  return keys.sort().join(';');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Signers.V4.prototype.stringToSign"></a>[function <span class="apidocSignatureSpan">s3.AWS.Signers.V4.prototype.</span>stringToSign (datetime)](#apidoc.element.s3.AWS.Signers.V4.prototype.stringToSign)
- description and source-code
```javascript
function stringToSign(datetime) {
  var parts = [];
  parts.push('AWS4-HMAC-SHA256');
  parts.push(datetime);
  parts.push(this.credentialString(datetime));
  parts.push(this.hexEncodedHash(this.canonicalString()));
  return parts.join('\n');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Signers.V4.prototype.updateBody"></a>[function <span class="apidocSignatureSpan">s3.AWS.Signers.V4.prototype.</span>updateBody (credentials)](#apidoc.element.s3.AWS.Signers.V4.prototype.updateBody)
- description and source-code
```javascript
function updateBody(credentials) {
  if (this.request.params) {
    this.request.params.AWSAccessKeyId = credentials.accessKeyId;

    if (credentials.sessionToken) {
      this.request.params.SecurityToken = credentials.sessionToken;
    }

    this.request.body = AWS.util.queryParamsToString(this.request.params);
    this.request.headers['Content-Length'] = this.request.body.length;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Signers.V4.prototype.updateForPresigned"></a>[function <span class="apidocSignatureSpan">s3.AWS.Signers.V4.prototype.</span>updateForPresigned (credentials, datetime)](#apidoc.element.s3.AWS.Signers.V4.prototype.updateForPresigned)
- description and source-code
```javascript
function updateForPresigned(credentials, datetime) {
  var credString = this.credentialString(datetime);
  var qs = {
    'X-Amz-Date': datetime,
    'X-Amz-Algorithm': this.algorithm,
    'X-Amz-Credential': credentials.accessKeyId + '/' + credString,
    'X-Amz-Expires': this.request.headers[expiresHeader],
    'X-Amz-SignedHeaders': this.signedHeaders()
  };

  if (credentials.sessionToken) {
    qs['X-Amz-Security-Token'] = credentials.sessionToken;
  }

  if (this.request.headers['Content-Type']) {
    qs['Content-Type'] = this.request.headers['Content-Type'];
  }

  // need to pull in any other X-Amz-* headers
  AWS.util.each.call(this, this.request.headers, function(key, value) {
    if (key === expiresHeader) return;
    if (this.isSignableHeader(key) &&
        key.toLowerCase().indexOf('x-amz-') === 0) {
      qs[key] = value;
    }
  });

  var sep = this.request.path.indexOf('?') >= 0 ? '&' : '?';
  this.request.path += sep + AWS.util.queryParamsToString(qs);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.SimpleDB"></a>[module s3.AWS.SimpleDB](#apidoc.module.s3.AWS.SimpleDB)

#### <a name="apidoc.element.s3.AWS.SimpleDB.SimpleDB"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>SimpleDB ()](#apidoc.element.s3.AWS.SimpleDB.SimpleDB)
- description and source-code
```javascript
SimpleDB = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.SimpleDB.__super__"></a>[function <span class="apidocSignatureSpan">s3.AWS.SimpleDB.</span>__super__ (config)](#apidoc.element.s3.AWS.SimpleDB.__super__)
- description and source-code
```javascript
function Service(config) {
  if (!this.loadServiceClass) {
    throw AWS.util.error(new Error(),
      'Service must be constructed with 'new\' operator');
  }
  var ServiceClass = this.loadServiceClass(config || {});
  if (ServiceClass) return new ServiceClass(config);
  this.initialize(config);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.SimpleDB.prototype"></a>[module s3.AWS.SimpleDB.prototype](#apidoc.module.s3.AWS.SimpleDB.prototype)

#### <a name="apidoc.element.s3.AWS.SimpleDB.prototype.constructor"></a>[function <span class="apidocSignatureSpan">s3.AWS.SimpleDB.prototype.</span>constructor ()](#apidoc.element.s3.AWS.SimpleDB.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.StorageGateway"></a>[module s3.AWS.StorageGateway](#apidoc.module.s3.AWS.StorageGateway)

#### <a name="apidoc.element.s3.AWS.StorageGateway.StorageGateway"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>StorageGateway ()](#apidoc.element.s3.AWS.StorageGateway.StorageGateway)
- description and source-code
```javascript
StorageGateway = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.StorageGateway.__super__"></a>[function <span class="apidocSignatureSpan">s3.AWS.StorageGateway.</span>__super__ (config)](#apidoc.element.s3.AWS.StorageGateway.__super__)
- description and source-code
```javascript
function Service(config) {
  if (!this.loadServiceClass) {
    throw AWS.util.error(new Error(),
      'Service must be constructed with 'new\' operator');
  }
  var ServiceClass = this.loadServiceClass(config || {});
  if (ServiceClass) return new ServiceClass(config);
  this.initialize(config);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.StorageGateway.prototype"></a>[module s3.AWS.StorageGateway.prototype](#apidoc.module.s3.AWS.StorageGateway.prototype)

#### <a name="apidoc.element.s3.AWS.StorageGateway.prototype.constructor"></a>[function <span class="apidocSignatureSpan">s3.AWS.StorageGateway.prototype.</span>constructor ()](#apidoc.element.s3.AWS.StorageGateway.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.Support"></a>[module s3.AWS.Support](#apidoc.module.s3.AWS.Support)

#### <a name="apidoc.element.s3.AWS.Support.Support"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>Support ()](#apidoc.element.s3.AWS.Support.Support)
- description and source-code
```javascript
Support = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.Support.__super__"></a>[function <span class="apidocSignatureSpan">s3.AWS.Support.</span>__super__ (config)](#apidoc.element.s3.AWS.Support.__super__)
- description and source-code
```javascript
function Service(config) {
  if (!this.loadServiceClass) {
    throw AWS.util.error(new Error(),
      'Service must be constructed with 'new\' operator');
  }
  var ServiceClass = this.loadServiceClass(config || {});
  if (ServiceClass) return new ServiceClass(config);
  this.initialize(config);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.Support.prototype"></a>[module s3.AWS.Support.prototype](#apidoc.module.s3.AWS.Support.prototype)

#### <a name="apidoc.element.s3.AWS.Support.prototype.constructor"></a>[function <span class="apidocSignatureSpan">s3.AWS.Support.prototype.</span>constructor ()](#apidoc.element.s3.AWS.Support.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.TemporaryCredentials"></a>[module s3.AWS.TemporaryCredentials](#apidoc.module.s3.AWS.TemporaryCredentials)

#### <a name="apidoc.element.s3.AWS.TemporaryCredentials.TemporaryCredentials"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>TemporaryCredentials (params)](#apidoc.element.s3.AWS.TemporaryCredentials.TemporaryCredentials)
- description and source-code
```javascript
function TemporaryCredentials(params) {
  AWS.Credentials.call(this);
  this.loadMasterCredentials();
  this.expired = true;

  this.params = params || {};
  if (this.params.RoleArn) {
    this.params.RoleSessionName =
      this.params.RoleSessionName || 'temporary-credentials';
  }
  this.service = new AWS.STS({params: this.params});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.TemporaryCredentials.__super__"></a>[function <span class="apidocSignatureSpan">s3.AWS.TemporaryCredentials.</span>__super__ ()](#apidoc.element.s3.AWS.TemporaryCredentials.__super__)
- description and source-code
```javascript
function Credentials() {
  // hide secretAccessKey from being displayed with util.inspect
  AWS.util.hideProperties(this, ['secretAccessKey']);

  this.expired = false;
  this.expireTime = null;
  if (arguments.length === 1 && typeof arguments[0] === 'object') {
    var creds = arguments[0].credentials || arguments[0];
    this.accessKeyId = creds.accessKeyId;
    this.secretAccessKey = creds.secretAccessKey;
    this.sessionToken = creds.sessionToken;
  } else {
    this.accessKeyId = arguments[0];
    this.secretAccessKey = arguments[1];
    this.sessionToken = arguments[2];
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.TemporaryCredentials.prototype"></a>[module s3.AWS.TemporaryCredentials.prototype](#apidoc.module.s3.AWS.TemporaryCredentials.prototype)

#### <a name="apidoc.element.s3.AWS.TemporaryCredentials.prototype.constructor"></a>[function <span class="apidocSignatureSpan">s3.AWS.TemporaryCredentials.prototype.</span>constructor (params)](#apidoc.element.s3.AWS.TemporaryCredentials.prototype.constructor)
- description and source-code
```javascript
function TemporaryCredentials(params) {
  AWS.Credentials.call(this);
  this.loadMasterCredentials();
  this.expired = true;

  this.params = params || {};
  if (this.params.RoleArn) {
    this.params.RoleSessionName =
      this.params.RoleSessionName || 'temporary-credentials';
  }
  this.service = new AWS.STS({params: this.params});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.TemporaryCredentials.prototype.loadMasterCredentials"></a>[function <span class="apidocSignatureSpan">s3.AWS.TemporaryCredentials.prototype.</span>loadMasterCredentials ()](#apidoc.element.s3.AWS.TemporaryCredentials.prototype.loadMasterCredentials)
- description and source-code
```javascript
function loadMasterCredentials() {
  this.masterCredentials = AWS.config.credentials;
  while (this.masterCredentials.masterCredentials) {
    this.masterCredentials = this.masterCredentials.masterCredentials;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.TemporaryCredentials.prototype.refresh"></a>[function <span class="apidocSignatureSpan">s3.AWS.TemporaryCredentials.prototype.</span>refresh (callback)](#apidoc.element.s3.AWS.TemporaryCredentials.prototype.refresh)
- description and source-code
```javascript
function refresh(callback) {
  var self = this;
  if (!callback) callback = function(err) { if (err) throw err; };

  self.service.config.credentials = self.masterCredentials;
  var operation = self.params.RoleArn ?
    self.service.assumeRole : self.service.getSessionToken;
  operation.call(self.service, function (err, data) {
    if (!err) {
      self.service.credentialsFrom(data, self);
    }
    callback(err);
  });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.WebIdentityCredentials"></a>[module s3.AWS.WebIdentityCredentials](#apidoc.module.s3.AWS.WebIdentityCredentials)

#### <a name="apidoc.element.s3.AWS.WebIdentityCredentials.WebIdentityCredentials"></a>[function <span class="apidocSignatureSpan">s3.AWS.</span>WebIdentityCredentials (params)](#apidoc.element.s3.AWS.WebIdentityCredentials.WebIdentityCredentials)
- description and source-code
```javascript
function WebIdentityCredentials(params) {
  AWS.Credentials.call(this);
  this.expired = true;
  this.params = params;
  this.params.RoleSessionName = this.params.RoleSessionName || 'web-identity';
  this.service = new AWS.STS({params: this.params});
  this.data = null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.WebIdentityCredentials.__super__"></a>[function <span class="apidocSignatureSpan">s3.AWS.WebIdentityCredentials.</span>__super__ ()](#apidoc.element.s3.AWS.WebIdentityCredentials.__super__)
- description and source-code
```javascript
function Credentials() {
  // hide secretAccessKey from being displayed with util.inspect
  AWS.util.hideProperties(this, ['secretAccessKey']);

  this.expired = false;
  this.expireTime = null;
  if (arguments.length === 1 && typeof arguments[0] === 'object') {
    var creds = arguments[0].credentials || arguments[0];
    this.accessKeyId = creds.accessKeyId;
    this.secretAccessKey = creds.secretAccessKey;
    this.sessionToken = creds.sessionToken;
  } else {
    this.accessKeyId = arguments[0];
    this.secretAccessKey = arguments[1];
    this.sessionToken = arguments[2];
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.WebIdentityCredentials.prototype"></a>[module s3.AWS.WebIdentityCredentials.prototype](#apidoc.module.s3.AWS.WebIdentityCredentials.prototype)

#### <a name="apidoc.element.s3.AWS.WebIdentityCredentials.prototype.constructor"></a>[function <span class="apidocSignatureSpan">s3.AWS.WebIdentityCredentials.prototype.</span>constructor (params)](#apidoc.element.s3.AWS.WebIdentityCredentials.prototype.constructor)
- description and source-code
```javascript
function WebIdentityCredentials(params) {
  AWS.Credentials.call(this);
  this.expired = true;
  this.params = params;
  this.params.RoleSessionName = this.params.RoleSessionName || 'web-identity';
  this.service = new AWS.STS({params: this.params});
  this.data = null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.WebIdentityCredentials.prototype.refresh"></a>[function <span class="apidocSignatureSpan">s3.AWS.WebIdentityCredentials.prototype.</span>refresh (callback)](#apidoc.element.s3.AWS.WebIdentityCredentials.prototype.refresh)
- description and source-code
```javascript
function refresh(callback) {
  var self = this;
  if (!callback) callback = function(err) { if (err) throw err; };

  self.service.assumeRoleWithWebIdentity(function (err, data) {
    self.data = null;
    if (!err) {
      self.data = data;
      self.service.credentialsFrom(data, self);
    }
    callback(err);
  });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.XML"></a>[module s3.AWS.XML](#apidoc.module.s3.AWS.XML)

#### <a name="apidoc.element.s3.AWS.XML.Builder"></a>[function <span class="apidocSignatureSpan">s3.AWS.XML.</span>Builder ()](#apidoc.element.s3.AWS.XML.Builder)
- description and source-code
```javascript
function XmlBuilder() { }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.XML.Parser"></a>[function <span class="apidocSignatureSpan">s3.AWS.XML.</span>Parser ()](#apidoc.element.s3.AWS.XML.Parser)
- description and source-code
```javascript
function NodeXmlParser() { }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.XML.Builder.prototype"></a>[module s3.AWS.XML.Builder.prototype](#apidoc.module.s3.AWS.XML.Builder.prototype)

#### <a name="apidoc.element.s3.AWS.XML.Builder.prototype.toXML"></a>[function <span class="apidocSignatureSpan">s3.AWS.XML.Builder.prototype.</span>toXML (params, shape, rootElement)](#apidoc.element.s3.AWS.XML.Builder.prototype.toXML)
- description and source-code
```javascript
toXML = function (params, shape, rootElement) {
  var xml = builder.create(rootElement);
  applyNamespaces(xml, shape);
  serialize(xml, params, shape);
  return xml.children.length === 0 ? '' : xml.root().toString();
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.XML.Parser.prototype"></a>[module s3.AWS.XML.Parser.prototype](#apidoc.module.s3.AWS.XML.Parser.prototype)

#### <a name="apidoc.element.s3.AWS.XML.Parser.prototype.parse"></a>[function <span class="apidocSignatureSpan">s3.AWS.XML.Parser.prototype.</span>parse (xml, shape)](#apidoc.element.s3.AWS.XML.Parser.prototype.parse)
- description and source-code
```javascript
parse = function (xml, shape) {
  shape = shape || {};

  var result = null;
  var error = null;

  var parser = new xml2js.Parser(options);
  parser.parseString(xml, function (e, r) {
    error = e;
    result = r;
  });

  if (result) {
    var data = parseXml(result, shape);
    if (result.ResponseMetadata) {
      data.ResponseMetadata = parseXml(result.ResponseMetadata[0], {});
    }
    return data;
  } else if (error) {
    throw util.error(error, {code: 'XMLParserError'});
  } else { // empty xml document
    return parseXml({}, shape);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.util"></a>[module s3.AWS.util](#apidoc.module.s3.AWS.util)

#### <a name="apidoc.element.s3.AWS.util.Buffer"></a>[function <span class="apidocSignatureSpan">s3.AWS.util.</span>Buffer (arg, encodingOrOffset, length)](#apidoc.element.s3.AWS.util.Buffer)
- description and source-code
```javascript
function Buffer(arg, encodingOrOffset, length) {
  // Common case.
  if (typeof arg === 'number') {
    if (typeof encodingOrOffset === 'string') {
      throw new Error(
        'If encoding is specified then the first argument must be a string'
      );
    }
    return Buffer.allocUnsafe(arg);
  }
  return Buffer.from(arg, encodingOrOffset, length);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.util.arrayEach"></a>[function <span class="apidocSignatureSpan">s3.AWS.util.</span>arrayEach (array, iterFunction)](#apidoc.element.s3.AWS.util.arrayEach)
- description and source-code
```javascript
function arrayEach(array, iterFunction) {
  for (var idx in array) {
    if (array.hasOwnProperty(idx)) {
      var ret = iterFunction.call(this, array[idx], parseInt(idx, 10));
      if (ret === util.abort) break;
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.util.copy"></a>[function <span class="apidocSignatureSpan">s3.AWS.util.</span>copy (object)](#apidoc.element.s3.AWS.util.copy)
- description and source-code
```javascript
function copy(object) {
  if (object === null || object === undefined) return object;
  var dupe = {};
  // jshint forin:false
  for (var key in object) {
    dupe[key] = object[key];
  }
  return dupe;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.util.each"></a>[function <span class="apidocSignatureSpan">s3.AWS.util.</span>each (object, iterFunction)](#apidoc.element.s3.AWS.util.each)
- description and source-code
```javascript
function each(object, iterFunction) {
  for (var key in object) {
    if (object.hasOwnProperty(key)) {
      var ret = iterFunction.call(this, key, object[key]);
      if (ret === util.abort) break;
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.util.engine"></a>[function <span class="apidocSignatureSpan">s3.AWS.util.</span>engine ()](#apidoc.element.s3.AWS.util.engine)
- description and source-code
```javascript
function engine() {
  if (util.isBrowser() && typeof navigator !== 'undefined') {
    return navigator.userAgent;
  } else {
    return process.platform + '/' + process.version;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.util.error"></a>[function <span class="apidocSignatureSpan">s3.AWS.util.</span>error (err, options)](#apidoc.element.s3.AWS.util.error)
- description and source-code
```javascript
function error(err, options) {
  var originalError = null;
  if (typeof err.message === 'string' && err.message !== '') {
    if (typeof options === 'string' || (options && options.message)) {
      originalError = util.copy(err);
      originalError.message = err.message;
    }
  }
  err.message = err.message || null;

  if (typeof options === 'string') {
    err.message = options;
  } else {
    util.update(err, options);
  }

  if (typeof Object.defineProperty === 'function') {
    Object.defineProperty(err, 'name', {writable: true, enumerable: false});
    Object.defineProperty(err, 'message', {enumerable: true});
  }

  err.name = err.name || err.code || 'Error';
  err.time = new Date();

  if (originalError) err.originalError = originalError;

  return err;
}
```
- example usage
```shell
...
  Key: "some/remote/file",
  // other options supported by putObject, except Body and ContentLength.
  // See: http://docs.aws.amazon.com/AWSJavaScriptSDK/latest/AWS/S3.html#putObject-property
},
};
var uploader = client.uploadFile(params);
uploader.on('error', function(err) {
console.error("unable to upload:", err.stack);
});
uploader.on('progress', function() {
console.log("progress", uploader.progressMd5Amount,
          uploader.progressAmount, uploader.progressTotal);
});
uploader.on('end', function() {
console.log("done uploading");
...
```

#### <a name="apidoc.element.s3.AWS.util.hideProperties"></a>[function <span class="apidocSignatureSpan">s3.AWS.util.</span>hideProperties (obj, props)](#apidoc.element.s3.AWS.util.hideProperties)
- description and source-code
```javascript
function hideProperties(obj, props) {
  if (typeof Object.defineProperty !== 'function') return;

  util.arrayEach(props, function (key) {
    Object.defineProperty(obj, key, {
      enumerable: false, writable: true, configurable: true });
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.util.inherit"></a>[function <span class="apidocSignatureSpan">s3.AWS.util.</span>inherit (klass, features)](#apidoc.element.s3.AWS.util.inherit)
- description and source-code
```javascript
function inherit(klass, features) {
  var newObject = null;
  if (features === undefined) {
    features = klass;
    klass = Object;
    newObject = {};
  } else {
    var ctor = function ConstructorWrapper() {};
    ctor.prototype = klass.prototype;
    newObject = new ctor();
  }

  // constructor not supplied, create pass-through ctor
  if (features.constructor === Object) {
    features.constructor = function() {
      if (klass !== Object) {
        return klass.apply(this, arguments);
      }
    };
  }

  features.constructor.prototype = newObject;
  util.update(features.constructor.prototype, features);
  features.constructor.__super__ = klass;
  return features.constructor;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.util.isBrowser"></a>[function <span class="apidocSignatureSpan">s3.AWS.util.</span>isBrowser ()](#apidoc.element.s3.AWS.util.isBrowser)
- description and source-code
```javascript
function isBrowser() { return process && process.browser; }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.util.isEmpty"></a>[function <span class="apidocSignatureSpan">s3.AWS.util.</span>isEmpty (obj)](#apidoc.element.s3.AWS.util.isEmpty)
- description and source-code
```javascript
function isEmpty(obj) {
  for (var prop in obj) {
    if (obj.hasOwnProperty(prop)) {
      return false;
    }
  }
  return true;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.util.isNode"></a>[function <span class="apidocSignatureSpan">s3.AWS.util.</span>isNode ()](#apidoc.element.s3.AWS.util.isNode)
- description and source-code
```javascript
function isNode() { return !util.isBrowser(); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.util.isType"></a>[function <span class="apidocSignatureSpan">s3.AWS.util.</span>isType (obj, type)](#apidoc.element.s3.AWS.util.isType)
- description and source-code
```javascript
function isType(obj, type) {
  // handle cross-"frame" objects
  if (typeof type === 'function') type = util.typeName(type);
  return Object.prototype.toString.call(obj) === '[object ' + type + ']';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.util.memoizedProperty"></a>[function <span class="apidocSignatureSpan">s3.AWS.util.</span>memoizedProperty (obj, name, get, enumerable)](#apidoc.element.s3.AWS.util.memoizedProperty)
- description and source-code
```javascript
function memoizedProperty(obj, name, get, enumerable) {
  var cachedValue = null;

  // build enumerable attribute for each value with lazy accessor.
  util.property(obj, name, function() {
    if (cachedValue === null) {
      cachedValue = get();
    }
    return cachedValue;
  }, enumerable);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.util.merge"></a>[function <span class="apidocSignatureSpan">s3.AWS.util.</span>merge (obj1, obj2)](#apidoc.element.s3.AWS.util.merge)
- description and source-code
```javascript
function merge(obj1, obj2) {
  return util.update(util.copy(obj1), obj2);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.util.mixin"></a>[function <span class="apidocSignatureSpan">s3.AWS.util.</span>mixin ()](#apidoc.element.s3.AWS.util.mixin)
- description and source-code
```javascript
function mixin() {
  var klass = arguments[0];
  for (var i = 1; i < arguments.length; i++) {
    // jshint forin:false
    for (var prop in arguments[i].prototype) {
      var fn = arguments[i].prototype[prop];
      if (prop !== 'constructor') {
        klass.prototype[prop] = fn;
      }
    }
  }
  return klass;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.util.multiRequire"></a>[function <span class="apidocSignatureSpan">s3.AWS.util.</span>multiRequire (module1, module2)](#apidoc.element.s3.AWS.util.multiRequire)
- description and source-code
```javascript
function multiRequire(module1, module2) {
  return require(util.isNode() ? module1 : module2);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.util.nodeRequire"></a>[function <span class="apidocSignatureSpan">s3.AWS.util.</span>nodeRequire (module)](#apidoc.element.s3.AWS.util.nodeRequire)
- description and source-code
```javascript
function nodeRequire(module) {
  if (util.isNode()) return require(module);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.util.property"></a>[function <span class="apidocSignatureSpan">s3.AWS.util.</span>property (obj, name, value, enumerable, isValue)](#apidoc.element.s3.AWS.util.property)
- description and source-code
```javascript
function property(obj, name, value, enumerable, isValue) {
  var opts = {
    configurable: true,
    enumerable: enumerable !== undefined ? enumerable : true
  };
  if (typeof value === 'function' && !isValue) {
    opts.get = value;
  }
  else {
    opts.value = value; opts.writable = true;
  }

  Object.defineProperty(obj, name, opts);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.util.queryParamsToString"></a>[function <span class="apidocSignatureSpan">s3.AWS.util.</span>queryParamsToString (params)](#apidoc.element.s3.AWS.util.queryParamsToString)
- description and source-code
```javascript
function queryParamsToString(params) {
  var items = [];
  var escape = util.uriEscape;
  var sortedKeys = Object.keys(params).sort();

  util.arrayEach(sortedKeys, function(name) {
    var value = params[name];
    var ename = escape(name);
    var result = ename + '=';
    if (Array.isArray(value)) {
      var vals = [];
      util.arrayEach(value, function(item) { vals.push(escape(item)); });
      result = ename + '=' + vals.sort().join('&' + ename + '=');
    } else if (value !== undefined && value !== null) {
      result = ename + '=' + escape(value);
    }
    items.push(result);
  });

  return items.join('&');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.util.queryStringParse"></a>[function <span class="apidocSignatureSpan">s3.AWS.util.</span>queryStringParse (qs)](#apidoc.element.s3.AWS.util.queryStringParse)
- description and source-code
```javascript
function queryStringParse(qs) {
  return require('querystring').parse(qs);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.util.readFileSync"></a>[function <span class="apidocSignatureSpan">s3.AWS.util.</span>readFileSync (path)](#apidoc.element.s3.AWS.util.readFileSync)
- description and source-code
```javascript
function readFileSync(path) {
  if (typeof window !== 'undefined') return null;
  return util.nodeRequire('fs').readFileSync(path, 'utf-8');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.util.typeName"></a>[function <span class="apidocSignatureSpan">s3.AWS.util.</span>typeName (type)](#apidoc.element.s3.AWS.util.typeName)
- description and source-code
```javascript
function typeName(type) {
  if (type.hasOwnProperty('name')) return type.name;
  var str = type.toString();
  var match = str.match(/^\s*function (.+)\(/);
  return match ? match[1] : str;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.util.update"></a>[function <span class="apidocSignatureSpan">s3.AWS.util.</span>update (obj1, obj2)](#apidoc.element.s3.AWS.util.update)
- description and source-code
```javascript
function update(obj1, obj2) {
  util.each(obj2, function iterator(key, item) {
    obj1[key] = item;
  });
  return obj1;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.util.uriEscape"></a>[function <span class="apidocSignatureSpan">s3.AWS.util.</span>uriEscape (string)](#apidoc.element.s3.AWS.util.uriEscape)
- description and source-code
```javascript
function uriEscape(string) {
  var output = encodeURIComponent(string);
  output = output.replace(/[^A-Za-z0-9_.~\-%]+/g, escape);

  // AWS percent-encodes some extra non-standard characters in a URI
  output = output.replace(/[*]/g, function(ch) {
    return '%' + ch.charCodeAt(0).toString(16).toUpperCase();
  });

  return output;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.util.uriEscapePath"></a>[function <span class="apidocSignatureSpan">s3.AWS.util.</span>uriEscapePath (string)](#apidoc.element.s3.AWS.util.uriEscapePath)
- description and source-code
```javascript
function uriEscapePath(string) {
  var parts = [];
  util.arrayEach(string.split('/'), function (part) {
    parts.push(util.uriEscape(part));
  });
  return parts.join('/');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.util.urlFormat"></a>[function <span class="apidocSignatureSpan">s3.AWS.util.</span>urlFormat (url)](#apidoc.element.s3.AWS.util.urlFormat)
- description and source-code
```javascript
function urlFormat(url) {
  return require('url').format(url);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.util.urlParse"></a>[function <span class="apidocSignatureSpan">s3.AWS.util.</span>urlParse (url)](#apidoc.element.s3.AWS.util.urlParse)
- description and source-code
```javascript
function urlParse(url) {
  return require('url').parse(url);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.util.userAgent"></a>[function <span class="apidocSignatureSpan">s3.AWS.util.</span>userAgent ()](#apidoc.element.s3.AWS.util.userAgent)
- description and source-code
```javascript
function userAgent() {
  var name = util.isBrowser() ? 'js' : 'nodejs';
  var agent = 'aws-sdk-' + name + '/' + require('./core').VERSION;
  if (name === 'nodejs') agent += ' ' + util.engine();
  return agent;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.AWS.util.Buffer.prototype"></a>[module s3.AWS.util.Buffer.prototype](#apidoc.module.s3.AWS.util.Buffer.prototype)

#### <a name="apidoc.element.s3.AWS.util.Buffer.prototype.asciiSlice"></a>[function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>asciiSlice ()](#apidoc.element.s3.AWS.util.Buffer.prototype.asciiSlice)
- description and source-code
```javascript
function asciiSlice() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.util.Buffer.prototype.asciiWrite"></a>[function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>asciiWrite ()](#apidoc.element.s3.AWS.util.Buffer.prototype.asciiWrite)
- description and source-code
```javascript
function asciiWrite() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.util.Buffer.prototype.base64Slice"></a>[function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>base64Slice ()](#apidoc.element.s3.AWS.util.Buffer.prototype.base64Slice)
- description and source-code
```javascript
function base64Slice() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.util.Buffer.prototype.base64Write"></a>[function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>base64Write ()](#apidoc.element.s3.AWS.util.Buffer.prototype.base64Write)
- description and source-code
```javascript
function base64Write() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.util.Buffer.prototype.compare"></a>[function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>compare (target, start, end, thisStart, thisEnd)](#apidoc.element.s3.AWS.util.Buffer.prototype.compare)
- description and source-code
```javascript
function compare(target, start, end, thisStart, thisEnd) {

  if (!(target instanceof Buffer))
    throw new TypeError('Argument must be a Buffer');
  if (arguments.length === 1)
    return compare_(this, target);

  if (start === undefined)
    start = 0;
  else if (start < 0)
    throw new RangeError('out of range index');
  else
    start >>>= 0;

  if (end === undefined)
    end = target.length;
  else if (end > target.length)
    throw new RangeError('out of range index');
  else
    end >>>= 0;

  if (thisStart === undefined)
    thisStart = 0;
  else if (thisStart < 0)
    throw new RangeError('out of range index');
  else
    thisStart >>>= 0;

  if (thisEnd === undefined)
    thisEnd = this.length;
  else if (thisEnd > this.length)
    throw new RangeError('out of range index');
  else
    thisEnd >>>= 0;

  if (thisStart >= thisEnd)
    return (start >= end ? 0 : -1);
  else if (start >= end)
    return 1;

  return compareOffset(this, target, start, thisStart, end, thisEnd);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.util.Buffer.prototype.copy"></a>[function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>copy ()](#apidoc.element.s3.AWS.util.Buffer.prototype.copy)
- description and source-code
```javascript
function copy() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.util.Buffer.prototype.equals"></a>[function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>equals (b)](#apidoc.element.s3.AWS.util.Buffer.prototype.equals)
- description and source-code
```javascript
function equals(b) {
  if (!(b instanceof Buffer))
    throw new TypeError('Argument must be a Buffer');

  if (this === b)
    return true;

  return binding.compare(this, b) === 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.util.Buffer.prototype.fill"></a>[function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>fill (val, start, end, encoding)](#apidoc.element.s3.AWS.util.Buffer.prototype.fill)
- description and source-code
```javascript
function fill(val, start, end, encoding) {
  // Handle string cases:
  if (typeof val === 'string') {
    if (typeof start === 'string') {
      encoding = start;
      start = 0;
      end = this.length;
    } else if (typeof end === 'string') {
      encoding = end;
      end = this.length;
    }

    if (encoding !== undefined && typeof encoding !== 'string') {
      throw new TypeError('encoding must be a string');
    }
    var normalizedEncoding = internalUtil.normalizeEncoding(encoding);
    if (normalizedEncoding === undefined) {
      throw new TypeError('Unknown encoding: ' + encoding);
    }

    if (val.length === 0) {
      // Previously, if val === '', the Buffer would not fill,
      // which is rather surprising.
      val = 0;
    } else if (val.length === 1) {
      var code = val.charCodeAt(0);
      if ((normalizedEncoding === 'utf8' && code < 128) ||
          normalizedEncoding === 'latin1') {
        // Fast path: If 'val' fits into a single byte, use that numeric value.
        val = code;
      }
    }
  } else if (typeof val === 'number') {
    val = val & 255;
  }

  // Invalid ranges are not set to a default, so can range check early.
  if (start < 0 || end > this.length)
    throw new RangeError('Out of range index');

  if (end <= start)
    return this;

  start = start >>> 0;
  end = end === undefined ? this.length : end >>> 0;

  binding.fill(this, val, start, end, encoding);

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.util.Buffer.prototype.hexSlice"></a>[function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>hexSlice ()](#apidoc.element.s3.AWS.util.Buffer.prototype.hexSlice)
- description and source-code
```javascript
function hexSlice() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.util.Buffer.prototype.hexWrite"></a>[function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>hexWrite ()](#apidoc.element.s3.AWS.util.Buffer.prototype.hexWrite)
- description and source-code
```javascript
function hexWrite() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.util.Buffer.prototype.includes"></a>[function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>includes (val, byteOffset, encoding)](#apidoc.element.s3.AWS.util.Buffer.prototype.includes)
- description and source-code
```javascript
function includes(val, byteOffset, encoding) {
  return this.indexOf(val, byteOffset, encoding) !== -1;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.util.Buffer.prototype.indexOf"></a>[function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>indexOf (val, byteOffset, encoding)](#apidoc.element.s3.AWS.util.Buffer.prototype.indexOf)
- description and source-code
```javascript
function indexOf(val, byteOffset, encoding) {
  return bidirectionalIndexOf(this, val, byteOffset, encoding, true);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.util.Buffer.prototype.inspect"></a>[function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>inspect ()](#apidoc.element.s3.AWS.util.Buffer.prototype.inspect)
- description and source-code
```javascript
function inspect() {
  var str = '';
  var max = exports.INSPECT_MAX_BYTES;
  if (this.length > 0) {
    str = this.toString('hex', 0, max).match(/.{2}/g).join(' ');
    if (this.length > max)
      str += ' ... ';
  }
  return '<' + this.constructor.name + ' ' + str + '>';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.util.Buffer.prototype.lastIndexOf"></a>[function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>lastIndexOf (val, byteOffset, encoding)](#apidoc.element.s3.AWS.util.Buffer.prototype.lastIndexOf)
- description and source-code
```javascript
function lastIndexOf(val, byteOffset, encoding) {
  return bidirectionalIndexOf(this, val, byteOffset, encoding, false);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.util.Buffer.prototype.latin1Slice"></a>[function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>latin1Slice ()](#apidoc.element.s3.AWS.util.Buffer.prototype.latin1Slice)
- description and source-code
```javascript
function latin1Slice() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.util.Buffer.prototype.latin1Write"></a>[function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>latin1Write ()](#apidoc.element.s3.AWS.util.Buffer.prototype.latin1Write)
- description and source-code
```javascript
function latin1Write() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.util.Buffer.prototype.readDoubleBE"></a>[function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>readDoubleBE (offset, noAssert)](#apidoc.element.s3.AWS.util.Buffer.prototype.readDoubleBE)
- description and source-code
```javascript
function readDoubleBE(offset, noAssert) {
  offset = offset >>> 0;
  if (!noAssert)
    checkOffset(offset, 8, this.length);
  return binding.readDoubleBE(this, offset);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.util.Buffer.prototype.readDoubleLE"></a>[function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>readDoubleLE (offset, noAssert)](#apidoc.element.s3.AWS.util.Buffer.prototype.readDoubleLE)
- description and source-code
```javascript
function readDoubleLE(offset, noAssert) {
  offset = offset >>> 0;
  if (!noAssert)
    checkOffset(offset, 8, this.length);
  return binding.readDoubleLE(this, offset);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.util.Buffer.prototype.readFloatBE"></a>[function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>readFloatBE (offset, noAssert)](#apidoc.element.s3.AWS.util.Buffer.prototype.readFloatBE)
- description and source-code
```javascript
function readFloatBE(offset, noAssert) {
  offset = offset >>> 0;
  if (!noAssert)
    checkOffset(offset, 4, this.length);
  return binding.readFloatBE(this, offset);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.util.Buffer.prototype.readFloatLE"></a>[function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>readFloatLE (offset, noAssert)](#apidoc.element.s3.AWS.util.Buffer.prototype.readFloatLE)
- description and source-code
```javascript
function readFloatLE(offset, noAssert) {
  offset = offset >>> 0;
  if (!noAssert)
    checkOffset(offset, 4, this.length);
  return binding.readFloatLE(this, offset);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.util.Buffer.prototype.readInt16BE"></a>[function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>readInt16BE (offset, noAssert)](#apidoc.element.s3.AWS.util.Buffer.prototype.readInt16BE)
- description and source-code
```javascript
readInt16BE = function (offset, noAssert) {
  offset = offset >>> 0;
  if (!noAssert)
    checkOffset(offset, 2, this.length);
  var val = this[offset + 1] | (this[offset] << 8);
  return (val & 0x8000) ? val | 0xFFFF0000 : val;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.util.Buffer.prototype.readInt16LE"></a>[function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>readInt16LE (offset, noAssert)](#apidoc.element.s3.AWS.util.Buffer.prototype.readInt16LE)
- description and source-code
```javascript
readInt16LE = function (offset, noAssert) {
  offset = offset >>> 0;
  if (!noAssert)
    checkOffset(offset, 2, this.length);
  var val = this[offset] | (this[offset + 1] << 8);
  return (val & 0x8000) ? val | 0xFFFF0000 : val;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.util.Buffer.prototype.readInt32BE"></a>[function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>readInt32BE (offset, noAssert)](#apidoc.element.s3.AWS.util.Buffer.prototype.readInt32BE)
- description and source-code
```javascript
readInt32BE = function (offset, noAssert) {
  offset = offset >>> 0;
  if (!noAssert)
    checkOffset(offset, 4, this.length);

  return (this[offset] << 24) |
      (this[offset + 1] << 16) |
      (this[offset + 2] << 8) |
      (this[offset + 3]);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.util.Buffer.prototype.readInt32LE"></a>[function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>readInt32LE (offset, noAssert)](#apidoc.element.s3.AWS.util.Buffer.prototype.readInt32LE)
- description and source-code
```javascript
readInt32LE = function (offset, noAssert) {
  offset = offset >>> 0;
  if (!noAssert)
    checkOffset(offset, 4, this.length);

  return (this[offset]) |
      (this[offset + 1] << 8) |
      (this[offset + 2] << 16) |
      (this[offset + 3] << 24);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.util.Buffer.prototype.readInt8"></a>[function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>readInt8 (offset, noAssert)](#apidoc.element.s3.AWS.util.Buffer.prototype.readInt8)
- description and source-code
```javascript
readInt8 = function (offset, noAssert) {
  offset = offset >>> 0;
  if (!noAssert)
    checkOffset(offset, 1, this.length);
  var val = this[offset];
  return !(val & 0x80) ? val : (0xff - val + 1) * -1;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.util.Buffer.prototype.readIntBE"></a>[function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>readIntBE (offset, byteLength, noAssert)](#apidoc.element.s3.AWS.util.Buffer.prototype.readIntBE)
- description and source-code
```javascript
readIntBE = function (offset, byteLength, noAssert) {
  offset = offset >>> 0;
  byteLength = byteLength >>> 0;
  if (!noAssert)
    checkOffset(offset, byteLength, this.length);

  var i = byteLength;
  var mul = 1;
  var val = this[offset + --i];
  while (i > 0 && (mul *= 0x100))
    val += this[offset + --i] * mul;
  mul *= 0x80;

  if (val >= mul)
    val -= Math.pow(2, 8 * byteLength);

  return val;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.util.Buffer.prototype.readIntLE"></a>[function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>readIntLE (offset, byteLength, noAssert)](#apidoc.element.s3.AWS.util.Buffer.prototype.readIntLE)
- description and source-code
```javascript
readIntLE = function (offset, byteLength, noAssert) {
  offset = offset >>> 0;
  byteLength = byteLength >>> 0;
  if (!noAssert)
    checkOffset(offset, byteLength, this.length);

  var val = this[offset];
  var mul = 1;
  var i = 0;
  while (++i < byteLength && (mul *= 0x100))
    val += this[offset + i] * mul;
  mul *= 0x80;

  if (val >= mul)
    val -= Math.pow(2, 8 * byteLength);

  return val;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.util.Buffer.prototype.readUInt16BE"></a>[function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>readUInt16BE (offset, noAssert)](#apidoc.element.s3.AWS.util.Buffer.prototype.readUInt16BE)
- description and source-code
```javascript
readUInt16BE = function (offset, noAssert) {
  offset = offset >>> 0;
  if (!noAssert)
    checkOffset(offset, 2, this.length);
  return (this[offset] << 8) | this[offset + 1];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.util.Buffer.prototype.readUInt16LE"></a>[function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>readUInt16LE (offset, noAssert)](#apidoc.element.s3.AWS.util.Buffer.prototype.readUInt16LE)
- description and source-code
```javascript
readUInt16LE = function (offset, noAssert) {
  offset = offset >>> 0;
  if (!noAssert)
    checkOffset(offset, 2, this.length);
  return this[offset] | (this[offset + 1] << 8);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.util.Buffer.prototype.readUInt32BE"></a>[function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>readUInt32BE (offset, noAssert)](#apidoc.element.s3.AWS.util.Buffer.prototype.readUInt32BE)
- description and source-code
```javascript
readUInt32BE = function (offset, noAssert) {
  offset = offset >>> 0;
  if (!noAssert)
    checkOffset(offset, 4, this.length);

  return (this[offset] * 0x1000000) +
      ((this[offset + 1] << 16) |
      (this[offset + 2] << 8) |
      this[offset + 3]);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.util.Buffer.prototype.readUInt32LE"></a>[function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>readUInt32LE (offset, noAssert)](#apidoc.element.s3.AWS.util.Buffer.prototype.readUInt32LE)
- description and source-code
```javascript
readUInt32LE = function (offset, noAssert) {
  offset = offset >>> 0;
  if (!noAssert)
    checkOffset(offset, 4, this.length);

  return ((this[offset]) |
      (this[offset + 1] << 8) |
      (this[offset + 2] << 16)) +
      (this[offset + 3] * 0x1000000);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.util.Buffer.prototype.readUInt8"></a>[function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>readUInt8 (offset, noAssert)](#apidoc.element.s3.AWS.util.Buffer.prototype.readUInt8)
- description and source-code
```javascript
readUInt8 = function (offset, noAssert) {
  offset = offset >>> 0;
  if (!noAssert)
    checkOffset(offset, 1, this.length);
  return this[offset];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.util.Buffer.prototype.readUIntBE"></a>[function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>readUIntBE (offset, byteLength, noAssert)](#apidoc.element.s3.AWS.util.Buffer.prototype.readUIntBE)
- description and source-code
```javascript
readUIntBE = function (offset, byteLength, noAssert) {
  offset = offset >>> 0;
  byteLength = byteLength >>> 0;
  if (!noAssert)
    checkOffset(offset, byteLength, this.length);

  var val = this[offset + --byteLength];
  var mul = 1;
  while (byteLength > 0 && (mul *= 0x100))
    val += this[offset + --byteLength] * mul;

  return val;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.util.Buffer.prototype.readUIntLE"></a>[function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>readUIntLE (offset, byteLength, noAssert)](#apidoc.element.s3.AWS.util.Buffer.prototype.readUIntLE)
- description and source-code
```javascript
readUIntLE = function (offset, byteLength, noAssert) {
  offset = offset >>> 0;
  byteLength = byteLength >>> 0;
  if (!noAssert)
    checkOffset(offset, byteLength, this.length);

  var val = this[offset];
  var mul = 1;
  var i = 0;
  while (++i < byteLength && (mul *= 0x100))
    val += this[offset + i] * mul;

  return val;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.util.Buffer.prototype.slice"></a>[function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>slice (start, end)](#apidoc.element.s3.AWS.util.Buffer.prototype.slice)
- description and source-code
```javascript
function slice(start, end) {
  const srcLength = this.length;
  start = adjustOffset(start, srcLength);
  end = end !== undefined ? adjustOffset(end, srcLength) : srcLength;
  const newLength = end > start ? end - start : 0;
  return new FastBuffer(this.buffer, this.byteOffset + start, newLength);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.util.Buffer.prototype.swap16"></a>[function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>swap16 ()](#apidoc.element.s3.AWS.util.Buffer.prototype.swap16)
- description and source-code
```javascript
function swap16() {
  // For Buffer.length < 128, it's generally faster to
  // do the swap in javascript. For larger buffers,
  // dropping down to the native code is faster.
  const len = this.length;
  if (len % 2 !== 0)
    throw new RangeError('Buffer size must be a multiple of 16-bits');
  if (len < 128) {
    for (var i = 0; i < len; i += 2)
      swap(this, i, i + 1);
    return this;
  }
  return swap16n(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.util.Buffer.prototype.swap32"></a>[function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>swap32 ()](#apidoc.element.s3.AWS.util.Buffer.prototype.swap32)
- description and source-code
```javascript
function swap32() {
  // For Buffer.length < 192, it's generally faster to
  // do the swap in javascript. For larger buffers,
  // dropping down to the native code is faster.
  const len = this.length;
  if (len % 4 !== 0)
    throw new RangeError('Buffer size must be a multiple of 32-bits');
  if (len < 192) {
    for (var i = 0; i < len; i += 4) {
      swap(this, i, i + 3);
      swap(this, i + 1, i + 2);
    }
    return this;
  }
  return swap32n(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.util.Buffer.prototype.swap64"></a>[function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>swap64 ()](#apidoc.element.s3.AWS.util.Buffer.prototype.swap64)
- description and source-code
```javascript
function swap64() {
  // For Buffer.length < 192, it's generally faster to
  // do the swap in javascript. For larger buffers,
  // dropping down to the native code is faster.
  const len = this.length;
  if (len % 8 !== 0)
    throw new RangeError('Buffer size must be a multiple of 64-bits');
  if (len < 192) {
    for (var i = 0; i < len; i += 8) {
      swap(this, i, i + 7);
      swap(this, i + 1, i + 6);
      swap(this, i + 2, i + 5);
      swap(this, i + 3, i + 4);
    }
    return this;
  }
  return swap64n(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.util.Buffer.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>toJSON ()](#apidoc.element.s3.AWS.util.Buffer.prototype.toJSON)
- description and source-code
```javascript
toJSON = function () {
  if (this.length) {
    const data = [];
    for (var i = 0; i < this.length; ++i)
      data[i] = this[i];
    return { type: 'Buffer', data };
  } else {
    return { type: 'Buffer', data: [] };
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.util.Buffer.prototype.toString"></a>[function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>toString ()](#apidoc.element.s3.AWS.util.Buffer.prototype.toString)
- description and source-code
```javascript
toString = function () {
  let result;
  if (arguments.length === 0) {
    result = this.utf8Slice(0, this.length);
  } else {
    result = slowToString.apply(this, arguments);
  }
  if (result === undefined)
    throw new Error('"toString()" failed');
  return result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.util.Buffer.prototype.ucs2Slice"></a>[function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>ucs2Slice ()](#apidoc.element.s3.AWS.util.Buffer.prototype.ucs2Slice)
- description and source-code
```javascript
function ucs2Slice() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.util.Buffer.prototype.ucs2Write"></a>[function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>ucs2Write ()](#apidoc.element.s3.AWS.util.Buffer.prototype.ucs2Write)
- description and source-code
```javascript
function ucs2Write() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.util.Buffer.prototype.utf8Slice"></a>[function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>utf8Slice ()](#apidoc.element.s3.AWS.util.Buffer.prototype.utf8Slice)
- description and source-code
```javascript
function utf8Slice() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.util.Buffer.prototype.utf8Write"></a>[function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>utf8Write ()](#apidoc.element.s3.AWS.util.Buffer.prototype.utf8Write)
- description and source-code
```javascript
function utf8Write() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.util.Buffer.prototype.write"></a>[function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>write (string, offset, length, encoding)](#apidoc.element.s3.AWS.util.Buffer.prototype.write)
- description and source-code
```javascript
write = function (string, offset, length, encoding) {
  // Buffer#write(string);
  if (offset === undefined) {
    encoding = 'utf8';
    length = this.length;
    offset = 0;

  // Buffer#write(string, encoding)
  } else if (length === undefined && typeof offset === 'string') {
    encoding = offset;
    length = this.length;
    offset = 0;

  // Buffer#write(string, offset[, length][, encoding])
  } else if (isFinite(offset)) {
    offset = offset >>> 0;
    if (isFinite(length)) {
      length = length >>> 0;
      if (encoding === undefined)
        encoding = 'utf8';
    } else {
      encoding = length;
      length = undefined;
    }
  } else {
    // if someone is still calling the obsolete form of write(), tell them.
    // we don't want eg buf.write("foo", "utf8", 10) to silently turn into
    // buf.write("foo", "utf8"), so we can't ignore extra args
    throw new Error('Buffer.write(string, encoding, offset[, length]) ' +
                    'is no longer supported');
  }

  var remaining = this.length - offset;
  if (length === undefined || length > remaining)
    length = remaining;

  if (string.length > 0 && (length < 0 || offset < 0))
    throw new RangeError('Attempt to write outside buffer bounds');

  if (!encoding)
    encoding = 'utf8';

  var loweredCase = false;
  for (;;) {
    switch (encoding) {
      case 'hex':
        return this.hexWrite(string, offset, length);

      case 'utf8':
      case 'utf-8':
        return this.utf8Write(string, offset, length);

      case 'ascii':
        return this.asciiWrite(string, offset, length);

      case 'latin1':
      case 'binary':
        return this.latin1Write(string, offset, length);

      case 'base64':
        // Warning: maxLength not taken into account in base64Write
        return this.base64Write(string, offset, length);

      case 'ucs2':
      case 'ucs-2':
      case 'utf16le':
      case 'utf-16le':
        return this.ucs2Write(string, offset, length);

      default:
        if (loweredCase)
          throw new TypeError('Unknown encoding: ' + encoding);
        encoding = ('' + encoding).toLowerCase();
        loweredCase = true;
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.util.Buffer.prototype.writeDoubleBE"></a>[function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>writeDoubleBE (val, offset, noAssert)](#apidoc.element.s3.AWS.util.Buffer.prototype.writeDoubleBE)
- description and source-code
```javascript
function writeDoubleBE(val, offset, noAssert) {
  val = +val;
  offset = offset >>> 0;
  if (!noAssert)
    binding.writeDoubleBE(this, val, offset);
  else
    binding.writeDoubleBE(this, val, offset, true);
  return offset + 8;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.util.Buffer.prototype.writeDoubleLE"></a>[function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>writeDoubleLE (val, offset, noAssert)](#apidoc.element.s3.AWS.util.Buffer.prototype.writeDoubleLE)
- description and source-code
```javascript
function writeDoubleLE(val, offset, noAssert) {
  val = +val;
  offset = offset >>> 0;
  if (!noAssert)
    binding.writeDoubleLE(this, val, offset);
  else
    binding.writeDoubleLE(this, val, offset, true);
  return offset + 8;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.util.Buffer.prototype.writeFloatBE"></a>[function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>writeFloatBE (val, offset, noAssert)](#apidoc.element.s3.AWS.util.Buffer.prototype.writeFloatBE)
- description and source-code
```javascript
function writeFloatBE(val, offset, noAssert) {
  val = +val;
  offset = offset >>> 0;
  if (!noAssert)
    binding.writeFloatBE(this, val, offset);
  else
    binding.writeFloatBE(this, val, offset, true);
  return offset + 4;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.util.Buffer.prototype.writeFloatLE"></a>[function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>writeFloatLE (val, offset, noAssert)](#apidoc.element.s3.AWS.util.Buffer.prototype.writeFloatLE)
- description and source-code
```javascript
function writeFloatLE(val, offset, noAssert) {
  val = +val;
  offset = offset >>> 0;
  if (!noAssert)
    binding.writeFloatLE(this, val, offset);
  else
    binding.writeFloatLE(this, val, offset, true);
  return offset + 4;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.util.Buffer.prototype.writeInt16BE"></a>[function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>writeInt16BE (value, offset, noAssert)](#apidoc.element.s3.AWS.util.Buffer.prototype.writeInt16BE)
- description and source-code
```javascript
writeInt16BE = function (value, offset, noAssert) {
  value = +value;
  offset = offset >>> 0;
  if (!noAssert)
    checkInt(this, value, offset, 2, 0x7fff, -0x8000);
  this[offset] = (value >>> 8);
  this[offset + 1] = value;
  return offset + 2;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.util.Buffer.prototype.writeInt16LE"></a>[function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>writeInt16LE (value, offset, noAssert)](#apidoc.element.s3.AWS.util.Buffer.prototype.writeInt16LE)
- description and source-code
```javascript
writeInt16LE = function (value, offset, noAssert) {
  value = +value;
  offset = offset >>> 0;
  if (!noAssert)
    checkInt(this, value, offset, 2, 0x7fff, -0x8000);
  this[offset] = value;
  this[offset + 1] = (value >>> 8);
  return offset + 2;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.util.Buffer.prototype.writeInt32BE"></a>[function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>writeInt32BE (value, offset, noAssert)](#apidoc.element.s3.AWS.util.Buffer.prototype.writeInt32BE)
- description and source-code
```javascript
writeInt32BE = function (value, offset, noAssert) {
  value = +value;
  offset = offset >>> 0;
  if (!noAssert)
    checkInt(this, value, offset, 4, 0x7fffffff, -0x80000000);
  this[offset] = (value >>> 24);
  this[offset + 1] = (value >>> 16);
  this[offset + 2] = (value >>> 8);
  this[offset + 3] = value;
  return offset + 4;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.util.Buffer.prototype.writeInt32LE"></a>[function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>writeInt32LE (value, offset, noAssert)](#apidoc.element.s3.AWS.util.Buffer.prototype.writeInt32LE)
- description and source-code
```javascript
writeInt32LE = function (value, offset, noAssert) {
  value = +value;
  offset = offset >>> 0;
  if (!noAssert)
    checkInt(this, value, offset, 4, 0x7fffffff, -0x80000000);
  this[offset] = value;
  this[offset + 1] = (value >>> 8);
  this[offset + 2] = (value >>> 16);
  this[offset + 3] = (value >>> 24);
  return offset + 4;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.util.Buffer.prototype.writeInt8"></a>[function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>writeInt8 (value, offset, noAssert)](#apidoc.element.s3.AWS.util.Buffer.prototype.writeInt8)
- description and source-code
```javascript
writeInt8 = function (value, offset, noAssert) {
  value = +value;
  offset = offset >>> 0;
  if (!noAssert)
    checkInt(this, value, offset, 1, 0x7f, -0x80);
  this[offset] = value;
  return offset + 1;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.util.Buffer.prototype.writeIntBE"></a>[function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>writeIntBE (value, offset, byteLength, noAssert)](#apidoc.element.s3.AWS.util.Buffer.prototype.writeIntBE)
- description and source-code
```javascript
writeIntBE = function (value, offset, byteLength, noAssert) {
  value = +value;
  offset = offset >>> 0;
  if (!noAssert) {
    checkInt(this,
             value,
             offset,
             byteLength,
             Math.pow(2, 8 * byteLength - 1) - 1,
             -Math.pow(2, 8 * byteLength - 1));
  }

  var i = byteLength - 1;
  var mul = 1;
  var sub = 0;
  this[offset + i] = value;
  while (--i >= 0 && (mul *= 0x100)) {
    if (value < 0 && sub === 0 && this[offset + i + 1] !== 0)
      sub = 1;
    this[offset + i] = ((value / mul) >> 0) - sub;
  }

  return offset + byteLength;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.util.Buffer.prototype.writeIntLE"></a>[function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>writeIntLE (value, offset, byteLength, noAssert)](#apidoc.element.s3.AWS.util.Buffer.prototype.writeIntLE)
- description and source-code
```javascript
writeIntLE = function (value, offset, byteLength, noAssert) {
  value = +value;
  offset = offset >>> 0;
  if (!noAssert) {
    checkInt(this,
             value,
             offset,
             byteLength,
             Math.pow(2, 8 * byteLength - 1) - 1,
             -Math.pow(2, 8 * byteLength - 1));
  }

  var i = 0;
  var mul = 1;
  var sub = 0;
  this[offset] = value;
  while (++i < byteLength && (mul *= 0x100)) {
    if (value < 0 && sub === 0 && this[offset + i - 1] !== 0)
      sub = 1;
    this[offset + i] = ((value / mul) >> 0) - sub;
  }

  return offset + byteLength;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.util.Buffer.prototype.writeUInt16BE"></a>[function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>writeUInt16BE (value, offset, noAssert)](#apidoc.element.s3.AWS.util.Buffer.prototype.writeUInt16BE)
- description and source-code
```javascript
writeUInt16BE = function (value, offset, noAssert) {
  value = +value;
  offset = offset >>> 0;
  if (!noAssert)
    checkInt(this, value, offset, 2, 0xffff, 0);
  this[offset] = (value >>> 8);
  this[offset + 1] = value;
  return offset + 2;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.util.Buffer.prototype.writeUInt16LE"></a>[function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>writeUInt16LE (value, offset, noAssert)](#apidoc.element.s3.AWS.util.Buffer.prototype.writeUInt16LE)
- description and source-code
```javascript
writeUInt16LE = function (value, offset, noAssert) {
  value = +value;
  offset = offset >>> 0;
  if (!noAssert)
    checkInt(this, value, offset, 2, 0xffff, 0);
  this[offset] = value;
  this[offset + 1] = (value >>> 8);
  return offset + 2;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.util.Buffer.prototype.writeUInt32BE"></a>[function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>writeUInt32BE (value, offset, noAssert)](#apidoc.element.s3.AWS.util.Buffer.prototype.writeUInt32BE)
- description and source-code
```javascript
writeUInt32BE = function (value, offset, noAssert) {
  value = +value;
  offset = offset >>> 0;
  if (!noAssert)
    checkInt(this, value, offset, 4, 0xffffffff, 0);
  this[offset] = (value >>> 24);
  this[offset + 1] = (value >>> 16);
  this[offset + 2] = (value >>> 8);
  this[offset + 3] = value;
  return offset + 4;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.util.Buffer.prototype.writeUInt32LE"></a>[function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>writeUInt32LE (value, offset, noAssert)](#apidoc.element.s3.AWS.util.Buffer.prototype.writeUInt32LE)
- description and source-code
```javascript
writeUInt32LE = function (value, offset, noAssert) {
  value = +value;
  offset = offset >>> 0;
  if (!noAssert)
    checkInt(this, value, offset, 4, 0xffffffff, 0);
  this[offset + 3] = (value >>> 24);
  this[offset + 2] = (value >>> 16);
  this[offset + 1] = (value >>> 8);
  this[offset] = value;
  return offset + 4;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.util.Buffer.prototype.writeUInt8"></a>[function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>writeUInt8 (value, offset, noAssert)](#apidoc.element.s3.AWS.util.Buffer.prototype.writeUInt8)
- description and source-code
```javascript
writeUInt8 = function (value, offset, noAssert) {
  value = +value;
  offset = offset >>> 0;
  if (!noAssert)
    checkInt(this, value, offset, 1, 0xff, 0);
  this[offset] = value;
  return offset + 1;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.util.Buffer.prototype.writeUIntBE"></a>[function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>writeUIntBE (value, offset, byteLength, noAssert)](#apidoc.element.s3.AWS.util.Buffer.prototype.writeUIntBE)
- description and source-code
```javascript
writeUIntBE = function (value, offset, byteLength, noAssert) {
  value = +value;
  offset = offset >>> 0;
  byteLength = byteLength >>> 0;
  if (!noAssert) {
    const maxBytes = Math.pow(2, 8 * byteLength) - 1;
    checkInt(this, value, offset, byteLength, maxBytes, 0);
  }

  var i = byteLength - 1;
  var mul = 1;
  this[offset + i] = value;
  while (--i >= 0 && (mul *= 0x100))
    this[offset + i] = (value / mul) >>> 0;

  return offset + byteLength;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.AWS.util.Buffer.prototype.writeUIntLE"></a>[function <span class="apidocSignatureSpan">s3.AWS.util.Buffer.prototype.</span>writeUIntLE (value, offset, byteLength, noAssert)](#apidoc.element.s3.AWS.util.Buffer.prototype.writeUIntLE)
- description and source-code
```javascript
writeUIntLE = function (value, offset, byteLength, noAssert) {
  value = +value;
  offset = offset >>> 0;
  byteLength = byteLength >>> 0;
  if (!noAssert) {
    const maxBytes = Math.pow(2, 8 * byteLength) - 1;
    checkInt(this, value, offset, byteLength, maxBytes, 0);
  }

  var mul = 1;
  var i = 0;
  this[offset] = value;
  while (++i < byteLength && (mul *= 0x100))
    this[offset + i] = (value / mul) >>> 0;

  return offset + byteLength;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.Client"></a>[module s3.Client](#apidoc.module.s3.Client)

#### <a name="apidoc.element.s3.Client.Client"></a>[function <span class="apidocSignatureSpan">s3.</span>Client (options)](#apidoc.element.s3.Client.Client)
- description and source-code
```javascript
function Client(options) {
  options = options || {};
  this.s3 = options.s3Client || new AWS.S3(options.s3Options);
  this.s3Pend = new Pend();
  this.s3Pend.max = options.maxAsyncS3 || 20;
  this.s3RetryCount = options.s3RetryCount || 3;
  this.s3RetryDelay = options.s3RetryDelay || 1000;
  this.multipartUploadThreshold = options.multipartUploadThreshold || (20 * 1024 * 1024);
  this.multipartUploadSize = options.multipartUploadSize || (15 * 1024 * 1024);
  this.multipartDownloadThreshold = options.multipartDownloadThreshold || (20 * 1024 * 1024);
  this.multipartDownloadSize = options.multipartDownloadSize || (15 * 1024 * 1024);

  if (this.multipartUploadThreshold < MIN_MULTIPART_SIZE) {
    throw new Error("Minimum multipartUploadThreshold is 5MB.");
  }
  if (this.multipartUploadThreshold > MAX_PUTOBJECT_SIZE) {
    throw new Error("Maximum multipartUploadThreshold is 5GB.");
  }
  if (this.multipartUploadSize < MIN_MULTIPART_SIZE) {
    throw new Error("Minimum multipartUploadSize is 5MB.");
  }
  if (this.multipartUploadSize > MAX_PUTOBJECT_SIZE) {
    throw new Error("Maximum multipartUploadSize is 5GB.");
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.Client.prototype"></a>[module s3.Client.prototype](#apidoc.module.s3.Client.prototype)

#### <a name="apidoc.element.s3.Client.prototype.copyObject"></a>[function <span class="apidocSignatureSpan">s3.Client.prototype.</span>copyObject (_s3Params)](#apidoc.element.s3.Client.prototype.copyObject)
- description and source-code
```javascript
copyObject = function (_s3Params) {
  var self = this;
  var ee = new EventEmitter();
  var s3Params = extend({}, _s3Params);
  delete s3Params.MFA;
  doWithRetry(doCopyWithPend, self.s3RetryCount, self.s3RetryDelay, function(err, data) {
    if (err) {
      ee.emit('error', err);
    } else {
      ee.emit('end', data);
    }
  });
  function doCopyWithPend(cb) {
    self.s3Pend.go(function(pendCb) {
      doTheCopy(function(err, data) {
        pendCb();
        cb(err, data);
      });
    });
  }
  function doTheCopy(cb) {
    self.s3.copyObject(s3Params, cb);
  }
  return ee;
}
```
- example usage
```shell
...
'deleteDir' works like this:

 0. Start listing all objects in a bucket recursively. S3 returns 1000 objects
    per response.
 0. For each response that comes back with a list of objects in the bucket,
    immediately send a delete request for all of them.

### client.copyObject(s3Params)

See http://docs.aws.amazon.com/AWSJavaScriptSDK/latest/AWS/S3.html#copyObject-property

's3Params' are the same. Don't forget that 'CopySource' must contain the
source bucket name as well as the source key name.

The difference between using AWS SDK 'copyObject' and this one:
...
```

#### <a name="apidoc.element.s3.Client.prototype.deleteDir"></a>[function <span class="apidocSignatureSpan">s3.Client.prototype.</span>deleteDir (s3Params)](#apidoc.element.s3.Client.prototype.deleteDir)
- description and source-code
```javascript
deleteDir = function (s3Params) {
  var self = this;
  var ee = new EventEmitter();
  var bucket = s3Params.Bucket;
  var mfa = s3Params.MFA;
  var listObjectsParams = {
    recursive: true,
    s3Params: {
      Bucket: bucket,
      Prefix: s3Params.Prefix,
    },
  };
  var finder = self.listObjects(listObjectsParams);
  var pend = new Pend();
  ee.progressAmount = 0;
  ee.progressTotal = 0;
  finder.on('error', function(err) {
    ee.emit('error', err);
  });
  finder.on('data', function(objects) {
    ee.progressTotal += objects.Contents.length;
    ee.emit('progress');
    if (objects.Contents.length > 0) {
      pend.go(deleteThem);
    }

    function deleteThem(cb) {
      var params = {
        Bucket: bucket,
        Delete: {
          Objects: objects.Contents.map(keyOnly),
          Quiet: true,
        },
        MFA: mfa,
      };
      var deleter = self.deleteObjects(params);
      deleter.on('error', function(err) {
        finder.abort();
        ee.emit('error', err);
      });
      deleter.on('end', function() {
        ee.progressAmount += objects.Contents.length;
        ee.emit('progress');
        cb();
      });
    }
  });
  finder.on('end', function() {
    pend.wait(function() {
      ee.emit('end');
    });
  });
  return ee;
}
```
- example usage
```shell
...
0. Now S3 object listing and MD5 sum computing are happening in parallel. As
   each operation progresses we compare both sorted lists side-by-side,
   iterating over them one at a time, downloading objects whose MD5 sums don't
   match the local file (or the local file is missing), and, if
   'deleteRemoved' is set, deleting local files whose corresponding objects
   are missing.

### client.deleteDir(s3Params)

Deletes an entire directory on S3.

's3Params':

* 'Bucket'
* 'Prefix'
...
```

#### <a name="apidoc.element.s3.Client.prototype.deleteObjects"></a>[function <span class="apidocSignatureSpan">s3.Client.prototype.</span>deleteObjects (s3Params)](#apidoc.element.s3.Client.prototype.deleteObjects)
- description and source-code
```javascript
deleteObjects = function (s3Params) {
  var self = this;
  var ee = new EventEmitter();

  var params = {
    Bucket: s3Params.Bucket,
    Delete: extend({}, s3Params.Delete),
    MFA: s3Params.MFA,
  };
  var slices = chunkArray(params.Delete.Objects, MAX_DELETE_COUNT);
  var errorOccurred = false;
  var pend = new Pend();

  ee.progressAmount = 0;
  ee.progressTotal = params.Delete.Objects.length;

  slices.forEach(uploadSlice);
  pend.wait(function(err) {
    if (err) {
      ee.emit('error', err);
      return;
    }
    ee.emit('end');
  });
  return ee;

  function uploadSlice(slice) {
    pend.go(function(cb) {
      doWithRetry(tryDeletingObjects, self.s3RetryCount, self.s3RetryDelay, function(err, data) {
        if (err) {
          cb(err);
        } else {
          ee.progressAmount += slice.length;
          ee.emit('progress');
          ee.emit('data', data);
          cb();
        }
      });
    });

    function tryDeletingObjects(cb) {
      self.s3Pend.go(function(pendCb) {
        params.Delete.Objects = slice;
        self.s3.deleteObjects(params, function(err, data) {
          pendCb();
          cb(err, data);
        });
      });
    }
  }
}
```
- example usage
```shell
...
 * ''progress'' - emitted when 'progressAmount', 'objectsFound', and
   'dirsFound' properties change.

And these methods:

 * 'abort()' - call this to stop the find operation.

### client.deleteObjects(s3Params)

See http://docs.aws.amazon.com/AWSJavaScriptSDK/latest/AWS/S3.html#deleteObjects-property

's3Params' are the same.

The difference between using AWS SDK 'deleteObjects' and this one:
...
```

#### <a name="apidoc.element.s3.Client.prototype.downloadBuffer"></a>[function <span class="apidocSignatureSpan">s3.Client.prototype.</span>downloadBuffer (s3Params)](#apidoc.element.s3.Client.prototype.downloadBuffer)
- description and source-code
```javascript
downloadBuffer = function (s3Params) {
  var self = this;
  var downloader = new EventEmitter();
  s3Params = extend({}, s3Params);

  downloader.progressAmount = 0;

  doWithRetry(doDownloadWithPend, self.s3RetryCount, self.s3RetryDelay, function(err, buffer) {
    if (err) {
      downloader.emit('error', err);
      return;
    }
    downloader.emit('end', buffer);
  });

  return downloader;

  function doDownloadWithPend(cb) {
    self.s3Pend.go(function(pendCb) {
      doTheDownload(function(err, buffer) {
        pendCb();
        cb(err, buffer);
      });
    });
  }

  function doTheDownload(cb) {
    var errorOccurred = false;
    var request = self.s3.getObject(s3Params);
    var hashCheckPend = new Pend();
    request.on('httpHeaders', function(statusCode, headers, resp) {
      if (statusCode >= 300) {
        handleError(new Error("http status code " + statusCode));
        return;
      }
      var contentLength = parseInt(headers['content-length'], 10);
      downloader.progressTotal = contentLength;
      downloader.progressAmount = 0;
      downloader.emit('progress');
      downloader.emit('httpHeaders', statusCode, headers, resp);
      var eTag = cleanETag(headers.etag);
      var eTagCount = getETagCount(eTag);

      var outStream = new StreamSink();
      var multipartETag = new MultipartETag({size: contentLength, count: eTagCount});
      var httpStream = resp.httpResponse.createUnbufferedStream();

      httpStream.on('error', handleError);
      outStream.on('error', handleError);

      hashCheckPend.go(function(cb) {
        multipartETag.on('end', function() {
          if (multipartETag.bytes !== contentLength) {
            handleError(new Error("Downloaded size does not match Content-Length"));
            return;
          }
          if (eTagCount === 1 && !multipartETag.anyMatch(eTag)) {
            handleError(new Error("ETag does not match MD5 checksum"));
            return;
          }
          cb();
        });
      });
      multipartETag.on('progress', function() {
        downloader.progressAmount = multipartETag.bytes;
        downloader.emit('progress');
      });
      outStream.on('finish', function() {
        if (errorOccurred) return;
        hashCheckPend.wait(function() {
          cb(null, outStream.toBuffer());
        });
      });

      httpStream.pipe(multipartETag);
      httpStream.pipe(outStream);
      multipartETag.resume();
    });

    request.send(handleError);

    function handleError(err) {
      if (!err) return;
      if (errorOccurred) return;
      errorOccurred = true;
      cb(err);
    }
  }
}
```
- example usage
```shell
...
And these events:

 * ''error' (err)'
 * ''end'' - emitted when the file is downloaded successfully
 * ''progress'' - emitted when 'progressAmount' and 'progressTotal'
   properties change.

### client.downloadBuffer(s3Params)

http://docs.aws.amazon.com/AWSJavaScriptSDK/latest/AWS/S3.html#getObject-property

 * 's3Params': params to pass to AWS SDK 'getObject'.

The difference between using AWS SDK 'getObject' and this one:
...
```

#### <a name="apidoc.element.s3.Client.prototype.downloadDir"></a>[function <span class="apidocSignatureSpan">s3.Client.prototype.</span>downloadDir (params)](#apidoc.element.s3.Client.prototype.downloadDir)
- description and source-code
```javascript
downloadDir = function (params) {
  return syncDir(this, params, false);
}
```
- example usage
```shell
...
0. Now S3 object listing and MD5 sum computing are happening in parallel. As
   each operation progresses we compare both sorted lists side-by-side,
   iterating over them one at a time, uploading files whose MD5 sums don't
   match the remote object (or the remote object is missing), and, if
   'deleteRemoved' is set, deleting remote objects whose corresponding local
   files are missing.

### client.downloadDir(params)

Syncs an entire directory from S3.

'params':

* 'localDir' - destination directory on local file system to sync to
* 's3Params'
...
```

#### <a name="apidoc.element.s3.Client.prototype.downloadFile"></a>[function <span class="apidocSignatureSpan">s3.Client.prototype.</span>downloadFile (params)](#apidoc.element.s3.Client.prototype.downloadFile)
- description and source-code
```javascript
downloadFile = function (params) {
  var self = this;
  var downloader = new EventEmitter();
  var localFile = params.localFile;
  var s3Params = extend({}, params.s3Params);

  var dirPath = path.dirname(localFile);
  downloader.progressAmount = 0;
  mkdirp(dirPath, function(err) {
    if (err) {
      downloader.emit('error', err);
      return;
    }

    doWithRetry(doDownloadWithPend, self.s3RetryCount, self.s3RetryDelay, function(err) {
      if (err) {
        downloader.emit('error', err);
        return;
      }
      downloader.emit('end');
    });
  });

  return downloader;

  function doDownloadWithPend(cb) {
    self.s3Pend.go(function(pendCb) {
      doTheDownload(function(err) {
        pendCb();
        cb(err);
      });
    });
  }

  function doTheDownload(cb) {
    var request = self.s3.getObject(s3Params);
    var errorOccurred = false;
    var hashCheckPend = new Pend();

    request.on('httpHeaders', function(statusCode, headers, resp) {
      if (statusCode >= 300) {
        handleError(new Error("http status code " + statusCode));
        return;
      }
      var contentLength = parseInt(headers['content-length'], 10);
      downloader.progressTotal = contentLength;
      downloader.progressAmount = 0;
      downloader.emit('progress');
      downloader.emit('httpHeaders', statusCode, headers, resp);
      var eTag = cleanETag(headers.etag);
      var eTagCount = getETagCount(eTag);

      var outStream = fs.createWriteStream(localFile);
      var multipartETag = new MultipartETag({size: contentLength, count: eTagCount});
      var httpStream = resp.httpResponse.createUnbufferedStream();

      httpStream.on('error', handleError);
      outStream.on('error', handleError);

      hashCheckPend.go(function(cb) {
        multipartETag.on('end', function() {
          if (multipartETag.bytes !== contentLength) {
            handleError(new Error("Downloaded size does not match Content-Length"));
            return;
          }
          if (eTagCount === 1 && !multipartETag.anyMatch(eTag)) {
            handleError(new Error("ETag does not match MD5 checksum"));
            return;
          }
          cb();
        });
      });
      multipartETag.on('progress', function() {
        downloader.progressAmount = multipartETag.bytes;
        downloader.emit('progress');
      });
      outStream.on('close', function() {
        if (errorOccurred) return;
        hashCheckPend.wait(cb);
      });

      httpStream.pipe(multipartETag);
      httpStream.pipe(outStream);
      multipartETag.resume();
    });

    request.send(handleError);

    function handleError(err) {
      if (!err) return;
      if (errorOccurred) return;
      errorOccurred = true;
      cb(err);
    }
  }
}
```
- example usage
```shell
...
  s3Params: {
    Bucket: "s3 bucket name",
    Key: "some/remote/file",
    // other options supported by getObject
    // See: http://docs.aws.amazon.com/AWSJavaScriptSDK/latest/AWS/S3.html#getObject-property
  },
};
var downloader = client.downloadFile(params);
downloader.on('error', function(err) {
  console.error("unable to download:", err.stack);
});
downloader.on('progress', function() {
  console.log("progress", downloader.progressAmount, downloader.progressTotal);
});
downloader.on('end', function() {
...
```

#### <a name="apidoc.element.s3.Client.prototype.downloadStream"></a>[function <span class="apidocSignatureSpan">s3.Client.prototype.</span>downloadStream (s3Params)](#apidoc.element.s3.Client.prototype.downloadStream)
- description and source-code
```javascript
downloadStream = function (s3Params) {
  var self = this;
  var downloadStream = new PassThrough();
  s3Params = extend({}, s3Params);

  doDownloadWithPend(function(err) {
    if (err) downloadStream.emit('error', err);
  });
  return downloadStream;

  function doDownloadWithPend(cb) {
    self.s3Pend.go(function(pendCb) {
      doTheDownload(function(err) {
        pendCb();
        cb(err);
      });
    });
  }

  function doTheDownload(cb) {
    var errorOccurred = false;
    var request = self.s3.getObject(s3Params);
    var hashCheckPend = new Pend();
    request.on('httpHeaders', function(statusCode, headers, resp) {
      if (statusCode >= 300) {
        handleError(new Error("http status code " + statusCode));
        return;
      }
      downloadStream.emit('httpHeaders', statusCode, headers, resp);
      var httpStream = resp.httpResponse.createUnbufferedStream();

      httpStream.on('error', handleError);

      downloadStream.on('finish', function() {
        if (errorOccurred) return;
        cb();
      });

      httpStream.pipe(downloadStream);
    });

    request.send(handleError);

    function handleError(err) {
      if (!err) return;
      if (errorOccurred) return;
      errorOccurred = true;
      cb(err);
    }
  }
}
```
- example usage
```shell
...

 * ''error' (err)'
 * ''end' (buffer)' - emitted when the file is downloaded successfully.
   'buffer' is a 'Buffer' containing the object data.
 * ''progress'' - emitted when 'progressAmount' and 'progressTotal'
   properties change.

### client.downloadStream(s3Params)

http://docs.aws.amazon.com/AWSJavaScriptSDK/latest/AWS/S3.html#getObject-property

 * 's3Params': params to pass to AWS SDK 'getObject'.

The difference between using AWS SDK 'getObject' and this one:
...
```

#### <a name="apidoc.element.s3.Client.prototype.listObjects"></a>[function <span class="apidocSignatureSpan">s3.Client.prototype.</span>listObjects (params)](#apidoc.element.s3.Client.prototype.listObjects)
- description and source-code
```javascript
listObjects = function (params) {
  var self = this;
  var ee = new EventEmitter();
  var s3Details = extend({}, params.s3Params);
  var recursive = !!params.recursive;
  var abort = false;

  ee.progressAmount = 0;
  ee.objectsFound = 0;
  ee.dirsFound = 0;
  findAllS3Objects(s3Details.Marker, s3Details.Prefix, function(err, data) {
    if (err) {
      ee.emit('error', err);
      return;
    }
    ee.emit('end');
  });

  ee.abort = function() {
    abort = true;
  };

  return ee;

  function findAllS3Objects(marker, prefix, cb) {
    if (abort) return;
    doWithRetry(listObjects, self.s3RetryCount, self.s3RetryDelay, function(err, data) {
      if (abort) return;
      if (err) return cb(err);

      ee.progressAmount += 1;
      ee.objectsFound += data.Contents.length;
      ee.dirsFound += data.CommonPrefixes.length;
      ee.emit('progress');
      ee.emit('data', data);

      var pend = new Pend();

      if (recursive) {
        data.CommonPrefixes.forEach(recurse);
        data.CommonPrefixes = [];
      }

      if (data.IsTruncated) {
        pend.go(findNext1000);
      }

      pend.wait(function(err) {
        cb(err);
      });

      function findNext1000(cb) {
        var nextMarker = data.NextMarker || data.Contents[data.Contents.length - 1].Key;
        findAllS3Objects(nextMarker, prefix, cb);
      }

      function recurse(dirObj) {
        var prefix = dirObj.Prefix;
        pend.go(function(cb) {
          findAllS3Objects(null, prefix, cb);
        });
      }
    });

    function listObjects(cb) {
      if (abort) return;
      self.s3Pend.go(function(pendCb) {
        if (abort) {
          pendCb();
          return;
        }
        s3Details.Marker = marker;
        s3Details.Prefix = prefix;
        self.s3.listObjects(s3Details, function(err, data) {
          pendCb();
          if (abort) return;
          cb(err, data);
        });
      });
    }
  }
}
```
- example usage
```shell
...
If you want retries, progress, or MD5 checking, you must code it yourself.

Returns a 'ReadableStream' with these additional events:

* ''httpHeaders' (statusCode, headers)' - contains the HTTP response
  headers and status code.

### client.listObjects(params)

See http://docs.aws.amazon.com/AWSJavaScriptSDK/latest/AWS/S3.html#listObjects-property

'params':

* 's3Params' - params to pass to AWS SDK 'listObjects'.
* (optional) 'recursive' - 'true' or 'false' whether or not you want to recurse
...
```

#### <a name="apidoc.element.s3.Client.prototype.moveObject"></a>[function <span class="apidocSignatureSpan">s3.Client.prototype.</span>moveObject (s3Params)](#apidoc.element.s3.Client.prototype.moveObject)
- description and source-code
```javascript
moveObject = function (s3Params) {
  var self = this;
  var ee = new EventEmitter();
  var copier = self.copyObject(s3Params);
  var copySource = s3Params.CopySource;
  var mfa = s3Params.MFA;
  copier.on('error', function(err) {
    ee.emit('error', err);
  });
  copier.on('end', function(data) {
    ee.emit('copySuccess', data);
    var slashIndex = copySource.indexOf('/');
    var sourceBucket = copySource.substring(0, slashIndex);
    var sourceKey = copySource.substring(slashIndex + 1);
    var deleteS3Params = {
      Bucket: sourceBucket,
      Delete: {
        Objects: [
          {
            Key: sourceKey,
          },
        ],
        Quiet: true,
      },
      MFA: mfa,
    };
    var deleter = self.deleteObjects(deleteS3Params);
    deleter.on('error', function(err) {
      ee.emit('error', err);
    });
    var deleteData;
    deleter.on('data', function(data) {
      deleteData = data;
    });
    deleter.on('end', function() {
      ee.emit('end', deleteData);
    });
  });
  return ee;
}
```
- example usage
```shell
...
 * Retry based on the client's retry settings.

Returns an 'EventEmitter' with these events:

 * ''error' (err)'
 * ''end' (data)'

### client.moveObject(s3Params)

See http://docs.aws.amazon.com/AWSJavaScriptSDK/latest/AWS/S3.html#copyObject-property

's3Params' are the same. Don't forget that 'CopySource' must contain the
source bucket name as well as the source key name.

Under the hood, this uses 'copyObject' and then 'deleteObjects' only if the
...
```

#### <a name="apidoc.element.s3.Client.prototype.uploadDir"></a>[function <span class="apidocSignatureSpan">s3.Client.prototype.</span>uploadDir (params)](#apidoc.element.s3.Client.prototype.uploadDir)
- description and source-code
```javascript
uploadDir = function (params) {
  return syncDir(this, params, true);
}
```
- example usage
```shell
...
  s3Params: {
    Bucket: "s3 bucket name",
    Prefix: "some/remote/dir/",
    // other options supported by putObject, except Body and ContentLength.
    // See: http://docs.aws.amazon.com/AWSJavaScriptSDK/latest/AWS/S3.html#putObject-property
  },
};
var uploader = client.uploadDir(params);
uploader.on('error', function(err) {
  console.error("unable to sync:", err.stack);
});
uploader.on('progress', function() {
  console.log("progress", uploader.progressAmount, uploader.progressTotal);
});
uploader.on('end', function() {
...
```

#### <a name="apidoc.element.s3.Client.prototype.uploadFile"></a>[function <span class="apidocSignatureSpan">s3.Client.prototype.</span>uploadFile (params)](#apidoc.element.s3.Client.prototype.uploadFile)
- description and source-code
```javascript
uploadFile = function (params) {
  var self = this;
  var uploader = new EventEmitter();
  uploader.progressMd5Amount = 0;
  uploader.progressAmount = 0;
  uploader.progressTotal = 0;
  uploader.abort = handleAbort;

  var localFile = params.localFile;
  var localFileStat = null;
  var s3Params = extend({}, params.s3Params);
  if (s3Params.ContentType === undefined) {
    var defaultContentType = params.defaultContentType || 'application/octet-stream';
    s3Params.ContentType = mime.lookup(localFile, defaultContentType);
  }
  var fatalError = false;
  var localFileSlicer = null;
  var parts = [];

  openFile();

  return uploader;

  function handleError(err) {
    if (localFileSlicer) {
      localFileSlicer.unref();
      localFileSlicer = null;
    }
    if (fatalError) return;
    fatalError = true;
    uploader.emit('error', err);
  }

  function handleAbort() {
    fatalError = true;
  }

  function openFile() {
    fs.open(localFile, 'r', function(err, fd) {
      if (err) return handleError(err);
      localFileSlicer = fd_slicer.createFromFd(fd, {autoClose: true});
      localFileSlicer.on('error', handleError);
      localFileSlicer.on('close', function() {
        uploader.emit('fileClosed');
      });

      // keep an extra reference alive until we decide that we're completely
      // done with the file
      localFileSlicer.ref();

      uploader.emit('fileOpened', localFileSlicer);

      fs.fstat(fd, function(err, stat) {
        if (err) return handleError(err);
        localFileStat = stat;
        uploader.progressTotal = stat.size;
        startPuttingObject();
      });
    });
  }

  function startPuttingObject() {
    if (localFileStat.size >= self.multipartUploadThreshold) {
      var multipartUploadSize = self.multipartUploadSize;
      var partsRequiredCount = Math.ceil(localFileStat.size / multipartUploadSize);
      if (partsRequiredCount > MAX_MULTIPART_COUNT) {
        multipartUploadSize = smallestPartSizeFromFileSize(localFileStat.size);
      }
      if (multipartUploadSize > MAX_PUTOBJECT_SIZE) {
        var err = new Error("File size exceeds maximum object size: " + localFile);
        err.retryable = false;
        handleError(err);
        return;
      }
      startMultipartUpload(multipartUploadSize);
    } else {
      doWithRetry(tryPuttingObject, self.s3RetryCount, self.s3RetryDelay, onPutObjectDone);
    }

    function onPutObjectDone(err, data) {
      if (fatalError) return;
      if (err) return handleError(err);
      if (localFileSlicer) {
        localFileSlicer.unref();
        localFileSlicer = null;
      }
      uploader.emit('end', data);
    }
  }

  function startMultipartUpload(multipartUploadSize) {
    doWithRetry(tryCreateMultipartUpload, self.s3RetryCount, self.s3RetryDelay, function(err, data) {
      if (fatalError) return;
      if (err) return handleError(err);
      uploader.emit('data', data);
      s3Params = {
        Bucket: s3Params.Bucket,
        Key: s3Params.Key,
        SSECustomerAlgorithm: s3Params.SSECustomerAlgorithm,
        SSECustomerKey: s3Params.SSECustomerKey,
        SSECustomerKeyMD5: s3Params.SSECustomerKeyMD5,
      };
      queueAllParts(data.UploadId, multipartUploadSize);
    });
  }

  function queueAllParts(uploadId, multipartUploadSize) {
    var cursor = 0;
    var nextPartNumber = 1;
    var pend = new Pend();
    while (cursor < localFileStat.size) {
      var start = cursor;
      var end = cursor + multipartUploadSize;
      if (end > localFileStat.size) {
        end = localFileStat.size;
      }
      cursor = end;
      var part = {
        ETag: null,
        PartNumber: nextPartNumber++,
      };
      parts.push(part);
      pend.go(makeUploadPartFn(start, end, part, uploadId));
    }
    pend.wait(function(err) {
      if (fatalError) return;
      if (err) return handleError(err);
      completeMultipartUpload();
    });
  }

  function makeUploadPartFn(start, end, part, uploadId) {
    return function(cb) {
      doWithRetry(tryUploadPart, self.s3RetryCount, self.s3RetryDelay, function(err, data) {
        if (fatalError) ...
```
- example usage
```shell
...
  s3Params: {
    Bucket: "s3 bucket name",
    Key: "some/remote/file",
    // other options supported by putObject, except Body and ContentLength.
    // See: http://docs.aws.amazon.com/AWSJavaScriptSDK/latest/AWS/S3.html#putObject-property
  },
};
var uploader = client.uploadFile(params);
uploader.on('error', function(err) {
  console.error("unable to upload:", err.stack);
});
uploader.on('progress', function() {
  console.log("progress", uploader.progressMd5Amount,
            uploader.progressAmount, uploader.progressTotal);
});
...
```



# <a name="apidoc.module.s3.MultipartETag"></a>[module s3.MultipartETag](#apidoc.module.s3.MultipartETag)

#### <a name="apidoc.element.s3.MultipartETag.MultipartETag"></a>[function <span class="apidocSignatureSpan">s3.</span>MultipartETag (options)](#apidoc.element.s3.MultipartETag.MultipartETag)
- description and source-code
```javascript
function MultipartETag(options) {
  options = options || {};
  Transform.call(this, options);
  var sizes = [
    maximumUploadSize,
    minimumUploadSize,
    commonUploadSize1,
    commonUploadSize2,
  ];
  if (options.size != null && options.count != null) {
    if (options.count === 1) {
      sizes = [maximumUploadSize];
    } else {
      sizes.push(guessPartSizeFromSizeAndCount(options.size, options.count));
    }
  }
  this.sums = [];
  this.bytes = 0;
  this.digest = null; // if it is less than maximumUploadSize
  this.done = false;
  for (var i = 0; i < sizes.length; i += 1) {
    this.sums.push({
      size: sizes[i],
      hash: crypto.createHash('md5'),
      amtWritten: 0,
      digests: [],
      eTag: null,
    });
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.MultipartETag.super_"></a>[function <span class="apidocSignatureSpan">s3.MultipartETag.</span>super_ (options)](#apidoc.element.s3.MultipartETag.super_)
- description and source-code
```javascript
function Transform(options) {
  if (!(this instanceof Transform))
    return new Transform(options);

  Duplex.call(this, options);

  this._transformState = new TransformState(this);

  var stream = this;

  // start out asking for a readable event once data is transformed.
  this._readableState.needReadable = true;

  // we have implemented the _read method, and done the other things
  // that Readable wants before the first _read call, so unset the
  // sync guard flag.
  this._readableState.sync = false;

  if (options) {
    if (typeof options.transform === 'function')
      this._transform = options.transform;

    if (typeof options.flush === 'function')
      this._flush = options.flush;
  }

  // When the writable side finishes, then flush out anything remaining.
  this.once('prefinish', function() {
    if (typeof this._flush === 'function')
      this._flush(function(er) {
        done(stream, er);
      });
    else
      done(stream);
  });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.s3.MultipartETag.prototype"></a>[module s3.MultipartETag.prototype](#apidoc.module.s3.MultipartETag.prototype)

#### <a name="apidoc.element.s3.MultipartETag.prototype._flush"></a>[function <span class="apidocSignatureSpan">s3.MultipartETag.prototype.</span>_flush (callback)](#apidoc.element.s3.MultipartETag.prototype._flush)
- description and source-code
```javascript
_flush = function (callback) {
  for (var i = 0; i < this.sums.length; i += 1) {
    var sumObj = this.sums[i];
    var digest = sumObj.hash.digest();
    sumObj.digests.push(digest);
    var finalHash = crypto.createHash('md5');
    for (var partIndex = 0; partIndex < sumObj.digests.length; partIndex += 1) {
      digest = sumObj.digests[partIndex];
      finalHash.update(digest);
    }
    sumObj.eTag = finalHash.digest('hex') + '-' + sumObj.digests.length;
    if (i === 0 && sumObj.digests.length === 1) {
      this.digest = digest;
    }
  }
  this.done = true;
  this.push(null);
  callback();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.MultipartETag.prototype._transform"></a>[function <span class="apidocSignatureSpan">s3.MultipartETag.prototype.</span>_transform (chunk, encoding, callback)](#apidoc.element.s3.MultipartETag.prototype._transform)
- description and source-code
```javascript
_transform = function (chunk, encoding, callback) {
  this.bytes += chunk.length;
  for (var i = 0; i < this.sums.length; i += 1) {
    var sumObj = this.sums[i];
    var newAmtWritten = sumObj.amtWritten + chunk.length;
    if (newAmtWritten <= sumObj.size) {
      sumObj.amtWritten = newAmtWritten;
      sumObj.hash.update(chunk, encoding);
    } else {
      var finalBytes = sumObj.size - sumObj.amtWritten;
      sumObj.hash.update(chunk.slice(0, finalBytes), encoding);
      sumObj.digests.push(sumObj.hash.digest());
      sumObj.hash = crypto.createHash('md5');
      sumObj.hash.update(chunk.slice(finalBytes), encoding);
      sumObj.amtWritten = chunk.length - finalBytes;
    }
  }
  this.emit('progress');
  callback();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.s3.MultipartETag.prototype.anyMatch"></a>[function <span class="apidocSignatureSpan">s3.MultipartETag.prototype.</span>anyMatch (eTag)](#apidoc.element.s3.MultipartETag.prototype.anyMatch)
- description and source-code
```javascript
anyMatch = function (eTag) {
  if (this.digest && this.digest.toString('hex') === eTag) {
    return true;
  }
  for (var i = 0; i < this.sums.length; i += 1) {
    if (this.sums[i].eTag === eTag) {
      return true;
    }
  }
  return false;
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
