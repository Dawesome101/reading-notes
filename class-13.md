# Local Storage with Websites

## Index

[Home](README.md)  
[Local Storage and How to Use it on Websites](#local-storage-and-how-to-use-it-on-websites)  

## [Local Storage and How to Use it on Websites](https://www.smashingmagazine.com/2010/10/local-storage-and-how-to-use-it/)

1. Why would a developer use local storage for a web application?
   - To get around the statless nature of HTTP without having to bounce data back and forth from a server.  Everything is done client side so it's limited only by the speed of the users device and almost all devices can compute the tiny amounts of data(up to 4kb) in the blink of an eye.  It's faster, it gets around a stateless protocol and can generally make an interactive website better by giving it "memory" of the its users interactions without having to store anything server-side.
2. What information should not be stored in local storage?
   - Information of a user or a users actions without their knowledge.
3. Local storage can store what type of data? How would you convert it to that type before storing?
   - `string` data.  Use `JSON.stringify()` to store and `JSON.parse()` to get.

[Back To Top](#index)

