{% assign email = site.email_url | append: "?subject=" | append: product.info.name %}

Licenses can be purchased from the [Gumroad]({{ product.info.gumroad }}) e-shop. [Reach out]({{ email }}) if you want to include any add-ons, or if you have other support needs or preferred methods of payment or invoicing.


### Enterprise Licenses

The standard tiers are aimed at indie developers, startups and small businesses. Companies and organizations with more than $1M USD in annual proceeds can [reach out for a custom plan]({{ email }}).


### License Terms

By purchasing a license, you acknowledge and approve the [ terms & conditions](terms).


<div class="paper">
    <hr />
</div>


## GitHub

{{ product.info.name }} is hosted at [GitHub]({{ product.info.github }}), where you find the latest version, online documentation, a getting-started guide, code samples, issue tracker, and more.


<div class="paper">
    <hr />
</div>

{% assign products = site.data.products | where:"info.sdk",1 %}
{% include products/products-section.md products=products product=product %}