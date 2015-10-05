This module extends the dataflow module, so categories and child/parent SKUs can be added to the product export. This fork has been specifically optimised to export in a Magmi-compatible format, although it is versatile to export in most formats with custom delimiters.

It contains a parser, which can be used by an advanced profile. This &quot;parser&quot; has this features:
* adding category names to the product export
* removing html tags
* removing linebreaks from the content
* adding absolute image and product links
* adding parent SKUs for simple products that are part of a configurable product
* adding child SKUs for configurable products
* adding gallery image URLs
* Adding full URLs to image fields for Magmi imports
* Adding upsell and cross-sell SKU fields
* Adding related products

This module only can be used to export product data. See the Documentation for more details: 
[English Documentation] (http://www.magentocommerce.com/boards/viewthread/60113/)
[German Documentation] (http://www.magentocommerce.com/boards/viewthread/60111/)

Ability to add parent and child SKUs, cross-sell and up-sell products, image URLs and various other extensions added by Richard Aspden, http://www.insanityinside.net/

See example_configuration.xml for a full dataflow XML example.

If importing this file into Magmi with automatically associating configurable products, it is useful to load the CSV first and sort descending by type, so the simple products are above the configurables, or you may have to import them twice. I recommend using a program which won't mangle the fields, I used LibreOffice Calc 4.1.3.2. YMMV. If dynamically creating categories, delete the category_ids column first, or Magmi will complain.

Work in progress and needs some optimisation. Exporting configurable attributes currently relies on exporting child SKUs, can be seperated later if necessary.</description>

Please note, the package is currently out of date, I'll rebuild it when I get chance. I have just added a modman module for easy cloning though.
