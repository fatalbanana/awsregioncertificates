## AWS Region Certificates for Go

[![GHA](https://github.com/fatalbanana/awsregioncertificates/actions/workflows/ci.yml/badge.svg)](https://github.com/fatalbanana/awsregioncertificates/actions/workflows/ci.yml)
[![GHA](https://github.com/fatalbanana/awsregioncertificates/actions/workflows/generate_test.yml/badge.svg)](https://github.com/fatalbanana/awsregioncertificates/actions/workflows/generate_test.yml)

Embeds region certificates from AWS (run `go generate ./...` to refresh them) - AFAIU they can only be downloaded as part of documentation.

Can be used to validate EC2 [instance identity documents](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/instance-identity-documents.html) using the `rsa`/`base64-encoded signature`.

## Criticisms

 * Documentation is not a reasonable format to distribute the certificates in
 * Rollover hurts and refreshing certificates timeously is difficult
 * For lack of a timestamp or nonce (like supported in GCP, Azure) instance IDs are of questionable usefulness

## Expiry dates

| Region | Expiry date |
|---|---|
| af-south-1 | 2199-05-02 07:14:05 UTC |
| ap-east-1 | 2029-02-02 03:00:06 UTC |
| ap-east-2 | 2203-10-29 14:56:06 UTC |
| ap-northeast-1 | 2029-04-28 12:23:10 UTC |
| ap-northeast-2 | 2029-04-28 13:38:46 UTC |
| ap-northeast-3 | 2029-04-28 16:54:07 UTC |
| ap-south-1 | 2029-04-28 14:13:01 UTC |
| ap-south-2 | 2031-05-27 10:43:29 UTC |
| ap-southeast-1 | 2029-04-28 14:30:14 UTC |
| ap-southeast-2 | 2029-04-28 15:21:43 UTC |
| ap-southeast-3 | 2031-04-21 12:06:40 UTC |
| ap-southeast-4 | 2031-06-02 10:43:53 UTC |
| ap-southeast-5 | 2203-06-09 12:57:54 UTC |
| ap-southeast-6 | 2204-05-09 12:13:06 UTC |
| ap-southeast-7 | 2203-09-17 15:28:56 UTC |
| ca-central-1 | 2029-04-28 15:35:43 UTC |
| ca-west-1 | 2201-10-18 01:36:09 UTC |
| cn-north-1 | 2028-07-02 08:35:39 UTC |
| cn-northwest-1 | 2028-07-02 08:35:39 UTC |
| eu-central-1 | 2029-04-28 15:55:29 UTC |
| eu-central-2 | 2031-05-25 10:54:00 UTC |
| eu-north-1 | 2029-04-28 16:06:03 UTC |
| eu-south-1 | 2199-03-29 15:19:09 UTC |
| eu-south-2 | 2031-06-08 08:43:31 UTC |
| eu-west-1 | 2029-04-28 16:18:10 UTC |
| eu-west-2 | 2029-04-28 16:29:14 UTC |
| eu-west-3 | 2029-04-28 16:37:38 UTC |
| eusc-de-east-1 | 2204-03-24 09:39:37 UTC |
| il-central-1 | 2200-11-11 18:26:35 UTC |
| me-central-1 | 2200-04-14 18:39:33 UTC |
| me-south-1 | 2198-09-29 14:32:47 UTC |
| mx-central-1 | 2029-04-01 12:50:36 UTC |
| sa-east-1 | 2029-04-28 16:46:09 UTC |
| us-east-1 | 2029-04-28 17:34:01 UTC |
| us-east-2 | 2029-04-28 17:11:49 UTC |
| us-gov-east-1 | 2029-05-06 15:22:36 UTC |
| us-gov-west-1 | 2029-05-06 17:30:32 UTC |
| us-west-1 | 2029-04-28 17:02:43 UTC |
| us-west-2 | 2029-04-28 17:23:59 UTC |
