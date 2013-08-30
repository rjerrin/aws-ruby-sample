# AWS SDK for Ruby Sample Project

A simple Ruby application illustrating usage of the AWS SDK for Ruby (aws-sdk gem).

## Requirements

The only requirement of this application is bundler. All other dependencies can be installed with:
    
    bundle install

## Basic Configuration

You need to set your AWS security credentials in `config.yml` before the sample
is able to connect to AWS. This file should contain:

    access_key_id: <your access key id>
    secret_access_key: <your secret key>

See the [Security Credentials](http://aws.amazon.com/security-credentials) page
for more information on getting your keys.

## Running the S3 sample

This sample application connects to Amazon's [Simple Storage Service (S3)](http://aws.amazon.com/s3),
creates a bucket, and uploads a file to that bucket. We've already included a
file to upload (`hello_world.txt`) and the `upload_file.rb` script will generate
a unique bucket name for you. All you need to do is run it:

    ruby upload_file.rb hello_world.txt

The S3 documentation has a good overview of the [restrictions for bucket names](http://docs.aws.amazon.com/AmazonS3/latest/dev/BucketRestrictions.html)
for when you start making your own buckets.

## License

This sample application is distributed under the
[Apache License, Version 2.0](http://www.apache.org/licenses/LICENSE-2.0).

```no-highlight
Copyright 2013. Amazon Web Services, Inc. All Rights Reserved.

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
```
