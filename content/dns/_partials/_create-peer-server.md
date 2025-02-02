---
_build:
  publishResources: false
  render: never
  list: never
---

{{<tabs labels="Dashboard | API">}}
{{<tab label="dashboard" no-code="true">}}

To create a peer server using the dashboard:

1. Log in to the [Cloudflare dashboard](https://dash.cloudflare.com/login) and select your account.
2. Go to **Manage Account** > **Configurations**.
3. Select **DNS Zone Transfers**.
4. For **Peer DNS servers**, select **Create**.
5. Enter the following information, paying particular attention to:
    - **IP**: Specifies where Cloudflare sends transfer requests to.
    - **Port**: Specifies the IP Port for the transfer IP.
    - **Enable incremental (IXFR) zone transfers**: Specifies if Cloudflare sends IXFR requests in addition to the default AXFR requests.
    - **Link a an existing TSIG**: If desired, link the TSIG you [previously created](#1-create-tsig-optional).
6. Select **Create**.

{{</tab>}}
{{<tab label="api" no-code="true">}}

To create a peer DNS server using the API, send a [POST request](/api/operations/secondary-dns-(-peer)-create-peer).

{{</tab>}}
{{</tabs>}}