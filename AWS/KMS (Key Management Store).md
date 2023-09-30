Use AWS KMS to encrypt data across your AWS workloads, digitally sign data, encrypt within your  applications using AWS Encryption SDK

While AWS KMS does support sending data up to 4 KB to be encrypted directly, envelope encryption can offer significant performance benefits. When you encrypt data directly with AWS KMS it must be transferred over the network. Envelope encryption reduces the network load since only the request and delivery of the much smaller data key go over the network.

Environment variables must not exceed 4 KB