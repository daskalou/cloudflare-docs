---
title: Use egress policies to deliver consistent egress IPs
pcx_content_type: learning-unit
weight: 3
layout: learning-unit
---

{{<Aside type="note">}}
Only available on Enterprise plans.
{{</Aside>}}

Egress policies allow you to determine whether your organization's traffic egresses via the default Cloudflare IP or via a [dedicated egress IP](/cloudflare-one/policies/gateway/egress-policies/dedicated-egress-ips/) assigned to your account.

To create a new egress policy:

1. In [Zero Trust](https://one.dash.cloudflare.com/), go to **Gateway** > **Egress Policies**.
2. Select **Add a policy**.
3. Name the policy.
4. Build a logical expression that defines the traffic you want to control egress for. For example, you can add a policy to configure all traffic destined for a thrid-party network to use a static source IP:

   {{<render file="gateway/policies/_egress-destination-ip.md" productFolder="cloudflare-one">}}

5. Select **Create policy**.

For more information, refer to [Egress policies](/cloudflare-one/policies/gateway/egress-policies/).