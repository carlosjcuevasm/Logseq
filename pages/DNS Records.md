### 1.  **CNAME Records (Aliases)**
- **Yes, CNAMEs are aliases** - they point one domain name to *another domain name*.
- `www.`, `blog.`, `shop.` are all **subdomains** that can use CNAME records.
- Example:
  `www.revista110.do` → CNAME → `your-site.netlify.app`
  (Browser: "Where's [www.revista110.do](http://www.revista110.do)?" → DNS: "It's an alias for your-site.netlify.app")
- ### 2.  **A Records (Address Records)**
- Point **directly to an IP address** (like a physical address).
- Used for root domains (`revista110.do`) because:
	- DNS rules don't allow CNAMEs at the root level
	- Root domains need to handle other critical records (MX for email, etc.)
- ### 3.  **ALIAS/ANAME Records (The Modern Solution)**
- **Hybrid of A + CNAME**: Acts like a CNAME but works at the root level.
- How it works:
  You set: `revista110.do` → ALIAS → `your-site.netlify.app`
  The DNS provider automatically:
	- Looks up the IP of `your-site.netlify.app`
	- Serves it as an A record to users
- **Key difference from A records**:
  If Netlify changes their IPs, ALIAS updates automatically. With A records, you'd need manual updates.
-
-