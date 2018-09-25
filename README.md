# Making-Objects-Publicly-Available-from-IBM-Cloud-Object-Storage-

IBM Cloud Object Storage offers a way to store and serve unstructured data in the cloud. Developers can access objects via APIs, as well as store new objects through applications. 

Users may also need to make objects such as video clips, presentations or documents available publicly outside of applications – for example as an embedded URL within an email. This can be more difficult from IBM Cloud Object Storage, since it does not support automatic static website hosting (though it is possible to manually configure a web server and use it to serve publicly accessible content hosted in Object Storage. For more information, see this tutorial) but it is possible on an object-by-object basis.

I’ve created this ‘how-to’ guide to complement the official IBM Cloud documentation pages and provide a step-by-step approach to providing quick public access to particular objects stored in IBM Cloud Object Storage, via a URL. 

This will be done in two ways: the first using the IBM Cloud Object Storage API via Identity and Access Management; the second using a pre-signed URL and HMAC Authentication. In both cases, commands will be issued from the command line.

Note – this will make files available on the public internet, to anyone or process that has its URL. Ensure that any files that you expose do not contain sensitive information that should not be shared with the world. 
