# Extract the domain name from a URL (JavaScript)
Write a function that when given a URL as a string, parses out just the domain name and returns it as a string. For example:

domainName("http://github.com/carbonfive/raygun") == "github" 
domainName("http://www.zombie-bites.com") == "zombie-bites"
domainName("https://www.cnet.com") == "cnet"

# Solution
!! work in progress !!
```javascript
function domainName(url){
  let patt = /(\/{2}|\.)/g;
  let result = url.match(patt);
  console.log(result);
  let sliced = url.slice(url.indexOf(result[0]) + 2, url.indexOf(result[1]));
  return sliced;
}
```
