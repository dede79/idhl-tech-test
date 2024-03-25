## Custom Product Labels (Instructions) ##

There are 5 labels that can be added to the product page in the theme **(Sale, Bestseller, New Drop and Exclusive and Low stock)**. 

All labels are created and managed (text,color and background color) via the metaobjects area in the shopify admin.

### User instructions: ###

Product Settings:

The "custom labels" block is enabled by default. 

Once labels are created in the metaobject area, users can add, remove and reorder as many labels as needed through one metafield reference on each product variant.


**The Sale Label:**

The sale label is also created using metaobjects and can be fully customised. The label can be added when the "compare-at price" field is filled out or removed when the same field is empty.



### Developer instructions: ###


The custom labels use the product_label type metaobject.

the javascript to change labels is leveraging the `renderProductInfo()` function in global.js which updates the variants on click event.

The liquid logic and json schema for the labels are added in the files: 

- `sections/main-product.liquid`
- `sections/main-collection-product-grid.liquid`
- `snippets/card-product.liquid`
- `price.liquid`
- `assets/section-main-product.css`









