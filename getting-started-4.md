## 4. Creating a new Domain associated with your Edge Application {#creating-domain}

Now that you have finished setting up your **Edge Application**, we are going to configure a *Domain* for it. This process is very important. You will need to have *Domains* configured to connect your Edge Application to many other Azion products.

On [**Real-Time Manager**](https://manager.azion.com/), your main domain (example: `myapp.com`) and all your *subdomains* (example: `user.myapp.com`) must each be configured as a standalone *domain*.

To access the **Domains** configuration page, you can click on "Manage your Domains" from the RTM homepage. You can also find `Domains` at the *Products Menu*.

> If you have just created and **Edge Application** from *Build from scratch* you can find the **Domains** page on the "What do you want to do next" section in the **Launch** page.

On the *Domains* page, you can see all your **Edge Applications** listed. To set up a **Domain**, follow the steps below:

1. Click on **Add Domain**.
1. In "Add Configuration Name", choose a name for your domain.
    > You can use the same as your *domain name*.
1. Select the **Digital Certificate** you will use — it can be the standard *Azion (SAN)* or any third party Digital Certificate.
1. Write all Canonical Names (CNAMES) your domain has.
1. If you want your users to access your application by CNAME only, activate the **CNAME Access Only** switch.
1. In **Edge Application**, select the one your **Domain** will be connected to from the dropdown list.
1. Make sure the **Active** switch is on.
1. Click **Save**.

### Detailed information about the required fields to add a certificate on **Domains**

| Field | Description |
|-------|-------------|
| Digital Certificate | The usual setup is to use Azion's certificate. If you'd like to add another certificate, head to the Products Menu on Real-Time Manager and look for the Digital Certificates section.<br><br>If you've selected HTTP & HTTPS during the creation of your Edge Application, you must select the SSL certificate that will be used to encrypt your HTTPS traffic. Azion provides the Azion (SAN) certificate that can be used for the domains below azioncdn.net.<br><br>You can also upload your Custom Certificate at any time. Consult the Digital Certificates documents and learn how to do it. |
| CNAMEs              | Configure the list of delivery domains (CNAMEs) for your content or application. If necessary, you can use a Wildcard Domain (*.yourdomain.com). Example: www.azion.com<br><br>List the domains you want to use as a URL for your files by hitting enter.<br><br>Thus, you replace the address provided by Azion (for example, 10001.map.azionedge.net) with the listed domains.<br><br>In this case, you should register the CNAMEs in your DNS service to redirect any routes of your CNAME to those indicated by Azion.<br><br>For example, replace www.example.com with 10001.map.azionedge.net. |
| CNAME Access Only  | By default, all Domain configurations are automatically assigned a domain name below map.azionedge.net.<br><br>By checking this option, you will be configuring the Edge Application to deliver your content or applications only through the domains listed in the CNAME field. |
| Edge Application   | Select the Edge Application you want to associate with this delivery domain. |

> Learn more about [**Digital Certificates**](https://www.azion.com/en/documentation/products/edge-application/digital-certificates).
---

