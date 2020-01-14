# Folder structure

- imgs
  - icons
  - products
  - test
- styles
- modules
  - lit-element
  - lit-html
  - kaskadi-apps
  - kaskadi-elements
  - kaskadi-scripts
- scripts
- pico
  - miniwebsite1
  - ...
  - miniwebsiteN
- home
  - user1
  - ...
  - userN

# How to upload files to the CDN/bucket?

Until a client has been developed, you can use the following:
1. Copy a single file to the bucket: `aws s3 cp path/to/your/file s3://kaskadi-public/path/to/your/file/in/bucket`. The same command can be used for many [operations](https://docs.aws.amazon.com/cli/latest/reference/s3/cp.html) like for example moving files between buckets
2. Move a file inside of the bucket: `aws s3 mv path/to/your/file s3://kaskadi-public/path/to/your/file/in/bucket`. You can also use this command to move a file inside of the bucket (replace local path by bucket path) or rename files
3. Remove a file from the bucket: `aws s3 rm s3://kaskadi-public/path/to/your/file/in/bucket`

_For more details and advanced options_: [AWS CLI S3 documentation](https://docs.aws.amazon.com/cli/latest/reference/s3/)
