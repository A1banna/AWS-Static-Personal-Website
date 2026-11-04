# AWS-Static-Personal-Website
Simple Static Website Created in AWS

A simple static portfolio website hosted on AWS.
The S3 Bucket is Private, and CloudFront delivers the site over HTTPS.
Site: https://dt1phoe688hud.cloudfront.net

## Architecture
### Architecture is as follows:
Visitor Opens the CloudFront URL -> 
  CloudFront delivers the page from the nearest edge location, or gets it from the S3 Bucket if it wasn't cached
 [S3 Bucket stays private; only CloudFront is allowed to read from it]

## AWS Services used
Amazon S3: Stores the Site's files (Index.html & the badge image)
Amazon CloudFront:Delivers the site over HTTPS, caches content globally

## Screenshots Description:
S1: Live Site Over HTTPS

<p align="center">
  <img src="https://github.com/A1banna/AWS-Static-Personal-Website/blob/9621f2815baf819fd96583e9df1b740167706f79/SS1.png" width="500">
</p>

S2: CloudFront Distribution Deployed

<p align="center">
  <img src="https://github.com/A1banna/AWS-Static-Personal-Website/blob/578032e5cb98cbabc78624eb0c5423b753b1dade/SS2.png" width="500">
</p>

S3: S3 Bucket Contents

<p align="center">
  <img src="https://github.com/A1banna/AWS-Static-Personal-Website/blob/578032e5cb98cbabc78624eb0c5423b753b1dade/SS3.png" width="500">
</p>

S4: S3 Bucket Contents with Versioning Enabled

<p align="center">
  <img src="https://github.com/A1banna/AWS-Static-Personal-Website/blob/578032e5cb98cbabc78624eb0c5423b753b1dade/SS4.png" width="500">
</p>

S5: CloudFront Distribution Invalidations

<p align="center">
  <img src="https://github.com/A1banna/AWS-Static-Personal-Website/blob/578032e5cb98cbabc78624eb0c5423b753b1dade/SS5.png" width="500">
</p>

S6: Block Public Access Enabled (Bucket Is Private)

<p align="center">
  <img src="https://github.com/A1banna/AWS-Static-Personal-Website/blob/578032e5cb98cbabc78624eb0c5423b753b1dade/SS6.png" width="500">
</p>
  
## Key Things I've Learnt:
-  Why a private bucket plus CloudFront is better than public S3 website hosting (HTTPS, security, speed)
-  How CloudFront caching works and why invalidations are needed after updates
