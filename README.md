# penetration testing

Ethical USE ONLY !!!

Run the following commands:

1.To find subdomains:
```bash
subfinder -d target.com | tee subdomains.txt
```
2.Validate and Filter Your Data (check connection with found subdomains !)
Use a tool like httpx to see which subdomains are active:
```bash
cat subdomains.txt | httpx -silent | tee live_subdomains.txt
```

3.Automatic scan through filterd and live subdomains, checking if they are vulnerable or not !
```bash
subzy run --targets liveSubs.txt
```



