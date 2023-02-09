# Shopify

The tracking checkouts script is used to populate the docs for shopify at https://developers.heap.io/docs/shopify

Helpful shopify docs:
 - [customize order status](https://help.shopify.com/en/manual/orders/status-tracking/customize-order-status)
 - [The checkout object](https://shopify.dev/api/liquid/objects/checkout?shpxid=338ca0c2-FDFC-4D5E-7B41-F6D2FF7FF884)

## Embed 

The code can be embedded in our docs via a short script: 

<iframe id="github-iframe" src=""></iframe>
<script>
    fetch('https://api.github.com/repos/heap/docs-embeds/main/shopify/tracking-checkouts.html')
        .then(function(response) {
            return response.json();
        }).then(function(data) {
            var iframe = document.getElementById('github-iframe');
            iframe.src = 'data:text/html;base64,' + encodeURIComponent(data['content']);
        });
</script>