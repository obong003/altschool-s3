# Display Static webpage using an S3 Bucket

## The Process

### I first initialised a root user with different Privileges
![user with permissions](./img/new%20policies%20in%20permisssion.png)
### Next was to create a bUcket via S3
![new bucket](./img/created%20a%20bucket.png)
### Now, upload images to the folder. 
PS. I seperated the index.html and style.css files and uploaded them seperately before uploading the entire folder. I encountered an issue when trying to upload them directly with the folder. 
![new objects](./img/all%20objects%20uploaded%20to%20the%20bucket.png)
### Moved to create a Cloudfront as CDN for distribution
![new distribtion](./img/new%20cloudfront%20distribution.png)
#### I configured different settings to help render the page

> added origin domain
> changed the origin access to origin access control
> created a new OAC
> clicked on create.
> enabled security protections
> entered index.html in the default root object. This specified the root object to be displayed on the webpage. 
> finally clicked on create distribution. 

### Adjust New Policy for the Bucket in permissions
> cloudfront generated a new policy which I had to add my S3 bucket settings. I added them in the settings. 
![new additions for cloudfront](./img/new%20policy%20from%20cloudfront.png)
### Returned back to the cloudfront and copied the distribution URL
![new link for distribution](./img/new%20link%20for%20distribution.png)
## Static webpage displays on the browser
![static page on browser](./img/final%20rendition%20on%20browser.png)
