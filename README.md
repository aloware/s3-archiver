# S3 Archiver

Make an archive from a directory and all subsequent subdirectories and objects in S3.
The trick is will upload the archive directly to S3, without having to download it to the local machine.

## Installation
- Clone the repository to your local machine:
```bash
git clone https://github.com/aloware/s3-archiver.git
```
- Install the dependencies:
```bash
cd s3-archiver
npm install
```
- Configure the AWS credentials:
Check the [AWS CLI](https://docs.aws.amazon.com/cli/latest/userguide/cli-configure-files.html) for more information.


## Usage
```bash
node index.js -b <bucket> -d <directory> -z <zipfileName> [-r deleteFiles]
```

## Result
The archive will be uploaded to selected directory of the bucket.
