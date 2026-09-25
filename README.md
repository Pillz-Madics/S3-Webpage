WTC-2MGRHDW8

# Host a Website on Amazon S3

**Project Link:** [View Project](https://nextwork.ai/projects/70e2d059-31ab-5f67-8c58-f5edbd451140)

**Author:** Ludwick Molebale  
**Email:** madimetjamolebale8@gmail.com

---

![Image](https://nextwork.ai/stimulated_orange_joyful_cape_gooseberry/uploads/aws-host-a-website-on-s3_5d4474f9)

## Introducing Today's Project!

### Project overview

In this project, I will demonstrate how to host a static website using a s3 bucket. I'm doing this project to learn how s3 works and how it manages files and access.

### Tools and concepts

Services I used were S3 Key concepts I learnt include file and web hosting using S3, access management using ACL and Bucket policy

### Time, challenges, and wins

This project took me approximately an hour. The most challenging part was setting up the policy and static page hosting. It was most rewarding to finaly be able to access the page using the endpoint url

## How I Set Up an S3 Bucket

### What I did in this step

In this step, I will open an Amazon S3 to create storage for my website because S3 is where we will be storing all the files for our website

### How long it took to create the bucket

Creating an S3 bucket took me 5 minutes, but the process in future will take a lot less

### Region selection

The Region I picked for my S3 bucket was I picked Africa(Cape Town) because it's the region closest to me.

### Understanding bucket name uniqueness

S3 bucket names are globally unique! This means no other AWS account in the whole world can use this bucket name

![Image](https://nextwork.ai/stimulated_orange_joyful_cape_gooseberry/uploads/aws-host-a-website-on-s3_ba6d42ad)

## Upload Website Files to S3

### What I did in this step

In this step, I will add the website files to the bucket because we want to have the files available in the S3 in order to access the website

### Files I uploaded

I uploaded two files to my S3 bucket - they were the index.html file and it's assets folder

### How the files work together

Both files are necessary for this project as one defines the structure of the page and the other contains visual contents of the site(images)

![Image](https://nextwork.ai/stimulated_orange_joyful_cape_gooseberry/uploads/aws-host-a-website-on-s3_a265af88)

## Static Website Hosting on S3

### What I did in this step

In this step, I will configure the S3 for web hosting and expose the link because we want the website to be accessible

### Understanding website hosting

Website hosting means we're making the website accessible on the internet

### How I enabled website hosting

To enable website hosting with my S3 bucket, I went to the properties tab in my S3 bucket, went to the static web hosting tab, then enabled it. after enabling it I selected static hosting type then entered the name of my html file as the web page document.

### Access Control Lists (ACLs)

An ACL is a set of rules that control who can access each object in your bucket

![Image](https://nextwork.ai/stimulated_orange_joyful_cape_gooseberry/uploads/aws-host-a-website-on-s3_c22c54c0)

## Bucket Endpoints

### Understanding bucket endpoint URLs

Once static website is enabled, S3 produces a bucket endpoint URL, which is how we can access the bucket's files as a website.

### What I saw when I tested the endpoint

When I first visited the bucket endpoint URL, I saw 403 Forbidden. The reason for this error was because the bucket's objects are still private

![Image](https://nextwork.ai/stimulated_orange_joyful_cape_gooseberry/uploads/aws-host-a-website-on-s3_22ce4daf)

## Success!

### What I did in this step

In this step, I will make the objects in the bucket public because we want them to be accessible.

### How I resolved the 403 error

To resolve this 403 Forbidden error, I made the objects public using ACL

![Image](https://nextwork.ai/stimulated_orange_joyful_cape_gooseberry/uploads/aws-host-a-website-on-s3_5d4474f9)

## Bucket Policies

### What I did in this extension

In this project extension I'm about to setup a bucket policy. I'm doing this so that people won't be able to delete my index document/object

### Understanding bucket policies

An alternative to ACLs are bucket policies, which are used to control how the bucket is managed. The benefit of using bucket policies is that you have a much higher level of control over you bucket and how it is managed, while ACLs are useful for controling just access of objects

![Image](https://nextwork.ai/stimulated_orange_joyful_cape_gooseberry/uploads/aws-host-a-website-on-s3_sm2sm2sm)

### What my bucket policy does

My bucket policy prevents everyone from deleting the index file. I tested this by trying to delete the index file and saw a warning saying access denied.

---

*Built with [NextWork](https://nextwork.ai) - [View this project](https://nextwork.ai/projects/70e2d059-31ab-5f67-8c58-f5edbd451140)*
