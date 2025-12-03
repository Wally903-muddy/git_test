# An S3 static website project.
---

This was put together to demonstrate how easy it is to build a CI/CD pipeline
combining GitHub Actions and various AWS services.

- Create a static website locally.
- Push the website code to a *GitHub* repository.
- Create an S3 bucket on AWS and enable static website hosting.
- Upload the website code to the S3 bucket.
- Create an AWS IAM *user* with read and write permissions for the S3 bucket (using an AWS *Policy*).
- For the IAM *user* also generate Access and Secret Access keys.
- Configure *GitHub Actions* on the repository webpage adding a *YAML* file to syncronise the repository with the AWS S3 bucket. 
- Add the *user* keys as *GitHub* repository secrets so they can be accessed by *GitHub Actions*.
- Test the set up. Make changes to the local files and push the changes to GitHub. 
- Open http://the-bucket-at-the-end-of-the-rainbow.s3-website.eu-north-1.amazonaws.com/ to see if the changes have percolated through.
