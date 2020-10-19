# Cloudflare Systems Engineering Assignment

A profiling tool that helps profile the performance of a website using GET requests. The tool supports both HTTP and HTTPS requests. 

## How to build

```sh
$ make build
```

## How to use
Use the flag `--url` to pass in the URL with the scheme included and use the flag `--profile` to pass in the number of GET requests to make
```sh
$ ./main --url https://example.org --profile 10
```
Please note that the tool at this time does NOT follow redirect requests

## Findings

### Facebook (with some of the response)

![Facebook](/images/facebook.png)

### Google

![Google](/images/google.png)

### Cloudflare 

![Cloudflare](/images/cloudflare.png)

### General Assignment (Cloudflare) 

![Facebook](/images/assignment.png)


### Report
1. My cloudflare general assignment deployed on a `workers.dev` Cloudflare domain takes the least median time 
2. The login page for Facebook is the biggest in terms of Content-Length 


