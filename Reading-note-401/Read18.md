# AWS: API, Dynamo and Lambda 

### Review, Research, and Discussion

1. What are serverless functions?
- A serverless function is a programmatic function written by a software developer for a single purpose. It's then hosted and maintained on infrastructure by cloud computing companies. These companies take care of code maintenance and execution so that developers can deploy new code faster and easier

2. If you were to create a system that emulated Lambda functions, how would you do it?
- Open the Functions page on the Lambda console.

- Choose Create function.

- Under Basic information, do the following:

- For Function name, enter my-function.

- For Runtime, confirm that Node.js 14.x is selected. Note that Lambda provides runtimes for .NET (PowerShell, C#), Go, Java, Node.js, Python, and Ruby.

- Choose Create function.
3. Describe how a CDN works
- The mission of a CDN is to reduce latency. Latency is that annoying delay you experience when trying to access a web page or video stream before it fully loads on your device. Although measured in milliseconds, it can feel like forever, and may even result in a load error or time-out. Some content delivery networks alleviate latency by reducing the physical distance that the content needs to travel to reach you

[cdn ref](https://www.akamai.com/our-thinking/cdn/what-is-a-cdn#:~:text=A%20CDN%20(Content%20Delivery%20Network,the%20server%20and%20the%20user.&text=Without%20a%20CDN%2C%20content%20origin,every%20single%20end%20user%20request.))


### Document the following Vocabulary Terms

**Serverless Functions**
- A serverless function is a programmatic function written by a software developer for a single purpose. It's then hosted and maintained on infrastructure by cloud computing companies. These companies take care of code maintenance and execution so that developers can deploy new code faster and easier

**Cloud Storage**
- Cloud storage is a cloud computing model that stores data on the Internet through a cloud computing provider who manages and operates data storage as a service. It's delivered on demand with just-in-time capacity and costs, and eliminates buying and managing your own data storage infrastructure.

**CDN**
- A content delivery network (CDN) is a group of geographically distributed servers that speed up the delivery of web content by bringing it closer to where users are. Data centers across the globe use caching, a process that temporarily stores copies of files, so that you can access internet content from a web-enabled device or browser more quickly through a server near you