## 4. Creating a new Domain associated with your Edge Application {#creating-domain}

Now that you have your **Edge Application**, we are going to set up a *domain* for it.

On **Real-Time Manager**, your main domain (like `myapp.com`) and all your *subdomains* (like `user.myapp.com`) must be configured each, as a standalone *domain*.

You can access the *Domains* configuration page from the homepage or by clicking the *Products Menu*.

> If you just created and **Edge Application** from *Build from scratch* you can find this page on the "What do you want to do next" section below.

On the *Domains* page, you see all your **Edge Applications**. Click on "Add Domain" and:

* Define an "Configuration Name" by clicking "Add Configuration Name". This should be the same as your **domain name**;
* Select the **Digital Certificate** (can be the standard Azion [SAN] or any third party Digital Certificate).
* Write all Canonical Names (CNAMES) your domain has.
* Mark if you want your users to access your application by CNAME only.
* Select **Edge Application**.
* Make sure it is `Active`.
* Save it!

### Domain provider configuration

Your Domain Name System (DNS) provider must know where to redirect user that access your domain. 

Go to the your DNS provider and add the *link to your **Edge Application*** as an *ALIAS* (also know as *ANAME* or just *A*). 

> This process may change from different DNS providers.

### More information about the required fields to add certificate

| Field | Description |
|-------|-------------|
| Digital Certificate | The usual setup is to use Azion's certificate. If you'd like to add another certificate, head to the menu and look for the Digital Certificates section.<br><br>If you selected HTTP & HTTPS during the creation of your Edge Application, you must select the SSL certificate that will be used to encrypt your HTTPS traffic. Azion provides the certificate Azion (SAN) that can be used for the domains below azioncdn.net.<br><br>You can also upload your Custom Certificate at any time. Consult the Digital Certificates documents and learn how to do it. |
| CNAMEs              | Configure the list of delivery domains (CNAMEs) for your content or application. If necessary, you can use Wildcard Domain (* .yourdomain.com). Example: www.azion.com<br/><br />List the domains you want to use as a URL for your files by hitting enter.<br />Thus, you replace the address provided by Azion (for example, 10001.map.azionedge.net) with the listed domains.<br />In this case, you should register the CNAMEs in your DNS service to redirect any routes of your CNAME to those indicated by Azion.<br />For example, replace www.example.com with 10001.map.azionedge.net. |
| CNAME Access Only  | By default, all Domain configurations are automatically assigned a domain name below azioncdn.net.<br /><br />By checking this option, you will be configuring the Edge Application to deliver your content or applications only through the domains listed in the CNAME field. |
| Edge Application   | Select the Edge Application you want to associate with this delivery domain. |

> Learn more about [**Digital Certificates**](https://www.azion.com/en/documentation/products/edge-application/digital-certificates).
---
