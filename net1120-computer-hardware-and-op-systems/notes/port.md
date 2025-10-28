Well-known ports (0–1023): Reserved for core services (e.g., HTTP, FTP, SSH).

Registered ports (1024–49151): Used by user applications and services.

Dynamic/private ports (49152–65535): Temporary ports for client-side communication.

Port	Protocol	Service	Security Notes

|number| Protocol| Service| use|
|---|---|---|---|
|20/21|	TCP|	FTP|	Transfers files; unencrypted, vulnerable to sniffing
|22	|TCP	|SSH|	Secure remote login; often brute-forced|
|23|	TCP|	Telnet|	Remote login; transmits in plain text, insecure|
|25	|TCP	|SMTP|	Email sending; exploited for spam relays|
|53	|UDP/TCP|	DNS|	Domain resolution; vulnerable to poisoning|
|80|	TCP|	HTTP|	Web traffic; unencrypted, target for injection attacks|
|443	|TCP|	HTTPS|	Secure web traffic; encrypted, but still targetable|
|110|	TCP|	POP3|	Email retrieval; vulnerable if not encrypted|
|143	|TCP	|IMAP|	Email access; similar risks to POP3|
|3389|	TCP|	RDP|	Remote desktop; high-value target for ransomware|
|445	|TCP	|SMB|	File sharing; exploited in WannaCry and other worms|
|3306	|TCP	|MySQL	|Database access; must be secured from external access|
