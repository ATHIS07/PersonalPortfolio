# Static Website Hosting using AWS S3 and CloudFront

This project demonstrates hosting a static website using Amazon S3 for storage and Amazon CloudFront as a Content Delivery Network (CDN) to improve performance and availability.

## Project Overview
A simple static website was deployed by storing website files in an S3 bucket and distributing the content globally using CloudFront. Custom error handling was implemented to improve user experience.

## Services Used
- Amazon S3 – to store static website files (index.html, error.html)
- Amazon CloudFront – for global content delivery and caching

## Architecture
User → CloudFront → S3

## Features
- Static website hosting using Amazon S3  
- Faster content delivery using CloudFront CDN  
- Custom error page (error.html) for better UX  
- Cost-efficient setup without using WAF or paid services  

## Deployment Steps (High Level)
1. Created an S3 bucket and uploaded static website files.
2. Enabled static website hosting in S3.
3. Created a CloudFront distribution with the S3 bucket as the origin.
4. Configured CloudFront to serve custom error pages.
5. Accessed the website using the CloudFront distribution URL.

## Outcome
- Improved website performance through CDN caching
- Global accessibility without managing servers
- Zero-cost deployment using AWS free-tier services

## Future Enhancements
- Make the S3 bucket private and access it via CloudFront OAC
- Add AWS WAF for security when budget allows
- Automate deployment using GitHub Actions
