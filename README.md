### The Jack Fund

Hosted as a static site on S3:

http://thejackfund.com.s3-website-us-east-1.amazonaws.com/

Bucket policy:

```
{
  "Version": "2012-10-17",
  "Statement": [
    {
      "Sid": "AddPerm",
      "Effect": "Allow",
      "Principal": "*",
      "Action": "s3:GetObject",
      "Resource": "arn:aws:s3:::thejackfund.com/*"
    }
  ]
}
```

