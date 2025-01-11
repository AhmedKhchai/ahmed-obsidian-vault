We're migrating from odoo online (saas) to odoo community (open source) self hosted on a Hetzner server.
## Road blocks
We can not simply import the database into the new instance of odoo as it results in many custom module errors.
This is why the migration will demand good planning.
No Importing ! The goal is to avoid bulk importing as this will be the main database of products and as we've seen before bulk importing result in products being attributed to wrong categories/subcategories so the gaol here is the focus on the quality of data we will add into odoo.
## Plan
An overview of the plan would be to start creating the products and their related data (categores, attributes and eventualy product variants). Then either simultaiously or right after move on to creating the website and its related data: (menus, footers and blogs.) for both alkhayat.net ( That is already created and configured to a domain) and eventualy alqamis.ma (yet to be created and domain configured), while creating the prodcuts its important to focus on adding descriptions in the correct field to enable translation. once this is done we can move on to creating an inventory count for the product variants we've created (fairly simple procedure) 
### Products
- Categories
- Attributes
- Product Variants
### Websites
#### alkhayat.net
#### alqamis.ma
### Inventory
### Translation

## Current State
Categories, Attributes OK
Product price lists to show diff prices in different websites WIP 
Products are being uplaoded with their images, transaltions and variants 77/108
Alkhayat website, homepage, about and contact pages, domain routing OK, Checkout w/ no payment NOK
Alqamiss website WIP

## Follow up
They need to: 
- Create ecommerce categories and subcategories.
- Create price lists.
- Create website tags.
- Translate Alkhayat.net and Alqamiss.com