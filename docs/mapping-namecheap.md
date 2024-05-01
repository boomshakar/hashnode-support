---
id: mapping-namecheap
title: Mapping Domain from Namecheap
---

This section covers how to map a domain hosted or purchased on Namecheap to Hashnode.

1. Create an account on [NameCheap](http://namecheap.com/).

![Namecheap Homepage](https://cdn.hashnode.com/res/hashnode/image/upload/v1611181169490/zqRV_MW0X.png?auto=compress)

2. Purchase your preferred domain (example `edidiongasikpo.com`).

3. After completing the purchase, you will be redirected to the product page. Here, you will see your domain.

![Namecheap Product Page](https://cdn.hashnode.com/res/hashnode/image/upload/v1611181430365/vsu-_m3ku.png?auto=compress)

4. Click on the **Manage** button next to your domain to access the DNS management page.

![Namecheap Manage Icon](https://cdn.hashnode.com/res/hashnode/image/upload/v1611181459100/19wTUvj2f.png?auto=compress)

5. Navigate to the **Advanced DNS** tab.

6. Click on the **Add New Record** button in the **Host Records** section.

7. Select **CNAME Record** from the drop-down menu. Enter `@` under host, `hashnode.network` under target, and a **TTL** of 30 minutes.

8. Next, select **A Record** from the drop-down menu. Enter @ under the host, 76.76.21.21 under the value, and **TTL** of 30 minutes.

9. Check for the section titled **NAMESERVERS**, click the drop-down menu and select **Custom DNS**. Two input fields will be revealed,and add the texts below in the input fields.

```
ns1.vercel-dns.com
ns2.vercel-dns.com
```

> Domain propagation (the process whereby nameservers update across the internet to reflect a change in a domain's DNS record) takes 0 - 48 hours to start working in all locations across the internet. Once your domain propagates, we will automatically provision an SSL certificate for you when you visit your blog for the first time.
